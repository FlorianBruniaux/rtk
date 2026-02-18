# Fix Issue #84: rtk git status shows "Clean working tree" outside git repo

## Issue Context

**URL**: https://github.com/rtk-ai/rtk/issues/84
**Reporter**: @ChrisGVE
**Created**: 2026-02-12
**Status**: OPEN

### Problem Description

When `rtk git status` is executed in a directory that is NOT a git repository:

```sh
> rtk git status
Clean working tree

> git status
fatal: not a git repository (or any of the parent directories): .git
```

**Expected behavior**: rtk should propagate git's error and show "fatal: not a git repository" instead of claiming the working tree is clean.

---

## Root Cause Analysis

In `src/git.rs`, function `run_status` (line 525):

### Default Path (no args, lines 557-579)

1. **Line 559-563**: Runs `git status` for tracking with `.unwrap_or_default()` - silently swallows error
2. **Line 565-568**: Runs `git status --porcelain -b` but **NEVER checks `output.status.success()`**
3. **Line 571**: Passes stdout to `format_status_output()`
4. **Line 393-398** in `format_status_output()`: Empty porcelain (`lines.is_empty()`) returns "Clean working tree"

**What happens when git fails**:
- `git status --porcelain -b` returns exit code 128
- stdout is empty
- stderr contains "fatal: not a git repository..."
- The empty stdout becomes "Clean working tree"
- stderr is completely ignored

### Args Path (lines 529-555)

The stderr IS displayed (lines 539-541) but the exit code is NOT propagated when git fails.

---

## Implementation Plan

### Change 1: Default path error handling

**File**: `src/git.rs`
**Location**: After line 568 (after `.context("Failed to run git status")?;`), before line 570 (`let stdout = ...`)

**Insert**:
```rust
if !output.status.success() {
    let stderr = String::from_utf8_lossy(&output.stderr);
    eprintln!("{}", stderr);
    std::process::exit(output.status.code().unwrap_or(1));
}
```

This pattern mirrors `run_log` (lines 347-351).

### Change 2: Args path error handling

**File**: `src/git.rs`
**Location**: After line 534 (after `.context("Failed to run git status")?;`), before line 536 (`let stdout = ...`)

**Insert**:
```rust
if !output.status.success() {
    let stderr = String::from_utf8_lossy(&output.stderr);
    eprintln!("{}", stderr);
    std::process::exit(output.status.code().unwrap_or(1));
}
```

**Note**: Existing stderr printing on lines 539-541 still serves for warnings/verbose output on successful commands.

### Change 3: Smoke test for error propagation

**File**: `scripts/test-all.sh`

**Step 3a**: Add `assert_fails` helper after `assert_help()` (around line 75):

```bash
assert_fails() {
    local name="$1"
    shift
    local output
    if output=$("$@" 2>&1); then
        FAIL=$((FAIL + 1))
        FAILURES+=("$name")
        printf "  ${RED}FAIL${NC}  %s (expected failure, got success)\n" "$name"
    else
        PASS=$((PASS + 1))
        printf "  ${GREEN}PASS${NC}  %s\n" "$name"
    fi
}
```

**Step 3b**: Add test section in git tests section:

```bash
section "Error handling"
# Run rtk git status in /tmp (not a git repo) -- should fail, not show "Clean working tree"
assert_fails "git status outside repo" bash -c "cd /tmp && rtk git status"
assert_fails "git status --short outside repo" bash -c "cd /tmp && rtk git status --short"
```

---

## What NOT to Change

- **`format_status_output`**: Behavior (empty input = "Clean working tree") is correct for clean repos. Bug is upstream.
- **Lines 559-563 (raw_output tracking)**: `.unwrap_or_default()` is fine - process exits at porcelain check before tracking.
- **No unit test for error path**: `std::process::exit()` is not testable in-process. Smoke test covers this.

---

## Verification Steps

```bash
# 1. Unit tests pass (no changes to test behavior)
cargo test git::tests::

# 2. Manual verification
cd /tmp && rtk git status
# Expected: prints "fatal: not a git repository..." to stderr, exits with code 128

cd /tmp && rtk git status --short
# Expected: same error behavior

# 3. Smoke tests
bash scripts/test-all.sh
# Expected: new "Error handling" tests pass

# 4. Pre-commit verification
cargo fmt --all && rtk cargo clippy --all-targets && rtk cargo test
```

---

## Critical Files

- `/Users/florianbruniaux/Sites/perso/rtk/src/git.rs` - Lines ~534 and ~568 (add exit code checks)
- `/Users/florianbruniaux/Sites/perso/rtk/scripts/test-all.sh` - Add `assert_fails` helper + error tests
- Reference pattern: `src/git.rs` lines 347-352 (`run_log` error handling)

---

## Summary

Minimal 2-line fix (same pattern at 2 locations) + smoke tests. Pattern copied from existing `run_log` error handling. No behavioral changes to existing functionality, only proper error propagation when git command fails.
