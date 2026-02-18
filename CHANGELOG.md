# Changelog

All notable changes to rtk (Rust Token Killer) will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0](https://github.com/FlorianBruniaux/rtk/compare/v0.15.4...v1.0.0) (2026-02-18)


### ⚠ BREAKING CHANGES

* Removes --depth, --format (tree/flat/json) flags

### Features

* add --quota flag to rtk gain with tier-based analysis ([26b314d](https://github.com/FlorianBruniaux/rtk/commit/26b314d45b8b0a0c5c39fb0c17001ecbde9d97aa))
* add -A flag to kubectl pods/services for all namespaces ([06816b3](https://github.com/FlorianBruniaux/rtk/commit/06816b36859ab0ac0698ae56d7fa9598557d07ff))
* add chaining instructions to init command ([97ed27a](https://github.com/FlorianBruniaux/rtk/commit/97ed27ad127a0a282ede611a2207fb6f431e113e))
* add CI/CD automation (release management and automated metrics) ([22c3017](https://github.com/FlorianBruniaux/rtk/commit/22c3017ed5d20e5fb6531cfd7aea5e12257e3da9))
* add comprehensive claude code economics analysis ([ec1cf9a](https://github.com/FlorianBruniaux/rtk/commit/ec1cf9a56dd52565516823f55f99a205cfc04558))
* add comprehensive security review workflow for PRs ([1ca6e81](https://github.com/FlorianBruniaux/rtk/commit/1ca6e81bdf16a7eab503d52b342846c3519d89ff))
* add comprehensive security review workflow for PRs ([66101eb](https://github.com/FlorianBruniaux/rtk/commit/66101ebb65076359a1530d8f19e11a17c268bce2))
* add comprehensive temporal audit system for token savings analytics ([76703ca](https://github.com/FlorianBruniaux/rtk/commit/76703ca3f5d73d3345c2ed26e4de86e6df815aff))
* add discover command, auto-rewrite hook, and git show support ([ff1c759](https://github.com/FlorianBruniaux/rtk/commit/ff1c7598c240ca69ab51f507fe45d99d339152a0))
* add execution time tracking to rtk gain analytics ([a3bfbf7](https://github.com/FlorianBruniaux/rtk/commit/a3bfbf747c00979636f9bbe82d973b6ab43dfbca))
* add execution time tracking to rtk gain analytics ([2a1e1a8](https://github.com/FlorianBruniaux/rtk/commit/2a1e1a8ef3afb97080e9e51d7927ea3b5199ddc7))
* add GitHub CLI integration (depends on [#9](https://github.com/FlorianBruniaux/rtk/issues/9)) ([341c485](https://github.com/FlorianBruniaux/rtk/commit/341c48520792f81889543a5dc72e572976856bbb))
* add GitHub CLI integration with token optimizations ([0f7418e](https://github.com/FlorianBruniaux/rtk/commit/0f7418e958b23154cb9dcf52089a64013a666972))
* add JSON parsing with safe fallbacks for vitest, playwright, pnpm ([50ba21e](https://github.com/FlorianBruniaux/rtk/commit/50ba21e2e5fcc2ad5a5f3792f323900d9d5dffe4))
* add local LLM analysis, filter improvements, and testing scripts ([1d85791](https://github.com/FlorianBruniaux/rtk/commit/1d857914d61d569028e3b7b5a90b287fa5260f9f))
* add modern JavaScript tooling support ([b82fa85](https://github.com/FlorianBruniaux/rtk/commit/b82fa85ae5fe0cc1f17d8acab8c6873f436a4d62))
* add modern JavaScript tooling support (lint, tsc, next, prettier, playwright, prisma) ([88c0174](https://github.com/FlorianBruniaux/rtk/commit/88c0174d32e0603f6c5dcc7f969fa8f988573ec6))
* add Modern JS Stack commands to benchmark script ([b868987](https://github.com/FlorianBruniaux/rtk/commit/b868987f6f48876bb2ce9a11c9cad12725401916))
* add parser infrastructure with three-tier fallback system ([6493bc9](https://github.com/FlorianBruniaux/rtk/commit/6493bc92d8c4155cd3b2a5f39fdae846fee2ca81))
* add parser infrastructure with three-tier fallback system ([edab4e1](https://github.com/FlorianBruniaux/rtk/commit/edab4e142eecd81682006ad44c39809e7aae9011))
* add pnpm support (list, outdated, install) ([681729d](https://github.com/FlorianBruniaux/rtk/commit/681729d205705dd7d5e75530486c48abc4aa3d5e))
* add pnpm support + fix git argument parsing for modern stacks ([e574b6d](https://github.com/FlorianBruniaux/rtk/commit/e574b6df3acf2b7eb8dfcb4ba34c3541a42b11ee))
* add Python and Go support ([#88](https://github.com/FlorianBruniaux/rtk/issues/88)) ([30a30ee](https://github.com/FlorianBruniaux/rtk/commit/30a30eefd98396849e0235bd42e293f10c23e500))
* add Python and Go support ([#88](https://github.com/FlorianBruniaux/rtk/issues/88)) ([a005bb1](https://github.com/FlorianBruniaux/rtk/commit/a005bb15c030e16b7b87062317bddf50e12c6f32))
* add quota analysis with multi-tier support ([64c0b03](https://github.com/FlorianBruniaux/rtk/commit/64c0b03d4e4e75a7051eac95be2d562797f1a48a))
* add rtk tree + fix rtk ls + audit phase 1-2 ([278cc57](https://github.com/FlorianBruniaux/rtk/commit/278cc5700bc39770841d157f9c53161f8d62df1e))
* add shared utils module for JS stack commands ([0fc06f9](https://github.com/FlorianBruniaux/rtk/commit/0fc06f95098e00addf06fe71665638ab2beb1aac))
* add SQLite tracking, gain command, and CI/CD ([f8c9a81](https://github.com/FlorianBruniaux/rtk/commit/f8c9a8165f6f2fcc2f9046aa10d27cd85d001f8b))
* add wget command for compact download output ([26796da](https://github.com/FlorianBruniaux/rtk/commit/26796da96a5d1d7d9ad73960957804ff8110d299))
* audit phase 3 + tracking validation + rtk learn ([7975624](https://github.com/FlorianBruniaux/rtk/commit/7975624d0a83c44dfeb073e17fd07dbc62dc8329))
* cargo build/test/clippy with compact output ([bfd5646](https://github.com/FlorianBruniaux/rtk/commit/bfd5646f4eac32b46dbec05f923352a3e50c19ef))
* **cargo:** add `cargo install` filtering with 80-90% token reduction ([645a773](https://github.com/FlorianBruniaux/rtk/commit/645a773a65bb57dc2635aa405a6e2b87534491e3)), closes [#69](https://github.com/FlorianBruniaux/rtk/issues/69)
* **cargo:** add cargo install filtering ([447002f](https://github.com/FlorianBruniaux/rtk/commit/447002f8ba3bbd2b398f85db19b50982df817a02))
* **cargo:** aggregate test output into single line ([#83](https://github.com/FlorianBruniaux/rtk/issues/83)) ([3806c4b](https://github.com/FlorianBruniaux/rtk/commit/3806c4b4234eeb66bdaf2dc5639fbe9cea23d392))
* **cargo:** aggregate test output into single line ([#83](https://github.com/FlorianBruniaux/rtk/issues/83)) ([#85](https://github.com/FlorianBruniaux/rtk/issues/85)) ([06b1049](https://github.com/FlorianBruniaux/rtk/commit/06b10491f926f9eca4323c80d00530a1598ec649))
* CI/CD automation (versioning, benchmarks, README auto-update) ([b8bbfb8](https://github.com/FlorianBruniaux/rtk/commit/b8bbfb87b4dc2b664f64ee3b0231e346a2244055))
* **ci:** automate Homebrew formula update on release ([#80](https://github.com/FlorianBruniaux/rtk/issues/80)) ([a0d2184](https://github.com/FlorianBruniaux/rtk/commit/a0d2184bfef4d0a05225df5a83eedba3c35865b3))
* comprehensive economics analysis and code quality improvements ([8e72e7a](https://github.com/FlorianBruniaux/rtk/commit/8e72e7a8b8ac7e94e9b13958d8b6b8e9bf630660))
* Comprehensive Temporal Audit System for Token Savings Analytics ([862047e](https://github.com/FlorianBruniaux/rtk/commit/862047e387e95b137973983b4ebad810fe5b4431))
* curl with auto-JSON detection ([314accb](https://github.com/FlorianBruniaux/rtk/commit/314accbfd9ac82cc050155c6c47dfb76acab14ce))
* discover command, auto-rewrite hook, git show ([c9c64cf](https://github.com/FlorianBruniaux/rtk/commit/c9c64cfd30e2c867ce1df4be508415635d20132d))
* gh pr create/merge/diff/comment/edit + gh api ([517a93d](https://github.com/FlorianBruniaux/rtk/commit/517a93d0e4497414efe7486410c72afdad5f8a26))
* git branch, fetch, stash, worktree commands ([bc31da8](https://github.com/FlorianBruniaux/rtk/commit/bc31da8ad9d9e91eee8af8020e5bd7008da95dd2))
* **git:** add fallback passthrough for unsupported subcommands ([32bbd02](https://github.com/FlorianBruniaux/rtk/commit/32bbd025345872e46f67e8c999ecc6f71891856b))
* **grep:** add extra args passthrough (-i, -A/-B/-C, etc.) ([a240d1a](https://github.com/FlorianBruniaux/rtk/commit/a240d1a1ee0d94c178d0c54b411eded6c7839599))
* Hook-first installation with 99.5% token reduction ([e7f80ad](https://github.com/FlorianBruniaux/rtk/commit/e7f80ad29481393d16d19f55b3c2171a4b8b7915))
* **init:** auto-patch settings.json for frictionless hook installation ([2db7197](https://github.com/FlorianBruniaux/rtk/commit/2db7197e020857c02857c8ef836279c3fd660baf))
* **init:** auto-patch settings.json for frictionless hook installation ([848a63d](https://github.com/FlorianBruniaux/rtk/commit/848a63dfac5516308bf8050cbb94408b752e8997))
* **init:** refactor to hook-first with slim RTK.md ([9620f66](https://github.com/FlorianBruniaux/rtk/commit/9620f66cd64c299426958d4d3d65bd8d1a9bc92d))
* make install-local.sh self-contained ([#89](https://github.com/FlorianBruniaux/rtk/issues/89)) ([6bcdb3e](https://github.com/FlorianBruniaux/rtk/commit/6bcdb3e5863c064e283d77cff0d337281eb59baa))
* make install-local.sh self-contained ([#89](https://github.com/FlorianBruniaux/rtk/issues/89)) ([b82ad16](https://github.com/FlorianBruniaux/rtk/commit/b82ad168533881757f45e28826cb0c4bd4cc6f97))
* migrate vitest, playwright, pnpm to OutputParser trait ([cf26ad4](https://github.com/FlorianBruniaux/rtk/commit/cf26ad477bdbff448d7eb06725c86cf2805dcdef))
* npm/npx routing, pnpm build/typecheck, --skip-env flag ([49b3cf2](https://github.com/FlorianBruniaux/rtk/commit/49b3cf293d856ff3001c46cff8fee9de9ef501c5))
* **pnpm:** add fallback passthrough for unsupported subcommands ([614ff5c](https://github.com/FlorianBruniaux/rtk/commit/614ff5c13f526f537231aaa9fa098763822b4ee0))
* **python:** add lint dispatcher + universal format command ([#100](https://github.com/FlorianBruniaux/rtk/issues/100)) ([4cae6b6](https://github.com/FlorianBruniaux/rtk/commit/4cae6b6c9a4fbc91c56a99f640d217478b92e6d9))
* **read:** add stdin support via "-" path ([060c38b](https://github.com/FlorianBruniaux/rtk/commit/060c38b3c1ab29070c16c584ea29da3d5ca28f3d))
* rtk tree + fix rtk ls + full audit (phase 1-2-3) ([cb83da1](https://github.com/FlorianBruniaux/rtk/commit/cb83da104f7beba3035225858d7f6eb2979d950c))
* shared infrastructure for new commands ([6c60888](https://github.com/FlorianBruniaux/rtk/commit/6c608880e9ecbb2b3569f875e7fad37d1184d751))
* shared infrastructure for new commands ([9dbc117](https://github.com/FlorianBruniaux/rtk/commit/9dbc1178e7f7fab8a0695b624ed3744ab1a8bf02))
* **sqlite:** add custom sqlite db location ([6e181ae](https://github.com/FlorianBruniaux/rtk/commit/6e181aec087edb50625e08b72fe7abdadbb6c72b))
* **sqlite:** add custom sqlite db location ([93364b5](https://github.com/FlorianBruniaux/rtk/commit/93364b5457619201c656fc2423763fea77633f15))
* ultra-compact kubectl output (summary only, show issues) ([5ed6799](https://github.com/FlorianBruniaux/rtk/commit/5ed679911776d05e43b5650cf35380155e54e982))
* **vitest:** add module with ANSI stripping and test filtering ([62c9b19](https://github.com/FlorianBruniaux/rtk/commit/62c9b19689f70d99d6bffdc5576fcdd819a38f8a))


### Bug Fixes

* 3 issues (latest tag, ccusage fallback, versioning) ([d773ec3](https://github.com/FlorianBruniaux/rtk/commit/d773ec3ea515441e6c62bbac829f45660cfaccde))
* add security validation and error handling to pnpm ([f87be32](https://github.com/FlorianBruniaux/rtk/commit/f87be329b55b0e6a4cd242715ee8f42f75ce9e25))
* add website URL (rtk-ai.app) across project metadata ([#81](https://github.com/FlorianBruniaux/rtk/issues/81)) ([c84fa3c](https://github.com/FlorianBruniaux/rtk/commit/c84fa3c060c7acccaedb617852938c894f30f81e))
* allow git status to accept native flags ([a7ea143](https://github.com/FlorianBruniaux/rtk/commit/a7ea1439fb99a9bd02292068625bed6237f6be0c))
* allow git status to accept native flags ([a27bce8](https://github.com/FlorianBruniaux/rtk/commit/a27bce82f09701cb9df2ed958f682ab5ac8f954e))
* **ci:** correct rust-toolchain action name ([9526471](https://github.com/FlorianBruniaux/rtk/commit/9526471530b7d272f32aca38ace7548fd221547e))
* **ci:** fix release artifacts not uploading ([#73](https://github.com/FlorianBruniaux/rtk/issues/73)) ([bb20b1e](https://github.com/FlorianBruniaux/rtk/commit/bb20b1e9e1619e0d824eb0e0b87109f30bf4f513))
* **ci:** fix release workflow not uploading artifacts to GitHub releases ([bd76b36](https://github.com/FlorianBruniaux/rtk/commit/bd76b361908d10cce508aff6ac443340dcfbdd76))
* comprehensive code quality improvements ([5b840cc](https://github.com/FlorianBruniaux/rtk/commit/5b840cca492ea32488d8c80fd50d3802a0c41c72))
* convert rtk ls from reimplementation to native proxy ([fe4e0f9](https://github.com/FlorianBruniaux/rtk/commit/fe4e0f9976d10957ba3fbd7b221a4db5950a2f3b))
* convert rtk ls from reimplementation to native proxy ([2176369](https://github.com/FlorianBruniaux/rtk/commit/2176369467e00091dfd25f4fef57036e760842f2))
* correct install.sh URL (master not main) ([964601f](https://github.com/FlorianBruniaux/rtk/commit/964601f71018da81b027e2a7eb9ddbb4f09e5ee4))
* correct rust-toolchain action and macos runner ([2d40c7c](https://github.com/FlorianBruniaux/rtk/commit/2d40c7c02d3a79b746f7321aad43f1da9d0dd903))
* **discover:** add cargo check support, wire RtkStatus::Passthrough, enhance rtk init ([d5f8a94](https://github.com/FlorianBruniaux/rtk/commit/d5f8a9460421821861a32eedefc0800fb7720912))
* **docs:** escape HTML tags in rustdoc comments ([b13d92c](https://github.com/FlorianBruniaux/rtk/commit/b13d92c9ea83e28e97847e0a6da696053364bbfc))
* **find:** rewrite with ignore crate + fix json stdin + benchmark pipeline ([fcc1462](https://github.com/FlorianBruniaux/rtk/commit/fcc14624f89a7aa9742de4e7bc7b126d6d030871))
* forward args in rtk git push/pull to support -u, remote, branch ([4bb0130](https://github.com/FlorianBruniaux/rtk/commit/4bb0130695ad2f5d91123afac2e3303e510b240c))
* **git:** accept native git flags in add command (including -A) ([2ade8fe](https://github.com/FlorianBruniaux/rtk/commit/2ade8fe030d8b1bc2fa294aa710ed1f5f877136f))
* **git:** accept native git flags in add command (including -A) ([40e7ead](https://github.com/FlorianBruniaux/rtk/commit/40e7eadbaf0b89a54b63bea73014eac7cf9afb05))
* **git:** fix for issue [#82](https://github.com/FlorianBruniaux/rtk/issues/82) ([04e6bb0](https://github.com/FlorianBruniaux/rtk/commit/04e6bb032ccd67b51fb69e326e27eff66c934043))
* **git:** Returns "Not a git repository" when git status is executed in a non-repo folder [#82](https://github.com/FlorianBruniaux/rtk/issues/82) ([d4cb2c0](https://github.com/FlorianBruniaux/rtk/commit/d4cb2c08100d04755fa776ec8000c0b9673e4370))
* **hook:** use POSIX character classes for cross-platform grep compatibility ([#98](https://github.com/FlorianBruniaux/rtk/issues/98)) ([4aafc83](https://github.com/FlorianBruniaux/rtk/commit/4aafc832d4bdd438609358e2737a96bee4bb2467))
* improve CI reliability and hook coverage ([#95](https://github.com/FlorianBruniaux/rtk/issues/95)) ([50bb494](https://github.com/FlorianBruniaux/rtk/commit/50bb4943f73d8bf9c615155485f7efed802e64d6))
* improve CI reliability and hook coverage ([#95](https://github.com/FlorianBruniaux/rtk/issues/95)) ([ac80bfa](https://github.com/FlorianBruniaux/rtk/commit/ac80bfa88f91dfaf562cdd786ecd3048c554e4f7))
* improve command robustness and flag support ([c2cd691](https://github.com/FlorianBruniaux/rtk/commit/c2cd691c823c8b1dd20d50d01486664f7fd7bd28))
* improve command robustness and flag support ([d7d8c65](https://github.com/FlorianBruniaux/rtk/commit/d7d8c65b86d44792e30ce3d0aff9d90af0dd49ed))
* improve error handling and merge commit detection ([d3b7301](https://github.com/FlorianBruniaux/rtk/commit/d3b7301e21a1fbb8aff91306e66e274ee2a7c5c7))
* **ls:** compact output (-72% tokens) + fix discover panic ([ea7cdb7](https://github.com/FlorianBruniaux/rtk/commit/ea7cdb7a3b622f62e0a085144a637a22108ffdb7))
* optimize HashMap merge and add safety checks ([3b847f8](https://github.com/FlorianBruniaux/rtk/commit/3b847f863a90b2e9a9b7eb570f700a376bce8b22))
* P0 crashes + cargo check + dedup utilities + discover status ([05078ff](https://github.com/FlorianBruniaux/rtk/commit/05078ff2dab0c8745b9fb44b1d462c0d32ae8d77))
* P0 crashes + cargo check + dedup utilities + discover status ([60d2d25](https://github.com/FlorianBruniaux/rtk/commit/60d2d252efbedaebae750b3122385b2377ab01eb))
* pass git flags transparently to git command ([93f9fbe](https://github.com/FlorianBruniaux/rtk/commit/93f9fbedb4eb485989bc9a59a17bc5ff5bf9aac7))
* patrick's 3 issues (latest tag, ccusage fallback, versioning) ([9e322e2](https://github.com/FlorianBruniaux/rtk/commit/9e322e2aee9f7239cf04ce1bf9971920035ac4bb))
* prevent UTF-8 panics on multi-byte characters ([#93](https://github.com/FlorianBruniaux/rtk/issues/93)) ([155e264](https://github.com/FlorianBruniaux/rtk/commit/155e26423d1fe2acbaed3dc1aab8c365324d53e0))
* release pipeline trigger and version-agnostic package URLs ([108d0b5](https://github.com/FlorianBruniaux/rtk/commit/108d0b5ea316ab33c6998fb57b2caf8c65ebe3ef))
* release pipeline trigger and version-agnostic package URLs ([264539c](https://github.com/FlorianBruniaux/rtk/commit/264539cf20a29de0d9a1a39029c04cb8eb1b8f10))
* show full error output on git command failures ([1f1576a](https://github.com/FlorianBruniaux/rtk/commit/1f1576a6576f74209d8042fe3c81b040c4efe875))
* trigger release build after release-please creates tag ([3ddffdd](https://github.com/FlorianBruniaux/rtk/commit/3ddffddc6dc34dacbf5f9dd32dd71bacaa8b0881))
* trigger release build after release-please creates tag ([3b44ef9](https://github.com/FlorianBruniaux/rtk/commit/3b44ef98651906ccc44cdaa77c5434c3f033f462))
* **tsc:** show every TypeScript error instead of collapsing by code ([3df8ce5](https://github.com/FlorianBruniaux/rtk/commit/3df8ce552585d8d0a36f9c938d381ac0bc07b220))
* **tsc:** show every TypeScript error instead of collapsing by code ([67e8de8](https://github.com/FlorianBruniaux/rtk/commit/67e8de8732363d111583e5b514d05e092355b97e))
* update stale repo URLs from pszymkowiak/rtk to rtk-ai/rtk ([#78](https://github.com/FlorianBruniaux/rtk/issues/78)) ([55d010a](https://github.com/FlorianBruniaux/rtk/commit/55d010ad5eced14f525e659f9f35d051644a1246))
* **vitest:** improve parser to handle real Vitest output format ([fc1ed38](https://github.com/FlorianBruniaux/rtk/commit/fc1ed38f40e766d59d43325549b3e0c8b2944f21))
* **vitest:** robust JSON extraction for pnpm/dotenv prefixes ([#92](https://github.com/FlorianBruniaux/rtk/issues/92)) ([ab43e4b](https://github.com/FlorianBruniaux/rtk/commit/ab43e4b8231d977e561a963b2218b122a57183b7))
* **vitest:** robust JSON extraction for pnpm/dotenv prefixes ([#92](https://github.com/FlorianBruniaux/rtk/issues/92)) ([e5adba8](https://github.com/FlorianBruniaux/rtk/commit/e5adba8b214a6609cf1a2cda05f21bcf2a1adb94))

## [0.15.4](https://github.com/rtk-ai/rtk/compare/v0.15.3...v0.15.4) (2026-02-14)


### Bug Fixes

* **git:** fix for issue [#82](https://github.com/rtk-ai/rtk/issues/82) ([04e6bb0](https://github.com/rtk-ai/rtk/commit/04e6bb032ccd67b51fb69e326e27eff66c934043))
* **git:** Returns "Not a git repository" when git status is executed in a non-repo folder [#82](https://github.com/rtk-ai/rtk/issues/82) ([d4cb2c0](https://github.com/rtk-ai/rtk/commit/d4cb2c08100d04755fa776ec8000c0b9673e4370))

## [0.15.3](https://github.com/rtk-ai/rtk/compare/v0.15.2...v0.15.3) (2026-02-13)


### Bug Fixes

* prevent UTF-8 panics on multi-byte characters ([#93](https://github.com/rtk-ai/rtk/issues/93)) ([155e264](https://github.com/rtk-ai/rtk/commit/155e26423d1fe2acbaed3dc1aab8c365324d53e0))

## [0.15.2](https://github.com/rtk-ai/rtk/compare/v0.15.1...v0.15.2) (2026-02-13)


### Bug Fixes

* **hook:** use POSIX character classes for cross-platform grep compatibility ([#98](https://github.com/rtk-ai/rtk/issues/98)) ([4aafc83](https://github.com/rtk-ai/rtk/commit/4aafc832d4bdd438609358e2737a96bee4bb2467))

## [0.15.1](https://github.com/rtk-ai/rtk/compare/v0.15.0...v0.15.1) (2026-02-12)


### Bug Fixes

* improve CI reliability and hook coverage ([#95](https://github.com/rtk-ai/rtk/issues/95)) ([ac80bfa](https://github.com/rtk-ai/rtk/commit/ac80bfa88f91dfaf562cdd786ecd3048c554e4f7))
* **vitest:** robust JSON extraction for pnpm/dotenv prefixes ([#92](https://github.com/rtk-ai/rtk/issues/92)) ([e5adba8](https://github.com/rtk-ai/rtk/commit/e5adba8b214a6609cf1a2cda05f21bcf2a1adb94))

## [0.15.0](https://github.com/rtk-ai/rtk/compare/v0.14.0...v0.15.0) (2026-02-12)


### Features

* add Python and Go support ([#88](https://github.com/rtk-ai/rtk/issues/88)) ([a005bb1](https://github.com/rtk-ai/rtk/commit/a005bb15c030e16b7b87062317bddf50e12c6f32))
* **cargo:** aggregate test output into single line ([#83](https://github.com/rtk-ai/rtk/issues/83)) ([#85](https://github.com/rtk-ai/rtk/issues/85)) ([06b1049](https://github.com/rtk-ai/rtk/commit/06b10491f926f9eca4323c80d00530a1598ec649))
* make install-local.sh self-contained ([#89](https://github.com/rtk-ai/rtk/issues/89)) ([b82ad16](https://github.com/rtk-ai/rtk/commit/b82ad168533881757f45e28826cb0c4bd4cc6f97))

## [0.14.0](https://github.com/rtk-ai/rtk/compare/v0.13.1...v0.14.0) (2026-02-12)


### Features

* **ci:** automate Homebrew formula update on release ([#80](https://github.com/rtk-ai/rtk/issues/80)) ([a0d2184](https://github.com/rtk-ai/rtk/commit/a0d2184bfef4d0a05225df5a83eedba3c35865b3))


### Bug Fixes

* add website URL (rtk-ai.app) across project metadata ([#81](https://github.com/rtk-ai/rtk/issues/81)) ([c84fa3c](https://github.com/rtk-ai/rtk/commit/c84fa3c060c7acccaedb617852938c894f30f81e))
* update stale repo URLs from pszymkowiak/rtk to rtk-ai/rtk ([#78](https://github.com/rtk-ai/rtk/issues/78)) ([55d010a](https://github.com/rtk-ai/rtk/commit/55d010ad5eced14f525e659f9f35d051644a1246))

## [0.13.1](https://github.com/rtk-ai/rtk/compare/v0.13.0...v0.13.1) (2026-02-12)


### Bug Fixes

* **ci:** fix release artifacts not uploading ([#73](https://github.com/rtk-ai/rtk/issues/73)) ([bb20b1e](https://github.com/rtk-ai/rtk/commit/bb20b1e9e1619e0d824eb0e0b87109f30bf4f513))
* **ci:** fix release workflow not uploading artifacts to GitHub releases ([bd76b36](https://github.com/rtk-ai/rtk/commit/bd76b361908d10cce508aff6ac443340dcfbdd76))

## [0.13.0](https://github.com/rtk-ai/rtk/compare/v0.12.0...v0.13.0) (2026-02-12)


### Features

* **sqlite:** add custom sqlite db location ([6e181ae](https://github.com/rtk-ai/rtk/commit/6e181aec087edb50625e08b72fe7abdadbb6c72b))
* **sqlite:** add custom sqlite db location ([93364b5](https://github.com/rtk-ai/rtk/commit/93364b5457619201c656fc2423763fea77633f15))

## [0.12.0](https://github.com/rtk-ai/rtk/compare/v0.11.0...v0.12.0) (2026-02-09)


### Features

* **cargo:** add `cargo install` filtering with 80-90% token reduction ([645a773](https://github.com/rtk-ai/rtk/commit/645a773a65bb57dc2635aa405a6e2b87534491e3)), closes [#69](https://github.com/rtk-ai/rtk/issues/69)
* **cargo:** add cargo install filtering ([447002f](https://github.com/rtk-ai/rtk/commit/447002f8ba3bbd2b398f85db19b50982df817a02))

## [0.11.0](https://github.com/rtk-ai/rtk/compare/v0.10.0...v0.11.0) (2026-02-07)


### Features

* **init:** auto-patch settings.json for frictionless hook installation ([2db7197](https://github.com/rtk-ai/rtk/commit/2db7197e020857c02857c8ef836279c3fd660baf))

## [Unreleased]

### Added
- **settings.json auto-patch** for frictionless hook installation
  - Default `rtk init -g` now prompts to patch settings.json [y/N]
  - `--auto-patch`: Patch immediately without prompting (CI/CD workflows)
  - `--no-patch`: Skip patching, print manual instructions instead
  - Automatic backup: creates `settings.json.bak` before modification
  - Idempotent: detects existing hook, skips modification if present
  - `rtk init --show` now displays settings.json status
- **Uninstall command** for complete RTK removal
  - `rtk init -g --uninstall` removes hook, RTK.md, CLAUDE.md reference, and settings.json entry
  - Restores clean state for fresh installation or testing
- **Improved error handling** with detailed context messages
  - All error messages now include file paths and actionable hints
  - UTF-8 validation for hook paths
  - Disk space hints on write failures

### Changed
- Refactored `insert_hook_entry()` to use idiomatic Rust `entry()` API
- Simplified `hook_already_present()` logic with iterator chains
- Improved atomic write error messages for better debugging
## [0.10.0](https://github.com/rtk-ai/rtk/compare/v0.9.4...v0.10.0) (2026-02-07)


### Features

* Hook-first installation with 99.5% token reduction ([e7f80ad](https://github.com/rtk-ai/rtk/commit/e7f80ad29481393d16d19f55b3c2171a4b8b7915))
* **init:** refactor to hook-first with slim RTK.md ([9620f66](https://github.com/rtk-ai/rtk/commit/9620f66cd64c299426958d4d3d65bd8d1a9bc92d))

## [0.9.4](https://github.com/rtk-ai/rtk/compare/v0.9.3...v0.9.4) (2026-02-06)


### Bug Fixes

* **discover:** add cargo check support, wire RtkStatus::Passthrough, enhance rtk init ([d5f8a94](https://github.com/rtk-ai/rtk/commit/d5f8a9460421821861a32eedefc0800fb7720912))

## [0.9.3](https://github.com/rtk-ai/rtk/compare/v0.9.2...v0.9.3) (2026-02-06)


### Bug Fixes

* P0 crashes + cargo check + dedup utilities + discover status ([05078ff](https://github.com/rtk-ai/rtk/commit/05078ff2dab0c8745b9fb44b1d462c0d32ae8d77))
* P0 crashes + cargo check + dedup utilities + discover status ([60d2d25](https://github.com/rtk-ai/rtk/commit/60d2d252efbedaebae750b3122385b2377ab01eb))

## [0.9.2](https://github.com/rtk-ai/rtk/compare/v0.9.1...v0.9.2) (2026-02-05)


### Bug Fixes

* **git:** accept native git flags in add command (including -A) ([2ade8fe](https://github.com/rtk-ai/rtk/commit/2ade8fe030d8b1bc2fa294aa710ed1f5f877136f))
* **git:** accept native git flags in add command (including -A) ([40e7ead](https://github.com/rtk-ai/rtk/commit/40e7eadbaf0b89a54b63bea73014eac7cf9afb05))

## [0.9.1](https://github.com/rtk-ai/rtk/compare/v0.9.0...v0.9.1) (2026-02-04)


### Bug Fixes

* **tsc:** show every TypeScript error instead of collapsing by code ([3df8ce5](https://github.com/rtk-ai/rtk/commit/3df8ce552585d8d0a36f9c938d381ac0bc07b220))
* **tsc:** show every TypeScript error instead of collapsing by code ([67e8de8](https://github.com/rtk-ai/rtk/commit/67e8de8732363d111583e5b514d05e092355b97e))

## [0.9.0](https://github.com/rtk-ai/rtk/compare/v0.8.1...v0.9.0) (2026-02-03)


### Features

* add rtk tree + fix rtk ls + audit phase 1-2 ([278cc57](https://github.com/rtk-ai/rtk/commit/278cc5700bc39770841d157f9c53161f8d62df1e))
* audit phase 3 + tracking validation + rtk learn ([7975624](https://github.com/rtk-ai/rtk/commit/7975624d0a83c44dfeb073e17fd07dbc62dc8329))
* **git:** add fallback passthrough for unsupported subcommands ([32bbd02](https://github.com/rtk-ai/rtk/commit/32bbd025345872e46f67e8c999ecc6f71891856b))
* **grep:** add extra args passthrough (-i, -A/-B/-C, etc.) ([a240d1a](https://github.com/rtk-ai/rtk/commit/a240d1a1ee0d94c178d0c54b411eded6c7839599))
* **pnpm:** add fallback passthrough for unsupported subcommands ([614ff5c](https://github.com/rtk-ai/rtk/commit/614ff5c13f526f537231aaa9fa098763822b4ee0))
* **read:** add stdin support via "-" path ([060c38b](https://github.com/rtk-ai/rtk/commit/060c38b3c1ab29070c16c584ea29da3d5ca28f3d))
* rtk tree + fix rtk ls + full audit (phase 1-2-3) ([cb83da1](https://github.com/rtk-ai/rtk/commit/cb83da104f7beba3035225858d7f6eb2979d950c))


### Bug Fixes

* **docs:** escape HTML tags in rustdoc comments ([b13d92c](https://github.com/rtk-ai/rtk/commit/b13d92c9ea83e28e97847e0a6da696053364bbfc))
* **find:** rewrite with ignore crate + fix json stdin + benchmark pipeline ([fcc1462](https://github.com/rtk-ai/rtk/commit/fcc14624f89a7aa9742de4e7bc7b126d6d030871))
* **ls:** compact output (-72% tokens) + fix discover panic ([ea7cdb7](https://github.com/rtk-ai/rtk/commit/ea7cdb7a3b622f62e0a085144a637a22108ffdb7))

## [0.8.1](https://github.com/rtk-ai/rtk/compare/v0.8.0...v0.8.1) (2026-02-02)


### Bug Fixes

* allow git status to accept native flags ([a7ea143](https://github.com/rtk-ai/rtk/commit/a7ea1439fb99a9bd02292068625bed6237f6be0c))
* allow git status to accept native flags ([a27bce8](https://github.com/rtk-ai/rtk/commit/a27bce82f09701cb9df2ed958f682ab5ac8f954e))

## [0.8.0](https://github.com/rtk-ai/rtk/compare/v0.7.1...v0.8.0) (2026-02-02)


### Features

* add comprehensive security review workflow for PRs ([1ca6e81](https://github.com/rtk-ai/rtk/commit/1ca6e81bdf16a7eab503d52b342846c3519d89ff))
* add comprehensive security review workflow for PRs ([66101eb](https://github.com/rtk-ai/rtk/commit/66101ebb65076359a1530d8f19e11a17c268bce2))

## [0.7.1](https://github.com/pszymkowiak/rtk/compare/v0.7.0...v0.7.1) (2026-02-02)


### Features

* **execution time tracking**: Add command execution time metrics to `rtk gain` analytics
  - Total execution time and average time per command displayed in summary
  - Time column in "By Command" breakdown showing average execution duration
  - Daily breakdown (`--daily`) includes time metrics per day
  - JSON export includes `total_time_ms` and `avg_time_ms` fields
  - CSV export includes execution time columns
  - Backward compatible: historical data shows 0ms (pre-tracking)
  - Negligible overhead: <0.1ms per command
  - New SQLite column: `exec_time_ms` in commands table
* **parser infrastructure**: Three-tier fallback system for robust output parsing
  - Tier 1: Full JSON parsing with complete structured data
  - Tier 2: Degraded parsing with regex fallback and warnings
  - Tier 3: Passthrough with truncated raw output and error markers
  - Guarantees RTK never returns false data silently
* **migrate commands to OutputParser**: vitest, playwright, pnpm now use robust parsing
  - JSON parsing with safe fallbacks for all modern JS tooling
  - Improved error handling and debugging visibility
* **local LLM analysis**: Add economics analysis and comprehensive test scripts
  - `scripts/rtk-economics.sh` for token savings ROI analysis
  - `scripts/test-all.sh` with 69 assertions covering all commands
  - `scripts/test-aristote.sh` for T3 Stack project validation


### Bug Fixes

* convert rtk ls from reimplementation to native proxy for better reliability
* trigger release build after release-please creates tag


### Documentation

* add execution time tracking test guide (TEST_EXEC_TIME.md)
* comprehensive parser infrastructure documentation (src/parser/README.md)

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

- **Repository**: https://github.com/rtk-ai/rtk (maintained by pszymkowiak)
- **Issues**: https://github.com/rtk-ai/rtk/issues
