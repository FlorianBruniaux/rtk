# Changelog

All notable changes to rtk (Rust Token Killer) will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0](https://github.com/FlorianBruniaux/rtk/compare/v0.7.0...v1.0.0) (2026-02-02)


### ⚠ BREAKING CHANGES

* Removes --depth, --format (tree/flat/json) flags

### Features

* add --quota flag to rtk gain with tier-based analysis ([26b314d](https://github.com/FlorianBruniaux/rtk/commit/26b314d45b8b0a0c5c39fb0c17001ecbde9d97aa))
* add -A flag to kubectl pods/services for all namespaces ([06816b3](https://github.com/FlorianBruniaux/rtk/commit/06816b36859ab0ac0698ae56d7fa9598557d07ff))
* add chaining instructions to init command ([97ed27a](https://github.com/FlorianBruniaux/rtk/commit/97ed27ad127a0a282ede611a2207fb6f431e113e))
* add CI/CD automation (release management and automated metrics) ([22c3017](https://github.com/FlorianBruniaux/rtk/commit/22c3017ed5d20e5fb6531cfd7aea5e12257e3da9))
* add comprehensive claude code economics analysis ([ec1cf9a](https://github.com/FlorianBruniaux/rtk/commit/ec1cf9a56dd52565516823f55f99a205cfc04558))
* add comprehensive temporal audit system for token savings analytics ([76703ca](https://github.com/FlorianBruniaux/rtk/commit/76703ca3f5d73d3345c2ed26e4de86e6df815aff))
* add discover command, auto-rewrite hook, and git show support ([ff1c759](https://github.com/FlorianBruniaux/rtk/commit/ff1c7598c240ca69ab51f507fe45d99d339152a0))
* add execution time tracking to rtk gain analytics ([a3bfbf7](https://github.com/FlorianBruniaux/rtk/commit/a3bfbf747c00979636f9bbe82d973b6ab43dfbca))
* add execution time tracking to rtk gain analytics ([2a1e1a8](https://github.com/FlorianBruniaux/rtk/commit/2a1e1a8ef3afb97080e9e51d7927ea3b5199ddc7))
* add GitHub CLI integration (depends on [#9](https://github.com/FlorianBruniaux/rtk/issues/9)) ([341c485](https://github.com/FlorianBruniaux/rtk/commit/341c48520792f81889543a5dc72e572976856bbb))
* add GitHub CLI integration with token optimizations ([0f7418e](https://github.com/FlorianBruniaux/rtk/commit/0f7418e958b23154cb9dcf52089a64013a666972))
* add modern JavaScript tooling support ([b82fa85](https://github.com/FlorianBruniaux/rtk/commit/b82fa85ae5fe0cc1f17d8acab8c6873f436a4d62))
* add modern JavaScript tooling support (lint, tsc, next, prettier, playwright, prisma) ([88c0174](https://github.com/FlorianBruniaux/rtk/commit/88c0174d32e0603f6c5dcc7f969fa8f988573ec6))
* add Modern JS Stack commands to benchmark script ([b868987](https://github.com/FlorianBruniaux/rtk/commit/b868987f6f48876bb2ce9a11c9cad12725401916))
* add pnpm support (list, outdated, install) ([681729d](https://github.com/FlorianBruniaux/rtk/commit/681729d205705dd7d5e75530486c48abc4aa3d5e))
* add pnpm support + fix git argument parsing for modern stacks ([e574b6d](https://github.com/FlorianBruniaux/rtk/commit/e574b6df3acf2b7eb8dfcb4ba34c3541a42b11ee))
* add quota analysis with multi-tier support ([64c0b03](https://github.com/FlorianBruniaux/rtk/commit/64c0b03d4e4e75a7051eac95be2d562797f1a48a))
* add shared utils module for JS stack commands ([0fc06f9](https://github.com/FlorianBruniaux/rtk/commit/0fc06f95098e00addf06fe71665638ab2beb1aac))
* add SQLite tracking, gain command, and CI/CD ([f8c9a81](https://github.com/FlorianBruniaux/rtk/commit/f8c9a8165f6f2fcc2f9046aa10d27cd85d001f8b))
* add wget command for compact download output ([26796da](https://github.com/FlorianBruniaux/rtk/commit/26796da96a5d1d7d9ad73960957804ff8110d299))
* cargo build/test/clippy with compact output ([bfd5646](https://github.com/FlorianBruniaux/rtk/commit/bfd5646f4eac32b46dbec05f923352a3e50c19ef))
* CI/CD automation (versioning, benchmarks, README auto-update) ([b8bbfb8](https://github.com/FlorianBruniaux/rtk/commit/b8bbfb87b4dc2b664f64ee3b0231e346a2244055))
* comprehensive economics analysis and code quality improvements ([8e72e7a](https://github.com/FlorianBruniaux/rtk/commit/8e72e7a8b8ac7e94e9b13958d8b6b8e9bf630660))
* Comprehensive Temporal Audit System for Token Savings Analytics ([862047e](https://github.com/FlorianBruniaux/rtk/commit/862047e387e95b137973983b4ebad810fe5b4431))
* curl with auto-JSON detection ([314accb](https://github.com/FlorianBruniaux/rtk/commit/314accbfd9ac82cc050155c6c47dfb76acab14ce))
* discover command, auto-rewrite hook, git show ([c9c64cf](https://github.com/FlorianBruniaux/rtk/commit/c9c64cfd30e2c867ce1df4be508415635d20132d))
* gh pr create/merge/diff/comment/edit + gh api ([517a93d](https://github.com/FlorianBruniaux/rtk/commit/517a93d0e4497414efe7486410c72afdad5f8a26))
* git branch, fetch, stash, worktree commands ([bc31da8](https://github.com/FlorianBruniaux/rtk/commit/bc31da8ad9d9e91eee8af8020e5bd7008da95dd2))
* npm/npx routing, pnpm build/typecheck, --skip-env flag ([49b3cf2](https://github.com/FlorianBruniaux/rtk/commit/49b3cf293d856ff3001c46cff8fee9de9ef501c5))
* shared infrastructure for new commands ([6c60888](https://github.com/FlorianBruniaux/rtk/commit/6c608880e9ecbb2b3569f875e7fad37d1184d751))
* shared infrastructure for new commands ([9dbc117](https://github.com/FlorianBruniaux/rtk/commit/9dbc1178e7f7fab8a0695b624ed3744ab1a8bf02))
* ultra-compact kubectl output (summary only, show issues) ([5ed6799](https://github.com/FlorianBruniaux/rtk/commit/5ed679911776d05e43b5650cf35380155e54e982))
* **vitest:** add module with ANSI stripping and test filtering ([62c9b19](https://github.com/FlorianBruniaux/rtk/commit/62c9b19689f70d99d6bffdc5576fcdd819a38f8a))


### Bug Fixes

* 3 issues (latest tag, ccusage fallback, versioning) ([d773ec3](https://github.com/FlorianBruniaux/rtk/commit/d773ec3ea515441e6c62bbac829f45660cfaccde))
* add security validation and error handling to pnpm ([f87be32](https://github.com/FlorianBruniaux/rtk/commit/f87be329b55b0e6a4cd242715ee8f42f75ce9e25))
* **ci:** correct rust-toolchain action name ([9526471](https://github.com/FlorianBruniaux/rtk/commit/9526471530b7d272f32aca38ace7548fd221547e))
* comprehensive code quality improvements ([5b840cc](https://github.com/FlorianBruniaux/rtk/commit/5b840cca492ea32488d8c80fd50d3802a0c41c72))
* convert rtk ls from reimplementation to native proxy ([fe4e0f9](https://github.com/FlorianBruniaux/rtk/commit/fe4e0f9976d10957ba3fbd7b221a4db5950a2f3b))
* convert rtk ls from reimplementation to native proxy ([2176369](https://github.com/FlorianBruniaux/rtk/commit/2176369467e00091dfd25f4fef57036e760842f2))
* correct install.sh URL (master not main) ([964601f](https://github.com/FlorianBruniaux/rtk/commit/964601f71018da81b027e2a7eb9ddbb4f09e5ee4))
* correct rust-toolchain action and macos runner ([2d40c7c](https://github.com/FlorianBruniaux/rtk/commit/2d40c7c02d3a79b746f7321aad43f1da9d0dd903))
* forward args in rtk git push/pull to support -u, remote, branch ([4bb0130](https://github.com/FlorianBruniaux/rtk/commit/4bb0130695ad2f5d91123afac2e3303e510b240c))
* improve command robustness and flag support ([c2cd691](https://github.com/FlorianBruniaux/rtk/commit/c2cd691c823c8b1dd20d50d01486664f7fd7bd28))
* improve command robustness and flag support ([d7d8c65](https://github.com/FlorianBruniaux/rtk/commit/d7d8c65b86d44792e30ce3d0aff9d90af0dd49ed))
* improve error handling and merge commit detection ([d3b7301](https://github.com/FlorianBruniaux/rtk/commit/d3b7301e21a1fbb8aff91306e66e274ee2a7c5c7))
* optimize HashMap merge and add safety checks ([3b847f8](https://github.com/FlorianBruniaux/rtk/commit/3b847f863a90b2e9a9b7eb570f700a376bce8b22))
* pass git flags transparently to git command ([93f9fbe](https://github.com/FlorianBruniaux/rtk/commit/93f9fbedb4eb485989bc9a59a17bc5ff5bf9aac7))
* patrick's 3 issues (latest tag, ccusage fallback, versioning) ([9e322e2](https://github.com/FlorianBruniaux/rtk/commit/9e322e2aee9f7239cf04ce1bf9971920035ac4bb))
* release pipeline trigger and version-agnostic package URLs ([108d0b5](https://github.com/FlorianBruniaux/rtk/commit/108d0b5ea316ab33c6998fb57b2caf8c65ebe3ef))
* release pipeline trigger and version-agnostic package URLs ([264539c](https://github.com/FlorianBruniaux/rtk/commit/264539cf20a29de0d9a1a39029c04cb8eb1b8f10))
* show full error output on git command failures ([1f1576a](https://github.com/FlorianBruniaux/rtk/commit/1f1576a6576f74209d8042fe3c81b040c4efe875))
* trigger release build after release-please creates tag ([3ddffdd](https://github.com/FlorianBruniaux/rtk/commit/3ddffddc6dc34dacbf5f9dd32dd71bacaa8b0881))
* trigger release build after release-please creates tag ([3b44ef9](https://github.com/FlorianBruniaux/rtk/commit/3b44ef98651906ccc44cdaa77c5434c3f033f462))
* **vitest:** improve parser to handle real Vitest output format ([fc1ed38](https://github.com/FlorianBruniaux/rtk/commit/fc1ed38f40e766d59d43325549b3e0c8b2944f21))

## [0.7.0](https://github.com/pszymkowiak/rtk/compare/v0.6.0...v0.7.0) (2026-02-01)


### Features

* add discover command, auto-rewrite hook, and git show support ([ff1c759](https://github.com/pszymkowiak/rtk/commit/ff1c7598c240ca69ab51f507fe45d99d339152a0))
* discover command, auto-rewrite hook, git show ([c9c64cf](https://github.com/pszymkowiak/rtk/commit/c9c64cfd30e2c867ce1df4be508415635d20132d))


### Bug Fixes

* forward args in rtk git push/pull to support -u, remote, branch ([4bb0130](https://github.com/pszymkowiak/rtk/commit/4bb0130695ad2f5d91123afac2e3303e510b240c))

## [0.6.0](https://github.com/pszymkowiak/rtk/compare/v0.5.2...v0.6.0) (2026-02-01)


### Features

* cargo build/test/clippy with compact output ([bfd5646](https://github.com/pszymkowiak/rtk/commit/bfd5646f4eac32b46dbec05f923352a3e50c19ef))
* curl with auto-JSON detection ([314accb](https://github.com/pszymkowiak/rtk/commit/314accbfd9ac82cc050155c6c47dfb76acab14ce))
* gh pr create/merge/diff/comment/edit + gh api ([517a93d](https://github.com/pszymkowiak/rtk/commit/517a93d0e4497414efe7486410c72afdad5f8a26))
* git branch, fetch, stash, worktree commands ([bc31da8](https://github.com/pszymkowiak/rtk/commit/bc31da8ad9d9e91eee8af8020e5bd7008da95dd2))
* npm/npx routing, pnpm build/typecheck, --skip-env flag ([49b3cf2](https://github.com/pszymkowiak/rtk/commit/49b3cf293d856ff3001c46cff8fee9de9ef501c5))
* shared infrastructure for new commands ([6c60888](https://github.com/pszymkowiak/rtk/commit/6c608880e9ecbb2b3569f875e7fad37d1184d751))
* shared infrastructure for new commands ([9dbc117](https://github.com/pszymkowiak/rtk/commit/9dbc1178e7f7fab8a0695b624ed3744ab1a8bf02))

## [0.5.2](https://github.com/pszymkowiak/rtk/compare/v0.5.1...v0.5.2) (2026-01-30)


### Bug Fixes

* release pipeline trigger and version-agnostic package URLs ([108d0b5](https://github.com/pszymkowiak/rtk/commit/108d0b5ea316ab33c6998fb57b2caf8c65ebe3ef))
* release pipeline trigger and version-agnostic package URLs ([264539c](https://github.com/pszymkowiak/rtk/commit/264539cf20a29de0d9a1a39029c04cb8eb1b8f10))

## [0.5.1](https://github.com/pszymkowiak/rtk/compare/v0.5.0...v0.5.1) (2026-01-30)


### Bug Fixes

* 3 issues (latest tag, ccusage fallback, versioning) ([d773ec3](https://github.com/pszymkowiak/rtk/commit/d773ec3ea515441e6c62bbac829f45660cfaccde))
* patrick's 3 issues (latest tag, ccusage fallback, versioning) ([9e322e2](https://github.com/pszymkowiak/rtk/commit/9e322e2aee9f7239cf04ce1bf9971920035ac4bb))

## [0.5.0](https://github.com/pszymkowiak/rtk/compare/v0.4.0...v0.5.0) (2026-01-30)


### Features

* add comprehensive claude code economics analysis ([ec1cf9a](https://github.com/pszymkowiak/rtk/commit/ec1cf9a56dd52565516823f55f99a205cfc04558))
* comprehensive economics analysis and code quality improvements ([8e72e7a](https://github.com/pszymkowiak/rtk/commit/8e72e7a8b8ac7e94e9b13958d8b6b8e9bf630660))


### Bug Fixes

* comprehensive code quality improvements ([5b840cc](https://github.com/pszymkowiak/rtk/commit/5b840cca492ea32488d8c80fd50d3802a0c41c72))
* optimize HashMap merge and add safety checks ([3b847f8](https://github.com/pszymkowiak/rtk/commit/3b847f863a90b2e9a9b7eb570f700a376bce8b22))

## [0.4.0](https://github.com/pszymkowiak/rtk/compare/v0.3.1...v0.4.0) (2026-01-30)


### Features

* add comprehensive temporal audit system for token savings analytics ([76703ca](https://github.com/pszymkowiak/rtk/commit/76703ca3f5d73d3345c2ed26e4de86e6df815aff))
* Comprehensive Temporal Audit System for Token Savings Analytics ([862047e](https://github.com/pszymkowiak/rtk/commit/862047e387e95b137973983b4ebad810fe5b4431))

## [0.3.1](https://github.com/pszymkowiak/rtk/compare/v0.3.0...v0.3.1) (2026-01-29)


### Bug Fixes

* improve command robustness and flag support ([c2cd691](https://github.com/pszymkowiak/rtk/commit/c2cd691c823c8b1dd20d50d01486664f7fd7bd28))
* improve command robustness and flag support ([d7d8c65](https://github.com/pszymkowiak/rtk/commit/d7d8c65b86d44792e30ce3d0aff9d90af0dd49ed))

## [0.3.0](https://github.com/pszymkowiak/rtk/compare/v0.2.1...v0.3.0) (2026-01-29)


### Features

* add --quota flag to rtk gain with tier-based analysis ([26b314d](https://github.com/pszymkowiak/rtk/commit/26b314d45b8b0a0c5c39fb0c17001ecbde9d97aa))
* add CI/CD automation (release management and automated metrics) ([22c3017](https://github.com/pszymkowiak/rtk/commit/22c3017ed5d20e5fb6531cfd7aea5e12257e3da9))
* add GitHub CLI integration (depends on [#9](https://github.com/pszymkowiak/rtk/issues/9)) ([341c485](https://github.com/pszymkowiak/rtk/commit/341c48520792f81889543a5dc72e572976856bbb))
* add GitHub CLI integration with token optimizations ([0f7418e](https://github.com/pszymkowiak/rtk/commit/0f7418e958b23154cb9dcf52089a64013a666972))
* add modern JavaScript tooling support ([b82fa85](https://github.com/pszymkowiak/rtk/commit/b82fa85ae5fe0cc1f17d8acab8c6873f436a4d62))
* add modern JavaScript tooling support (lint, tsc, next, prettier, playwright, prisma) ([88c0174](https://github.com/pszymkowiak/rtk/commit/88c0174d32e0603f6c5dcc7f969fa8f988573ec6))
* add Modern JS Stack commands to benchmark script ([b868987](https://github.com/pszymkowiak/rtk/commit/b868987f6f48876bb2ce9a11c9cad12725401916))
* add quota analysis with multi-tier support ([64c0b03](https://github.com/pszymkowiak/rtk/commit/64c0b03d4e4e75a7051eac95be2d562797f1a48a))
* add shared utils module for JS stack commands ([0fc06f9](https://github.com/pszymkowiak/rtk/commit/0fc06f95098e00addf06fe71665638ab2beb1aac))
* CI/CD automation (versioning, benchmarks, README auto-update) ([b8bbfb8](https://github.com/pszymkowiak/rtk/commit/b8bbfb87b4dc2b664f64ee3b0231e346a2244055))


### Bug Fixes

* **ci:** correct rust-toolchain action name ([9526471](https://github.com/pszymkowiak/rtk/commit/9526471530b7d272f32aca38ace7548fd221547e))

## [Unreleased]

### Added
- `prettier` command for format checking with package manager auto-detection (pnpm/yarn/npx)
  - Shows only files needing formatting (~70% token reduction)
  - Exit code preservation for CI/CD compatibility
- `playwright` command for E2E test output filtering (~94% token reduction)
  - Shows only test failures and slow tests
  - Summary with pass/fail counts and timing
- `lint` command with ESLint/Biome support and pnpm detection
  - Groups violations by rule and file (~84% token reduction)
  - Shows top violators for quick navigation
- `tsc` command for TypeScript compiler output filtering
  - Groups errors by file and error code (~83% token reduction)
  - Shows top 10 affected files
- `next` command for Next.js build/dev output filtering (87% token reduction)
  - Extracts route count and bundle sizes
  - Highlights warnings and oversized bundles
- `prisma` command for Prisma CLI output filtering
  - Removes ASCII art and verbose logs (~88% token reduction)
  - Supports generate, migrate (dev/status/deploy), and db push
- `utils` module with common utilities (truncate, strip_ansi, execute_command)
  - Shared functionality for consistent output formatting
  - ANSI escape code stripping for clean parsing

### Changed
- Refactored duplicated code patterns into `utils.rs` module
- Improved package manager detection across all modern JS commands

## [0.2.1] - 2026-01-29

See upstream: https://github.com/pszymkowiak/rtk

## Links

- **Repository**: https://github.com/FlorianBruniaux/rtk (fork)
- **Upstream**: https://github.com/pszymkowiak/rtk
- **Issues**: https://github.com/FlorianBruniaux/rtk/issues
