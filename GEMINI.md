# GEMINI.md - Project Context: rtk (Rust Token Killer)

This file provides comprehensive architectural context and development guidelines for the `rtk` project, intended for use by LLMs and developers.

## Project Overview

**rtk (Rust Token Killer)** is a high-performance CLI proxy designed to minimize LLM token consumption. It sits between the user (or an LLM agent like Claude Code) and the system shell, filtering and compressing command outputs by 60-90% before they reach the LLM's context window.

### Key Technologies
- **Language:** Rust (2021 edition)
- **CLI Framework:** `clap` (v4) with derive macros
- **Storage:** `rusqlite` (bundled SQLite) for tracking token savings
- **Regex:** `regex` crate for output filtering and pattern matching
- **Error Handling:** `anyhow` and `thiserror`
- **Serialization:** `serde` and `serde_json`
- **Config:** `toml`

### Architecture
rtk follows a **command proxy pattern**:
1.  **Intercept:** Receives CLI commands and arguments.
2.  **Route:** Dispatches to specialized modules (e.g., `src/git.rs`, `src/npm_cmd.rs`) based on the subcommand.
3.  **Execute:** Runs the underlying system command (e.g., `git status`) and captures stdout/stderr.
4.  **Filter/Compress:** Applies domain-specific filtering strategies (stats extraction, error-only, grouping, deduplication, etc.).
5.  **Track:** Records token savings (input vs. output) and execution time in a local SQLite database (`~/.local/share/rtk/history.db`).
6.  **Output:** Prints the optimized output to the terminal.

## Core Components

- **`src/main.rs`:** CLI entry point and command router.
- **`src/runner.rs`:** Handles generic command execution with "err" (errors only) and "test" (failures only) filters.
- **`src/filter.rs`:** Implements language-aware code filtering (Rust, Python, JS/TS, etc.) for the `read` and `smart` commands.
- **`src/tracking.rs`:** Manages the SQLite-based token analytics system.
- **`src/utils.rs`:** Shared utilities, including package manager detection (pnpm/yarn/npm) and text processing.
- **`src/discover/`:** Analyzes Claude Code session history to identify missed token savings opportunities.
- **`src/learn/`:** Scans session history for CLI errors and generates corrective rules.

## Building and Running

### Prerequisites
- Rust and Cargo (latest stable)

### Key Commands
- **Build:** `cargo build` (debug) or `cargo build --release` (optimized)
- **Run:** `cargo run -- <command> <args>` (e.g., `cargo run -- git status`)
- **Test:** `cargo test` (runs unit tests)
- **Smoke Tests:** `bash scripts/test-all.sh` (requires `rtk` to be in PATH)
- **Lint:** `cargo clippy --all-targets`
- **Format:** `cargo fmt`

## Development Conventions

- **TDD:** Follow Red-Green-Refactor. Add unit tests for every new filtering logic in the same file using `#[cfg(test)] mod tests`.
- **Exit Code Preservation:** Always propagate the exit code of the underlying tool to ensure compatibility with CI/CD and pre-commit hooks.
- **Verbosity Levels:**
    - `-v`: Show debug messages.
    - `-vv`: Show the exact command being executed.
    - `-vvv`: Show raw output before filtering.
- **Ultra-Compact Mode (`-u`):** Use ASCII icons and inline formatting for maximum token savings.
- **Safety:** Ensure proper handling of `trailing_var_arg` and `allow_hyphen_values` in `clap` to avoid issues with native tool flags (especially for `git`).
- **Idiomatic Rust:** Use `anyhow` for application-level errors and `thiserror` for library-level errors.

## LLM Integration (Claude Code)

rtk is designed to be used with Claude Code via hooks:
- **`rtk-rewrite.sh`:** A `PreToolUse` hook that transparently rewrites standard commands (e.g., `git status`) to their `rtk` equivalents.
- **`RTK.md`:** A minimal context file that instructs the LLM to use `rtk`.
