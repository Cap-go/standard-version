# Changelog

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

### [1.0.6](https://github.com/Cap-go/standard-version/compare/v1.0.5...v1.0.6) (2023-01-12)

## [1.0.5](https://github.com/Cap-go/standard-version/compare/v1.0.4...v1.0.5) (2023-01-12)


### Bug Fixes

* readme ([60b040c](https://github.com/Cap-go/standard-version/commit/60b040cb9eeed1054797d605b62144d8a91860a0))

## [1.0.4](https://github.com/Cap-go/standard-version/compare/v1.0.3...v1.0.4) (2023-01-12)


### Bug Fixes

* issue for deploy ([7c546ee](https://github.com/Cap-go/standard-version/commit/7c546ee693f70c6a61f9d2dda04c476621c8a2b2))

## [1.0.3](https://github.com/Cap-go/standard-version/compare/v1.0.2...v1.0.3) (2023-01-12)


### Bug Fixes

* use normal registry ([9b6191d](https://github.com/Cap-go/standard-version/commit/9b6191d93b31da30d56c74e7d434ea84b2a35ff9))

## [1.0.2](https://github.com/Cap-go/standard-version/compare/v1.0.1...v1.0.2) (2023-01-12)


### Bug Fixes

* ci script use latest ([d9803b8](https://github.com/Cap-go/standard-version/commit/d9803b865655d1de72a4f455fa6e0bf8557e92ad))

## [1.0.1](https://github.com/Cap-go/standard-version/compare/v1.0.0...v1.0.1) (2023-01-12)


### Bug Fixes

* lock missing ([81f28a2](https://github.com/Cap-go/standard-version/commit/81f28a23ccbd06f5db5b66438b9e50803b1db6e7))

## 1.0.0 (2023-01-12)


### ⚠ BREAKING CHANGES

* NodeJS@8 is no longer supported. ([#612](https://github.com/Cap-go/standard-version/issues/612))
* `composer.json` and `composer.lock` will no longer be read from or bumped by default. If you need to obtain a version or write a version to these files, please use `bumpFiles` and/or `packageFiles` options accordingly.
* we were accepting .version.json as a config file, rather than .versionrc.json
* we now bump the minor rather than major if version < 1.0.0; --release-as can be used to bump to 1.0.0.
* tests are no longer run for Node 6
* we now use the conventionalcommits preset by default, which directly tracks conventionalcommits.org.
* if no package.json, bower.json, etc., is found, we now fallback to git tags
* removed Node 4/5 from testing matrix
* merge commits are now included in the CHANGELOG.
* drop support for Node < 4.0 to enable usage of new tools and packages.
* **conventional-changelog-standard:** 

### Features

* add --lerna-package flag used to extract tags in case of lerna repo ([#503](https://github.com/Cap-go/standard-version/issues/503)) ([f579ff0](https://github.com/Cap-go/standard-version/commit/f579ff08f386aaae022a395ed0dbec9af77a5d49))
* add --sign flag to sign git commit and tag ([#29](https://github.com/Cap-go/standard-version/issues/29)) ([de758bc](https://github.com/Cap-go/standard-version/commit/de758bcda0e898d28b4c2539c7cf436bb2ff9116))
* add .cjs config file ([#717](https://github.com/Cap-go/standard-version/issues/717)) ([eceaedf](https://github.com/Cap-go/standard-version/commit/eceaedf8b3cdeb282ee06bfa9c65503f42404858))
* add a --no-verify option to prevent git hooks from being verified ([#44](https://github.com/Cap-go/standard-version/issues/44)) ([026d844](https://github.com/Cap-go/standard-version/commit/026d84493de34b8bbe556bf177c51e1623c605ad))
* add dry-run mode ([#187](https://github.com/Cap-go/standard-version/issues/187)) ([d073353](https://github.com/Cap-go/standard-version/commit/d07335353ff78d01baa5a01dfde345ad4e4cad03))
* add prebump, postbump, precommit, lifecycle scripts ([#186](https://github.com/Cap-go/standard-version/issues/186)) ([dfd1d12](https://github.com/Cap-go/standard-version/commit/dfd1d12939d8e8a53efe4a012faeaa797219cd49))
* add prerelease lifecycle script hook (closes [#217](https://github.com/Cap-go/standard-version/issues/217)) ([#234](https://github.com/Cap-go/standard-version/issues/234)) ([ba4e7f6](https://github.com/Cap-go/standard-version/commit/ba4e7f61204a91a07f9257eed3913c20edc7fbf5))
* add support for `npm-shrinkwrap.json` ([#185](https://github.com/Cap-go/standard-version/issues/185)) ([86af7fc](https://github.com/Cap-go/standard-version/commit/86af7fcc5a35a50cacc00f39d7f1fa1989172139))
* add support for `package-lock.json` ([#190](https://github.com/Cap-go/standard-version/issues/190)) ([bc0fc53](https://github.com/Cap-go/standard-version/commit/bc0fc533d8ee2dd288ed54ead70646e94ea5d847))
* add support for bumping version # in bower.json ([#148](https://github.com/Cap-go/standard-version/issues/148)) ([b788c5f](https://github.com/Cap-go/standard-version/commit/b788c5fcfb480e6df6f8384f470e881b4ea88986))
* add support for skipping lifecycle steps, polish lifecycle work ([#188](https://github.com/Cap-go/standard-version/issues/188)) ([d31dcdb](https://github.com/Cap-go/standard-version/commit/d31dcdbd77071f11d9d7603ec8cc901aa2cfbf2b))
* added support for commitAll option in CLI ([#121](https://github.com/Cap-go/standard-version/issues/121)) ([a903f4d](https://github.com/Cap-go/standard-version/commit/a903f4d66caa8f5f334a85c1f21dce8a8d74ca48))
* adds configurable conventionalcommits preset ([#323](https://github.com/Cap-go/standard-version/issues/323)) ([4fcd4a7](https://github.com/Cap-go/standard-version/commit/4fcd4a7edabbfe4183fbaa7fcd0f55b2441449d1))
* Adds support for `header` (--header) configuration based on the spec. ([#364](https://github.com/Cap-go/standard-version/issues/364)) ([ba80a0c](https://github.com/Cap-go/standard-version/commit/ba80a0c27029f54c751fe845560504925b45eab8))
* adds support for bumping for composer versions ([#262](https://github.com/Cap-go/standard-version/issues/262)) ([fee872f](https://github.com/Cap-go/standard-version/commit/fee872f4e44a6f975ce93b2d670a671bcdf542a2))
* adds support for GitHub links (see [#13](https://github.com/Cap-go/standard-version/issues/13)), great idea [@bcoe](https://github.com/bcoe)! ([7bf6597](https://github.com/Cap-go/standard-version/commit/7bf6597e60f191192d65b5ed4b3ee8d50d83f7c5))
* allow a user to provide a custom changelog header ([#335](https://github.com/Cap-go/standard-version/issues/335)) ([1c51064](https://github.com/Cap-go/standard-version/commit/1c5106477a052f224771b0a61405d279b611608c))
* allow a version # to be provided for release-as, rather than just major, minor, patch. ([13eb9cd](https://github.com/Cap-go/standard-version/commit/13eb9cd47d780f90938c1c447a31149d2f02baea))
* allows seperate prefixTag version sequences ([#573](https://github.com/Cap-go/standard-version/issues/573)) ([3bbba02](https://github.com/Cap-go/standard-version/commit/3bbba025057ba40c3e15880fede2af851841165b))
* bump minor rather than major, if release is &lt; 1.0.0 ([#347](https://github.com/Cap-go/standard-version/issues/347)) ([5d972cf](https://github.com/Cap-go/standard-version/commit/5d972cf1fede448001e30283e3258d07bed41658))
* **changelogStream:** use more default opts ([#67](https://github.com/Cap-go/standard-version/issues/67)) ([3e0aa84](https://github.com/Cap-go/standard-version/commit/3e0aa84fe5fe4ee55cac51f4e9c4033eaaeeae6e))
* cli application accept path/preset option ([#279](https://github.com/Cap-go/standard-version/issues/279)) ([69c62cf](https://github.com/Cap-go/standard-version/commit/69c62cfbddea7ce5e9b307f5167e20aee63a87da))
* **cli:** print error and don't run with node &lt;4, closes [#124](https://github.com/Cap-go/standard-version/issues/124) ([d0d71a5](https://github.com/Cap-go/standard-version/commit/d0d71a54f6769c6945e4c6e8f5aee9f3e59b29e2))
* **cli:** use conventional default commit message with version ([9fadc5f](https://github.com/Cap-go/standard-version/commit/9fadc5f9253f94e227dc6fda6f0a9bca7c3258e4))
* **configuration:** .versionrc.js files are now supported ([#378](https://github.com/Cap-go/standard-version/issues/378)) ([ddc5c00](https://github.com/Cap-go/standard-version/commit/ddc5c0016271a7595df1a1cd9c6ea1c414b18139))
* **conventional-changelog-standard:** feat(conventional-changelog-standard):  ([c7ccadb](https://github.com/Cap-go/standard-version/commit/c7ccadba80bab7a46aa50f518f22605a8ddc7be1))
* custom 'bumpFiles' and 'packageFiles' support ([#372](https://github.com/Cap-go/standard-version/issues/372)) ([564d948](https://github.com/Cap-go/standard-version/commit/564d9482a459d5d7a2020c2972b4d39167ded4bf))
* **deprecated:** add deprecation message ([#907](https://github.com/Cap-go/standard-version/issues/907)) ([61b41fa](https://github.com/Cap-go/standard-version/commit/61b41fa47ef690f55b92e2edb82fe554e3c1e13a))
* do not update/commit files in .gitignore ([#230](https://github.com/Cap-go/standard-version/issues/230)) ([4fd3bc2](https://github.com/Cap-go/standard-version/commit/4fd3bc21d5127e438c17f751b64714e84ff4f80d))
* fallback to tags if no meta-information file found ([#275](https://github.com/Cap-go/standard-version/issues/275)) ([844cde6](https://github.com/Cap-go/standard-version/commit/844cde69658c59051183aa86c6dd85a5c059e55c))
* **format-commit-message:** support multiple %s in the message ([45fcad5](https://github.com/Cap-go/standard-version/commit/45fcad547e9034d55b257bbd362054847eac41cd))
* **index.js:** add checkpoint for publish script after tag successfully ([#47](https://github.com/Cap-go/standard-version/issues/47)) ([e414ed7](https://github.com/Cap-go/standard-version/commit/e414ed7d5e889d1af256b065fe5619e4a16b6a6f))
* **initial-release:** adds flag for generating CHANGELOG.md on the first release. ([b812b44](https://github.com/Cap-go/standard-version/commit/b812b44958b3d7ed96406fbb90d427bd1770777b))
* make tag prefix configurable ([#143](https://github.com/Cap-go/standard-version/issues/143)) ([70b20c8](https://github.com/Cap-go/standard-version/commit/70b20c8793e63483eb76e95c6495f03b8dd3dd89))
* manifest.json support ([#236](https://github.com/Cap-go/standard-version/issues/236)) ([371d992](https://github.com/Cap-go/standard-version/commit/371d99290164cf16dd0aa26d094215d49688f54f))
* **options:** add --silent flag and option for squelching output ([2a3fa61](https://github.com/Cap-go/standard-version/commit/2a3fa6167bd84466485d7d7c3ea2e3a62e41a0ff))
* preserve formatting when writing to package.json ([#282](https://github.com/Cap-go/standard-version/issues/282)) ([96216da](https://github.com/Cap-go/standard-version/commit/96216da5f7a9a8cb02b67d9478a1f20e513f9859))
* publish only if commit+push succeed ([#229](https://github.com/Cap-go/standard-version/issues/229)) ([c5e1ee2](https://github.com/Cap-go/standard-version/commit/c5e1ee2a63a3488484f5392a5180cf97026f948d))
* **rebrand:** rebrand recommended-workflow to standard-version ([#9](https://github.com/Cap-go/standard-version/issues/9)) ([1f673c0](https://github.com/Cap-go/standard-version/commit/1f673c002e89b162ff074c9c6fb057f9c3dddea6))
* separate cli and defaults from base functionality ([34a6a4e](https://github.com/Cap-go/standard-version/commit/34a6a4ea23c1f56d923a8bbe004bf57fecc6badd))
* suggest branch name other than master ([#331](https://github.com/Cap-go/standard-version/issues/331)) ([304b49a](https://github.com/Cap-go/standard-version/commit/304b49a7ffdf3adf8fc3e3234e11455b05062c2a))
* support custom updater as object as well as path ([#630](https://github.com/Cap-go/standard-version/issues/630)) ([55bbde8](https://github.com/Cap-go/standard-version/commit/55bbde8476013de7a2f24bf29c7c12cb07f96e3f))
* support releasing a custom version, including pre-releases ([#129](https://github.com/Cap-go/standard-version/issues/129)) ([068008d](https://github.com/Cap-go/standard-version/commit/068008d6a568033f4ace85dea8911031b3dc96ca))
* **tests:** adds test suite, fixed several Node 0.10 issues along the way ([03bd86c](https://github.com/Cap-go/standard-version/commit/03bd86c467421ebcc20bae3c262757dbaa62e82f))
* update commit msg for when using commitAll ([#320](https://github.com/Cap-go/standard-version/issues/320)) ([74a040a](https://github.com/Cap-go/standard-version/commit/74a040a517e489111709c5acd7826543ad814af0))


### Bug Fixes

* adds support for `releaseCommitMessageFormat` ([#351](https://github.com/Cap-go/standard-version/issues/351)) ([a7133cc](https://github.com/Cap-go/standard-version/commit/a7133cc0e5a1924793bdf0e4abdd0ad9c58dfc2d))
* always pass version to changelog context ([#327](https://github.com/Cap-go/standard-version/issues/327)) ([00e3381](https://github.com/Cap-go/standard-version/commit/00e338159e2158b23a58a4da9e95c5f5075257aa))
* append line feed to end of package.json ([#42](https://github.com/Cap-go/standard-version/issues/42)) ([178e001](https://github.com/Cap-go/standard-version/commit/178e00196af696c4bab3dec62df38b658aa7b543))
* bin now enforces Node.js &gt; 4 ([#274](https://github.com/Cap-go/standard-version/issues/274)) ([e1b5780](https://github.com/Cap-go/standard-version/commit/e1b57809ef8c65ef50205bc81348098cfd514606))
* **bump:** transmit tag prefix argument to conventionalRecommendedBump ([#393](https://github.com/Cap-go/standard-version/issues/393)) ([8205222](https://github.com/Cap-go/standard-version/commit/8205222150e0451dc4e20d0beef33802b873467a))
* check the private field in package.json([#102](https://github.com/Cap-go/standard-version/issues/102)) ([#103](https://github.com/Cap-go/standard-version/issues/103)) ([2ce4160](https://github.com/Cap-go/standard-version/commit/2ce4160fcf4cb2c7b9338adf9d800c9d68128b21))
* **cli:** display only one, correct default for --preset flag ([#377](https://github.com/Cap-go/standard-version/issues/377)) ([d17fc81](https://github.com/Cap-go/standard-version/commit/d17fc8103ac37887456483c29ef28f6ccd2519d1))
* Commit message and tag name is no longer enclosed in quotes. ([#619](https://github.com/Cap-go/standard-version/issues/619)) ([ae032bf](https://github.com/Cap-go/standard-version/commit/ae032bfa9268a0a14351b0d78b6deedee7891e3a))
* **commit:** don't try to process and add changelog if skipped ([#318](https://github.com/Cap-go/standard-version/issues/318)) ([3e4fdec](https://github.com/Cap-go/standard-version/commit/3e4fdecdb8e30b3e59c8682be64b7c18d3ff4175))
* **commit:** fix windows by separating add and commit exec ([#55](https://github.com/Cap-go/standard-version/issues/55)) ([f361c46](https://github.com/Cap-go/standard-version/commit/f361c465f87078467b597804a5d5b1a937ccc3c3)), closes [#49](https://github.com/Cap-go/standard-version/issues/49)
* composer.json and composer.lock have been removed from default package and bump files. ([c934f3a](https://github.com/Cap-go/standard-version/commit/c934f3a38da4e7234d9dba3b2405f3b7e4dc5aa8))
* **deps:** update dependency conventional-changelog to v3.1.12 ([#463](https://github.com/Cap-go/standard-version/issues/463)) ([f04161a](https://github.com/Cap-go/standard-version/commit/f04161ae624705e68f9018d563e9f3c09ccf6f30))
* **deps:** update dependency conventional-changelog to v3.1.15 ([#479](https://github.com/Cap-go/standard-version/issues/479)) ([492e721](https://github.com/Cap-go/standard-version/commit/492e72192ebf35d7c58c00526b1e6bd2abac7f13))
* **deps:** update dependency conventional-changelog to v3.1.18 ([#510](https://github.com/Cap-go/standard-version/issues/510)) ([e6aeb77](https://github.com/Cap-go/standard-version/commit/e6aeb779fe53ffed2a252e6cfd69cfcb786b9ef9))
* **deps:** update dependency conventional-changelog to v3.1.21 ([#586](https://github.com/Cap-go/standard-version/issues/586)) ([fd456c9](https://github.com/Cap-go/standard-version/commit/fd456c995f3f88497fbb912fb8aabb8a42d97dbb))
* **deps:** update dependency conventional-changelog to v3.1.23 ([#652](https://github.com/Cap-go/standard-version/issues/652)) ([00dd3c0](https://github.com/Cap-go/standard-version/commit/00dd3c01aab20d28a8bbd1e174e416d6c2b34d90))
* **deps:** update dependency conventional-changelog to v3.1.24 ([#677](https://github.com/Cap-go/standard-version/issues/677)) ([cc45036](https://github.com/Cap-go/standard-version/commit/cc45036d9960b6d83e0e850ccbbe8e8098d36ae6))
* **deps:** update dependency conventional-changelog to v3.1.25 ([#865](https://github.com/Cap-go/standard-version/issues/865)) ([4c938a2](https://github.com/Cap-go/standard-version/commit/4c938a2baac11385d655144429bc73b2199bb027))
* **deps:** update dependency conventional-changelog-config-spec to v2 ([#352](https://github.com/Cap-go/standard-version/issues/352)) ([f586844](https://github.com/Cap-go/standard-version/commit/f586844d7952937a3d13f6974c84b73b3354f743))
* **deps:** update dependency conventional-changelog-config-spec to v2.1.0 ([#442](https://github.com/Cap-go/standard-version/issues/442)) ([a2c5747](https://github.com/Cap-go/standard-version/commit/a2c574735ac5a165a190661b7735ea284bdc7dda))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.2.3 ([#496](https://github.com/Cap-go/standard-version/issues/496)) ([bc606f8](https://github.com/Cap-go/standard-version/commit/bc606f8e96bcef1d46b28305622fc76dfbf306cf))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.3.0 ([#587](https://github.com/Cap-go/standard-version/issues/587)) ([b3b5eed](https://github.com/Cap-go/standard-version/commit/b3b5eedea3eaf062d74d1004a55a0a6b1e3ca6c6))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.4.0 ([#650](https://github.com/Cap-go/standard-version/issues/650)) ([9f201a6](https://github.com/Cap-go/standard-version/commit/9f201a61bb50ec12053a04faccfaea20e44d6ff2))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.5.0 ([#678](https://github.com/Cap-go/standard-version/issues/678)) ([6317d36](https://github.com/Cap-go/standard-version/commit/6317d36130767cfd85114ab9033a6f1ef110388d))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.6.1 ([#752](https://github.com/Cap-go/standard-version/issues/752)) ([bb8869d](https://github.com/Cap-go/standard-version/commit/bb8869de7d8bcace1ec92f29e389e7fab506d64e))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.6.3 ([#866](https://github.com/Cap-go/standard-version/issues/866)) ([6c75ed0](https://github.com/Cap-go/standard-version/commit/6c75ed0b1456913ae7e4d6fe8532fb4106df1bdf))
* **deps:** update dependency conventional-recommended-bump to v6 ([#417](https://github.com/Cap-go/standard-version/issues/417)) ([4c5cad1](https://github.com/Cap-go/standard-version/commit/4c5cad133aa30de941e9a6bd9120644fd3bdecc2))
* **deps:** update dependency conventional-recommended-bump to v6.0.10 ([#653](https://github.com/Cap-go/standard-version/issues/653)) ([c360d6a](https://github.com/Cap-go/standard-version/commit/c360d6a307909c6e571b29d4a329fd786b4d4543))
* **deps:** update dependency conventional-recommended-bump to v6.0.11 ([#679](https://github.com/Cap-go/standard-version/issues/679)) ([360789a](https://github.com/Cap-go/standard-version/commit/360789ab84957a67d3919cb28db1882cb68296fc))
* **deps:** update dependency conventional-recommended-bump to v6.0.2 ([#462](https://github.com/Cap-go/standard-version/issues/462)) ([84bb581](https://github.com/Cap-go/standard-version/commit/84bb581209b50357761cbec45bb8253f6a182801))
* **deps:** update dependency conventional-recommended-bump to v6.0.5 ([#480](https://github.com/Cap-go/standard-version/issues/480)) ([1e1e215](https://github.com/Cap-go/standard-version/commit/1e1e215a633963188cdb02be1316b5506e3b99b7))
* **deps:** update dependency conventional-recommended-bump to v6.0.9 ([#588](https://github.com/Cap-go/standard-version/issues/588)) ([d4d2ac2](https://github.com/Cap-go/standard-version/commit/d4d2ac2a99c095227118da795e1c9e19d06c9a0a))
* **deps:** update dependency conventional-recommended-bump to v6.1.0 ([#695](https://github.com/Cap-go/standard-version/issues/695)) ([65dd070](https://github.com/Cap-go/standard-version/commit/65dd070b9f01ffe1764e64ba739bc064b84f4129))
* **deps:** update dependency detect-indent to v6 ([#341](https://github.com/Cap-go/standard-version/issues/341)) ([234d9dd](https://github.com/Cap-go/standard-version/commit/234d9dde80eb1e99795631e65ee27cd3302a6133))
* **deps:** update dependency detect-newline to v3 ([#342](https://github.com/Cap-go/standard-version/issues/342)) ([02a6093](https://github.com/Cap-go/standard-version/commit/02a609395ca4d26b7cc966552a6e2405359893b6))
* **deps:** update dependency detect-newline to v3.1.0 ([#482](https://github.com/Cap-go/standard-version/issues/482)) ([04ab36a](https://github.com/Cap-go/standard-version/commit/04ab36a12be58915cfa9c60771890e074d1f5685))
* **deps:** update dependency figures to v3 ([#343](https://github.com/Cap-go/standard-version/issues/343)) ([7208ded](https://github.com/Cap-go/standard-version/commit/7208dedeb2b701fdcb9c59ec5f2b4872306108a2))
* **deps:** update dependency figures to v3.1.0 ([#468](https://github.com/Cap-go/standard-version/issues/468)) ([63300a9](https://github.com/Cap-go/standard-version/commit/63300a935c0079fd03e8e1acc55fd5b1dcea677f))
* **deps:** update dependency find-up to v4 ([#355](https://github.com/Cap-go/standard-version/issues/355)) ([73b35f8](https://github.com/Cap-go/standard-version/commit/73b35f8c9086209109d3a5cee79a9c48b6da7ba0))
* **deps:** update dependency find-up to v4.1.0 ([#383](https://github.com/Cap-go/standard-version/issues/383)) ([b621a4a](https://github.com/Cap-go/standard-version/commit/b621a4a448244715926d9a05b2486632ee16bafb))
* **deps:** update dependency find-up to v5 ([#651](https://github.com/Cap-go/standard-version/issues/651)) ([df8db83](https://github.com/Cap-go/standard-version/commit/df8db832327a751d5c62fe361b6ac2d2b5f66bf6))
* **deps:** update dependency git-semver-tags to v3 ([#418](https://github.com/Cap-go/standard-version/issues/418)) ([1ce3f4a](https://github.com/Cap-go/standard-version/commit/1ce3f4afa9bc2520e50982773cbf4b041cdc157f))
* **deps:** update dependency git-semver-tags to v3.0.1 ([#485](https://github.com/Cap-go/standard-version/issues/485)) ([9cc188c](https://github.com/Cap-go/standard-version/commit/9cc188cbb84ee3ae80d5e66f5c54727877313b14))
* **deps:** update dependency git-semver-tags to v4 ([#589](https://github.com/Cap-go/standard-version/issues/589)) ([a0f0e81](https://github.com/Cap-go/standard-version/commit/a0f0e813b2be4a2065600a19075fda4d6f331ef8))
* **deps:** update dependency semver to v6 ([#344](https://github.com/Cap-go/standard-version/issues/344)) ([c40487a](https://github.com/Cap-go/standard-version/commit/c40487a4100b5d3f85fae2eeb1cbff91056cd11d))
* **deps:** update dependency semver to v6.3.0 ([#366](https://github.com/Cap-go/standard-version/issues/366)) ([cd866c7](https://github.com/Cap-go/standard-version/commit/cd866c7ae6818fa7f19e61e0bbb10db90036e9b7))
* **deps:** update dependency stringify-package to v1.0.1 ([#459](https://github.com/Cap-go/standard-version/issues/459)) ([e06a835](https://github.com/Cap-go/standard-version/commit/e06a835c8296a92f4fa7c07f98057d765c1a91e5))
* **deps:** update dependency yargs to v13 ([#345](https://github.com/Cap-go/standard-version/issues/345)) ([b2c8e59](https://github.com/Cap-go/standard-version/commit/b2c8e59087b3aac957b8c1f79fa1087764f9811b))
* **deps:** update dependency yargs to v13.2.4 ([#356](https://github.com/Cap-go/standard-version/issues/356)) ([00b2ce6](https://github.com/Cap-go/standard-version/commit/00b2ce6d7af33a66ff3bfc5f76cdf1d43ce934b3))
* **deps:** update dependency yargs to v13.3.0 ([#401](https://github.com/Cap-go/standard-version/issues/401)) ([3d0e8c7](https://github.com/Cap-go/standard-version/commit/3d0e8c7e33dc51d13aea43ee0fdb915f1961fcc8))
* **deps:** update dependency yargs to v14 ([#440](https://github.com/Cap-go/standard-version/issues/440)) ([fe37e73](https://github.com/Cap-go/standard-version/commit/fe37e7390760d8d16d1b94ca58d8123e292c46a8))
* **deps:** update dependency yargs to v14.2.0 ([#461](https://github.com/Cap-go/standard-version/issues/461)) ([fb21851](https://github.com/Cap-go/standard-version/commit/fb2185107a90ba4b9dc7c9c1d873ed1283706ac1))
* **deps:** update dependency yargs to v14.2.1 ([#483](https://github.com/Cap-go/standard-version/issues/483)) ([dc1fa61](https://github.com/Cap-go/standard-version/commit/dc1fa6170ffe12d4f8b44b70d23688a64d2ad0fb))
* **deps:** update dependency yargs to v14.2.2 ([#488](https://github.com/Cap-go/standard-version/issues/488)) ([ecf26b6](https://github.com/Cap-go/standard-version/commit/ecf26b6fc9421a78fb81793c4a932f579f7e9d4a))
* **deps:** update dependency yargs to v15 ([#484](https://github.com/Cap-go/standard-version/issues/484)) ([35b90c3](https://github.com/Cap-go/standard-version/commit/35b90c3f24cfb8237e94482fd20997900569193e))
* **deps:** update dependency yargs to v15.1.0 ([#518](https://github.com/Cap-go/standard-version/issues/518)) ([8f36f9e](https://github.com/Cap-go/standard-version/commit/8f36f9e073119fcbf5ad843237fb06a4ca42a0f9))
* **deps:** update dependency yargs to v15.3.1 ([#559](https://github.com/Cap-go/standard-version/issues/559)) ([d98cd46](https://github.com/Cap-go/standard-version/commit/d98cd4674b4d074c0b7f4d50d052ae618cf494c6))
* **deps:** update dependency yargs to v16 ([#660](https://github.com/Cap-go/standard-version/issues/660)) ([f6a7430](https://github.com/Cap-go/standard-version/commit/f6a7430329919874e1e744ac5dca2f83bba355df))
* **docs:** had a bad URL in package.json, which was breaking all of our links ([caa6359](https://github.com/Cap-go/standard-version/commit/caa63593efd0d6ccaf3f067b0d8fbc8051f94339))
* don't pass args to git rev-parse ([1ac72f7](https://github.com/Cap-go/standard-version/commit/1ac72f74fe447121c0096915955732f7d84b5dc3))
* Ensures provided `packageFiles` arguments are merged with `bumpFiles` when no `bumpFiles` argument is specified (default). ([#534](https://github.com/Cap-go/standard-version/issues/534)) ([2785023](https://github.com/Cap-go/standard-version/commit/2785023c91668e7300e6a22e55d31b6bd9dae59b)), closes [#533](https://github.com/Cap-go/standard-version/issues/533)
* **err:** don't fail on stderr output, but print the output to stderr ([#110](https://github.com/Cap-go/standard-version/issues/110)) ([f7a4915](https://github.com/Cap-go/standard-version/commit/f7a4915d26335e744066e89d734c2e6ea4b5e292))
* format the annotated tag message ([#28](https://github.com/Cap-go/standard-version/issues/28)) ([8f02736](https://github.com/Cap-go/standard-version/commit/8f0273676c7a78b69ed097e08fe6d886bfea8575))
* include merge commits in the changelog ([#139](https://github.com/Cap-go/standard-version/issues/139)) ([b6e1562](https://github.com/Cap-go/standard-version/commit/b6e1562808cdc712e157dbb1d6607f0624981f66))
* **index.js:** use blue figures.info for last checkpoint ([#64](https://github.com/Cap-go/standard-version/issues/64)) ([e600b42](https://github.com/Cap-go/standard-version/commit/e600b42968456ae96ab6af9965758ea93b1c0181))
* issue already load updater ([a5ff597](https://github.com/Cap-go/standard-version/commit/a5ff597894ef3c7c4323119281caf8066b1e7c3a))
* make pattern for finding CHANGELOG sections work for non anchors ([#292](https://github.com/Cap-go/standard-version/issues/292)) ([b684c78](https://github.com/Cap-go/standard-version/commit/b684c784c8986226889feb1524bc029b913c9571))
* no --tag prerelease for private module ([#296](https://github.com/Cap-go/standard-version/issues/296)) ([27e2ab4](https://github.com/Cap-go/standard-version/commit/27e2ab422c94c633affa652c07bb04d49484f04e)), closes [#294](https://github.com/Cap-go/standard-version/issues/294)
* package name ([cda4717](https://github.com/Cap-go/standard-version/commit/cda47172224b726aa0e591f1ac8969089293a46a))
* prevent duplicate headers from being added ([#305](https://github.com/Cap-go/standard-version/issues/305)) ([#307](https://github.com/Cap-go/standard-version/issues/307)) ([db2c6e5](https://github.com/Cap-go/standard-version/commit/db2c6e5459a01f005c09e39900bae0ff93400534))
* recommend `--tag` prerelease for npm publish of prereleases ([#196](https://github.com/Cap-go/standard-version/issues/196)) ([709dae1](https://github.com/Cap-go/standard-version/commit/709dae168069930e38b18d8ed0fb07addc9540b6)), closes [#183](https://github.com/Cap-go/standard-version/issues/183)
* renovate ([1ef186f](https://github.com/Cap-go/standard-version/commit/1ef186fd414469267c6f1ab7943950070454c152))
* run CI on more recent ([564c22e](https://github.com/Cap-go/standard-version/commit/564c22e193daf6e5d00f1e55fb3d41461128eb0f))
* should print message before we bump version ([2894bbc](https://github.com/Cap-go/standard-version/commit/2894bbc6998e7723eb658debe2a00e707cb3116a))
* show correct pre-release tag in help output ([#259](https://github.com/Cap-go/standard-version/issues/259)) ([d90154a](https://github.com/Cap-go/standard-version/commit/d90154a82b78d4ede26cf043c1d04ff9da2ad35c))
* show full tag name in checkpoint ([#241](https://github.com/Cap-go/standard-version/issues/241)) ([b4ed4f9](https://github.com/Cap-go/standard-version/commit/b4ed4f9ba9a905c4d36804f6e42e07d510499543))
* stop suggesting npm publish if package.json was not updated ([#319](https://github.com/Cap-go/standard-version/issues/319)) ([a5ac845](https://github.com/Cap-go/standard-version/commit/a5ac84545a51ce8eb5ea2db0cf06fb8b39188e82))
* support a wording change made to git status in git v2.9.1 ([#140](https://github.com/Cap-go/standard-version/issues/140)) ([80004ec](https://github.com/Cap-go/standard-version/commit/80004ec1d6b927354358d9998e6058cb51b4565b))
* update config file name in command based on README.md ([#357](https://github.com/Cap-go/standard-version/issues/357)) ([ce44dd2](https://github.com/Cap-go/standard-version/commit/ce44dd26deb6d6b0335cd6be2995bf7d2cc8d72a))
* update readme ([5ef14e2](https://github.com/Cap-go/standard-version/commit/5ef14e23e97d694455dd54a0864d5df0eba1dcc2))
* **updater:** npm7 package lock's inner version not being updated ([#713](https://github.com/Cap-go/standard-version/issues/713)) ([a316dd0](https://github.com/Cap-go/standard-version/commit/a316dd02f5a7d8dee33d99370afda8738985bc10))
* Updates package.json to _actual_ supported (tested) NodeJS versions. ([#379](https://github.com/Cap-go/standard-version/issues/379)) ([15eec8a](https://github.com/Cap-go/standard-version/commit/15eec8a1143dbd99e6d1b80a856cd4859fa13480))
* upgrade to version of nyc that works with new shelljs ([c7ac6e2](https://github.com/Cap-go/standard-version/commit/c7ac6e298ecb3a9e757fbe502cb6078df350780f))
* upgraded dependencies, switched back to angular format (fixes [#27](https://github.com/Cap-go/standard-version/issues/27)), pinned shelljs to version that works with nyc ([#30](https://github.com/Cap-go/standard-version/issues/30)) ([3f51e94](https://github.com/Cap-go/standard-version/commit/3f51e9438fb5ff7f68278d1993c34b9d95c1638c))
* use require.resolve for the default preset ([#465](https://github.com/Cap-go/standard-version/issues/465)) ([d557372](https://github.com/Cap-go/standard-version/commit/d55737239530f5eee684e9cbf959f7238d609fd4))
* use tagPrefix in CHANGELOG lifecycle step ([#243](https://github.com/Cap-go/standard-version/issues/243)) ([a56c7ac](https://github.com/Cap-go/standard-version/commit/a56c7ac78f9d7f6b4fb043d135b5e3d9ada89c70))
* use the `skip` default value for skip cli arg ([#211](https://github.com/Cap-go/standard-version/issues/211)) ([3fdd7fa](https://github.com/Cap-go/standard-version/commit/3fdd7fa22fa40f2e9f899aac24493f391e72a074))
* Vulnerability Report GHSL-2020-11101 ([9d978ac](https://github.com/Cap-go/standard-version/commit/9d978ac9d4f64be4c7b9d514712ab3757732d561))
* we had too many \n characters ([#17](https://github.com/Cap-go/standard-version/issues/17)) ([67a01cd](https://github.com/Cap-go/standard-version/commit/67a01cd78217acb74eed75b8c9441f6595142cdb))


### Reverts

* "chore(deps): bump conventional-changelog to v3.1.17" ([00512d0](https://github.com/Cap-go/standard-version/commit/00512d08eb3197d7b20a2f09894ed1a6ae4af272))


### Miscellaneous Chores

* package.json engines field &gt;=4.0, drop Node 0.10 and 0.12 ([28ff65a](https://github.com/Cap-go/standard-version/commit/28ff65a69cee682db05f899aafae8c2b6f1e4ccb))
* update testing matrix ([1d46627](https://github.com/Cap-go/standard-version/commit/1d466275518ae2649758b9e0e9b3c848734f534f))


### Build System

* drop Node 6 from testing matrix ([#346](https://github.com/Cap-go/standard-version/issues/346)) ([6718428](https://github.com/Cap-go/standard-version/commit/671842853b9fa62ecda126bf5e1fbe7aa60a5d1f))
* NodeJS@8 is no longer supported. ([#612](https://github.com/Cap-go/standard-version/issues/612)) ([05edef2](https://github.com/Cap-go/standard-version/commit/05edef2de79d8d4939a6e699ce0979ff8da12de9))

## [9.5.0](https://github.com/conventional-changelog/standard-version/compare/v9.4.0...v9.5.0) (2022-05-15)


### Features

* **deprecated:** add deprecation message ([#907](https://github.com/conventional-changelog/standard-version/issues/907)) ([61b41fa](https://github.com/conventional-changelog/standard-version/commit/61b41fa47ef690f55b92e2edb82fe554e3c1e13a))


### Bug Fixes

* **deps:** update dependency conventional-changelog to v3.1.25 ([#865](https://github.com/conventional-changelog/standard-version/issues/865)) ([4c938a2](https://github.com/conventional-changelog/standard-version/commit/4c938a2baac11385d655144429bc73b2199bb027))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.6.3 ([#866](https://github.com/conventional-changelog/standard-version/issues/866)) ([6c75ed0](https://github.com/conventional-changelog/standard-version/commit/6c75ed0b1456913ae7e4d6fe8532fb4106df1bdf))

## [9.4.0](https://github.com/conventional-changelog/standard-version/compare/v9.3.2...v9.4.0) (2021-12-31)


### Features

* add .cjs config file ([#717](https://github.com/conventional-changelog/standard-version/issues/717)) ([eceaedf](https://github.com/conventional-changelog/standard-version/commit/eceaedf8b3cdeb282ee06bfa9c65503f42404858))


### Bug Fixes

* Ensures provided `packageFiles` arguments are merged with `bumpFiles` when no `bumpFiles` argument is specified (default). ([#534](https://github.com/conventional-changelog/standard-version/issues/534)) ([2785023](https://github.com/conventional-changelog/standard-version/commit/2785023c91668e7300e6a22e55d31b6bd9dae59b)), closes [#533](https://github.com/conventional-changelog/standard-version/issues/533)

### [9.3.2](https://www.github.com/conventional-changelog/standard-version/compare/v9.3.1...v9.3.2) (2021-10-17)


### Bug Fixes

* **deps:** update dependency conventional-changelog-conventionalcommits to v4.6.1 ([#752](https://www.github.com/conventional-changelog/standard-version/issues/752)) ([bb8869d](https://www.github.com/conventional-changelog/standard-version/commit/bb8869de7d8bcace1ec92f29e389e7fab506d64e))

### [9.3.1](https://www.github.com/conventional-changelog/standard-version/compare/v9.3.0...v9.3.1) (2021-07-14)


### Bug Fixes

* **updater:** npm7 package lock's inner version not being updated ([#713](https://www.github.com/conventional-changelog/standard-version/issues/713)) ([a316dd0](https://www.github.com/conventional-changelog/standard-version/commit/a316dd02f5a7d8dee33d99370afda8738985bc10))

## [9.3.0](https://www.github.com/conventional-changelog/standard-version/compare/v9.2.0...v9.3.0) (2021-05-04)


### Features

* add --lerna-package flag used to extract tags in case of lerna repo ([#503](https://www.github.com/conventional-changelog/standard-version/issues/503)) ([f579ff0](https://www.github.com/conventional-changelog/standard-version/commit/f579ff08f386aaae022a395ed0dbec9af77a5d49))

## [9.2.0](https://www.github.com/conventional-changelog/standard-version/compare/v9.1.1...v9.2.0) (2021-04-06)


### Features

* allows seperate prefixTag version sequences ([#573](https://www.github.com/conventional-changelog/standard-version/issues/573)) ([3bbba02](https://www.github.com/conventional-changelog/standard-version/commit/3bbba025057ba40c3e15880fede2af851841165b))

### [9.1.1](https://www.github.com/conventional-changelog/standard-version/compare/v9.1.0...v9.1.1) (2021-02-06)


### Bug Fixes

* **deps:** update dependency conventional-recommended-bump to v6.1.0 ([#695](https://www.github.com/conventional-changelog/standard-version/issues/695)) ([65dd070](https://www.github.com/conventional-changelog/standard-version/commit/65dd070b9f01ffe1764e64ba739bc064b84f4129))
* **deps:** update dependency yargs to v16 ([#660](https://www.github.com/conventional-changelog/standard-version/issues/660)) ([f6a7430](https://www.github.com/conventional-changelog/standard-version/commit/f6a7430329919874e1e744ac5dca2f83bba355df))

## [9.1.0](https://www.github.com/conventional-changelog/standard-version/compare/v9.0.0...v9.1.0) (2020-12-01)


### Features

* support custom updater as object as well as path ([#630](https://www.github.com/conventional-changelog/standard-version/issues/630)) ([55bbde8](https://www.github.com/conventional-changelog/standard-version/commit/55bbde8476013de7a2f24bf29c7c12cb07f96e3f))


### Bug Fixes

* **deps:** update dependency conventional-changelog to v3.1.24 ([#677](https://www.github.com/conventional-changelog/standard-version/issues/677)) ([cc45036](https://www.github.com/conventional-changelog/standard-version/commit/cc45036d9960b6d83e0e850ccbbe8e8098d36ae6))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.5.0 ([#678](https://www.github.com/conventional-changelog/standard-version/issues/678)) ([6317d36](https://www.github.com/conventional-changelog/standard-version/commit/6317d36130767cfd85114ab9033a6f1ef110388d))
* **deps:** update dependency conventional-recommended-bump to v6.0.11 ([#679](https://www.github.com/conventional-changelog/standard-version/issues/679)) ([360789a](https://www.github.com/conventional-changelog/standard-version/commit/360789ab84957a67d3919cb28db1882cb68296fc))
* **deps:** update dependency find-up to v5 ([#651](https://www.github.com/conventional-changelog/standard-version/issues/651)) ([df8db83](https://www.github.com/conventional-changelog/standard-version/commit/df8db832327a751d5c62fe361b6ac2d2b5f66bf6))

## [9.0.0](https://www.github.com/conventional-changelog/standard-version/compare/v8.0.2...v9.0.0) (2020-08-15)


### ⚠ BREAKING CHANGES

* NodeJS@8 is no longer supported. (#612)

### Bug Fixes

* **deps:** update dependency conventional-changelog to v3.1.23 ([#652](https://www.github.com/conventional-changelog/standard-version/issues/652)) ([00dd3c0](https://www.github.com/conventional-changelog/standard-version/commit/00dd3c01aab20d28a8bbd1e174e416d6c2b34d90))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.4.0 ([#650](https://www.github.com/conventional-changelog/standard-version/issues/650)) ([9f201a6](https://www.github.com/conventional-changelog/standard-version/commit/9f201a61bb50ec12053a04faccfaea20e44d6ff2))
* **deps:** update dependency conventional-recommended-bump to v6.0.10 ([#653](https://www.github.com/conventional-changelog/standard-version/issues/653)) ([c360d6a](https://www.github.com/conventional-changelog/standard-version/commit/c360d6a307909c6e571b29d4a329fd786b4d4543))


### Build System

* NodeJS@8 is no longer supported. ([#612](https://www.github.com/conventional-changelog/standard-version/issues/612)) ([05edef2](https://www.github.com/conventional-changelog/standard-version/commit/05edef2de79d8d4939a6e699ce0979ff8da12de9))

### [8.0.2](https://www.github.com/conventional-changelog/standard-version/compare/v8.0.1...v8.0.2) (2020-07-14)


### Bug Fixes

* Commit message and tag name is no longer enclosed in quotes. ([#619](https://www.github.com/conventional-changelog/standard-version/issues/619)) ([ae032bf](https://www.github.com/conventional-changelog/standard-version/commit/ae032bfa9268a0a14351b0d78b6deedee7891e3a)), closes [#621](https://www.github.com/conventional-changelog/standard-version/issues/621) [#620](https://www.github.com/conventional-changelog/standard-version/issues/620)

### [8.0.1](https://www.github.com/conventional-changelog/standard-version/compare/v8.0.0...v8.0.1) (2020-07-12)


### Bug Fixes

* **deps:** update dependency conventional-changelog to v3.1.21 ([#586](https://www.github.com/conventional-changelog/standard-version/issues/586)) ([fd456c9](https://www.github.com/conventional-changelog/standard-version/commit/fd456c995f3f88497fbb912fb8aabb8a42d97dbb))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.3.0 ([#587](https://www.github.com/conventional-changelog/standard-version/issues/587)) ([b3b5eed](https://www.github.com/conventional-changelog/standard-version/commit/b3b5eedea3eaf062d74d1004a55a0a6b1e3ca6c6))
* **deps:** update dependency conventional-recommended-bump to v6.0.9 ([#588](https://www.github.com/conventional-changelog/standard-version/issues/588)) ([d4d2ac2](https://www.github.com/conventional-changelog/standard-version/commit/d4d2ac2a99c095227118da795e1c9e19d06c9a0a))
* **deps:** update dependency git-semver-tags to v4 ([#589](https://www.github.com/conventional-changelog/standard-version/issues/589)) ([a0f0e81](https://www.github.com/conventional-changelog/standard-version/commit/a0f0e813b2be4a2065600a19075fda4d6f331ef8))
* Vulnerability Report GHSL-2020-11101 ([9d978ac](https://www.github.com/conventional-changelog/standard-version/commit/9d978ac9d4f64be4c7b9d514712ab3757732d561))

## [8.0.0](https://www.github.com/conventional-changelog/standard-version/compare/v7.1.0...v8.0.0) (2020-05-06)


### ⚠ BREAKING CHANGES

* `composer.json` and `composer.lock` will no longer be read from or bumped by default. If you need to obtain a version or write a version to these files, please use `bumpFiles` and/or `packageFiles` options accordingly.

### Bug Fixes

* composer.json and composer.lock have been removed from default package and bump files. ([c934f3a](https://www.github.com/conventional-changelog/standard-version/commit/c934f3a38da4e7234d9dba3b2405f3b7e4dc5aa8)), closes [#495](https://www.github.com/conventional-changelog/standard-version/issues/495) [#394](https://www.github.com/conventional-changelog/standard-version/issues/394)
* **deps:** update dependency conventional-changelog to v3.1.18 ([#510](https://www.github.com/conventional-changelog/standard-version/issues/510)) ([e6aeb77](https://www.github.com/conventional-changelog/standard-version/commit/e6aeb779fe53ffed2a252e6cfd69cfcb786b9ef9))
* **deps:** update dependency yargs to v15.1.0 ([#518](https://www.github.com/conventional-changelog/standard-version/issues/518)) ([8f36f9e](https://www.github.com/conventional-changelog/standard-version/commit/8f36f9e073119fcbf5ad843237fb06a4ca42a0f9))
* **deps:** update dependency yargs to v15.3.1 ([#559](https://www.github.com/conventional-changelog/standard-version/issues/559)) ([d98cd46](https://www.github.com/conventional-changelog/standard-version/commit/d98cd4674b4d074c0b7f4d50d052ae618cf494c6))

## [7.1.0](https://github.com/conventional-changelog/standard-version/compare/v7.0.1...v7.1.0) (2019-12-08)


### Features

* Adds support for `header` (--header) configuration based on the spec. ([#364](https://github.com/conventional-changelog/standard-version/issues/364)) ([ba80a0c](https://github.com/conventional-changelog/standard-version/commit/ba80a0c27029f54c751fe845560504925b45eab8))
* custom 'bumpFiles' and 'packageFiles' support ([#372](https://github.com/conventional-changelog/standard-version/issues/372)) ([564d948](https://github.com/conventional-changelog/standard-version/commit/564d9482a459d5d7a2020c2972b4d39167ded4bf))


### Bug Fixes

* **deps:** update dependency conventional-changelog to v3.1.15 ([#479](https://github.com/conventional-changelog/standard-version/issues/479)) ([492e721](https://github.com/conventional-changelog/standard-version/commit/492e72192ebf35d7c58c00526b1e6bd2abac7f13))
* **deps:** update dependency conventional-changelog-conventionalcommits to v4.2.3 ([#496](https://github.com/conventional-changelog/standard-version/issues/496)) ([bc606f8](https://github.com/conventional-changelog/standard-version/commit/bc606f8e96bcef1d46b28305622fc76dfbf306cf))
* **deps:** update dependency conventional-recommended-bump to v6.0.5 ([#480](https://github.com/conventional-changelog/standard-version/issues/480)) ([1e1e215](https://github.com/conventional-changelog/standard-version/commit/1e1e215a633963188cdb02be1316b5506e3b99b7))
* **deps:** update dependency yargs to v15 ([#484](https://github.com/conventional-changelog/standard-version/issues/484)) ([35b90c3](https://github.com/conventional-changelog/standard-version/commit/35b90c3f24cfb8237e94482fd20997900569193e))
* use require.resolve for the default preset ([#465](https://github.com/conventional-changelog/standard-version/issues/465)) ([d557372](https://github.com/conventional-changelog/standard-version/commit/d55737239530f5eee684e9cbf959f7238d609fd4))
* **deps:** update dependency detect-newline to v3.1.0 ([#482](https://github.com/conventional-changelog/standard-version/issues/482)) ([04ab36a](https://github.com/conventional-changelog/standard-version/commit/04ab36a12be58915cfa9c60771890e074d1f5685))
* **deps:** update dependency figures to v3.1.0 ([#468](https://github.com/conventional-changelog/standard-version/issues/468)) ([63300a9](https://github.com/conventional-changelog/standard-version/commit/63300a935c0079fd03e8e1acc55fd5b1dcea677f))
* **deps:** update dependency git-semver-tags to v3.0.1 ([#485](https://github.com/conventional-changelog/standard-version/issues/485)) ([9cc188c](https://github.com/conventional-changelog/standard-version/commit/9cc188cbb84ee3ae80d5e66f5c54727877313b14))
* **deps:** update dependency yargs to v14.2.1 ([#483](https://github.com/conventional-changelog/standard-version/issues/483)) ([dc1fa61](https://github.com/conventional-changelog/standard-version/commit/dc1fa6170ffe12d4f8b44b70d23688a64d2ad0fb))
* **deps:** update dependency yargs to v14.2.2 ([#488](https://github.com/conventional-changelog/standard-version/issues/488)) ([ecf26b6](https://github.com/conventional-changelog/standard-version/commit/ecf26b6fc9421a78fb81793c4a932f579f7e9d4a))

### [7.0.1](https://github.com/conventional-changelog/standard-version/compare/v7.0.0...v7.0.1) (2019-11-07)


### Bug Fixes

* **deps:** update dependency conventional-changelog to v3.1.12 ([#463](https://github.com/conventional-changelog/standard-version/issues/463)) ([f04161a](https://github.com/conventional-changelog/standard-version/commit/f04161ae624705e68f9018d563e9f3c09ccf6f30))
* **deps:** update dependency conventional-changelog-config-spec to v2.1.0 ([#442](https://github.com/conventional-changelog/standard-version/issues/442)) ([a2c5747](https://github.com/conventional-changelog/standard-version/commit/a2c574735ac5a165a190661b7735ea284bdc7dda))
* **deps:** update dependency conventional-recommended-bump to v6.0.2 ([#462](https://github.com/conventional-changelog/standard-version/issues/462)) ([84bb581](https://github.com/conventional-changelog/standard-version/commit/84bb581209b50357761cbec45bb8253f6a182801))
* **deps:** update dependency stringify-package to v1.0.1 ([#459](https://github.com/conventional-changelog/standard-version/issues/459)) ([e06a835](https://github.com/conventional-changelog/standard-version/commit/e06a835c8296a92f4fa7c07f98057d765c1a91e5))
* **deps:** update dependency yargs to v14 ([#440](https://github.com/conventional-changelog/standard-version/issues/440)) ([fe37e73](https://github.com/conventional-changelog/standard-version/commit/fe37e7390760d8d16d1b94ca58d8123e292c46a8))
* **deps:** update dependency yargs to v14.2.0 ([#461](https://github.com/conventional-changelog/standard-version/issues/461)) ([fb21851](https://github.com/conventional-changelog/standard-version/commit/fb2185107a90ba4b9dc7c9c1d873ed1283706ac1))

## [7.0.0](https://github.com/conventional-changelog/standard-version/compare/v6.0.1...v7.0.0) (2019-07-30)


### ⚠ BREAKING CHANGES

* we were accepting .version.json as a config file, rather than .versionrc.json

### Bug Fixes

* **bump:** transmit tag prefix argument to conventionalRecommendedBump ([#393](https://github.com/conventional-changelog/standard-version/issues/393)) ([8205222](https://github.com/conventional-changelog/standard-version/commit/8205222))
* **cli:** display only one, correct default for --preset flag ([#377](https://github.com/conventional-changelog/standard-version/issues/377)) ([d17fc81](https://github.com/conventional-changelog/standard-version/commit/d17fc81))
* **commit:** don't try to process and add changelog if skipped ([#318](https://github.com/conventional-changelog/standard-version/issues/318)) ([3e4fdec](https://github.com/conventional-changelog/standard-version/commit/3e4fdec))
* **deps:** update dependency conventional-changelog-config-spec to v2 ([#352](https://github.com/conventional-changelog/standard-version/issues/352)) ([f586844](https://github.com/conventional-changelog/standard-version/commit/f586844))
* **deps:** update dependency conventional-recommended-bump to v6 ([#417](https://github.com/conventional-changelog/standard-version/issues/417)) ([4c5cad1](https://github.com/conventional-changelog/standard-version/commit/4c5cad1))
* **deps:** update dependency find-up to v4 ([#355](https://github.com/conventional-changelog/standard-version/issues/355)) ([73b35f8](https://github.com/conventional-changelog/standard-version/commit/73b35f8))
* **deps:** update dependency find-up to v4.1.0 ([#383](https://github.com/conventional-changelog/standard-version/issues/383)) ([b621a4a](https://github.com/conventional-changelog/standard-version/commit/b621a4a))
* **deps:** update dependency git-semver-tags to v3 ([#418](https://github.com/conventional-changelog/standard-version/issues/418)) ([1ce3f4a](https://github.com/conventional-changelog/standard-version/commit/1ce3f4a))
* **deps:** update dependency semver to v6.3.0 ([#366](https://github.com/conventional-changelog/standard-version/issues/366)) ([cd866c7](https://github.com/conventional-changelog/standard-version/commit/cd866c7))
* **deps:** update dependency yargs to v13.3.0 ([#401](https://github.com/conventional-changelog/standard-version/issues/401)) ([3d0e8c7](https://github.com/conventional-changelog/standard-version/commit/3d0e8c7))
* adds support for `releaseCommitMessageFormat` ([#351](https://github.com/conventional-changelog/standard-version/issues/351)) ([a7133cc](https://github.com/conventional-changelog/standard-version/commit/a7133cc))
* stop suggesting npm publish if package.json was not updated ([#319](https://github.com/conventional-changelog/standard-version/issues/319)) ([a5ac845](https://github.com/conventional-changelog/standard-version/commit/a5ac845))
* Updates package.json to _actual_ supported (tested) NodeJS versions. ([#379](https://github.com/conventional-changelog/standard-version/issues/379)) ([15eec8a](https://github.com/conventional-changelog/standard-version/commit/15eec8a))
* **deps:** update dependency yargs to v13.2.4 ([#356](https://github.com/conventional-changelog/standard-version/issues/356)) ([00b2ce6](https://github.com/conventional-changelog/standard-version/commit/00b2ce6))
* update config file name in command based on README.md ([#357](https://github.com/conventional-changelog/standard-version/issues/357)) ([ce44dd2](https://github.com/conventional-changelog/standard-version/commit/ce44dd2))

### [6.0.1](https://github.com/conventional-changelog/standard-version/compare/v6.0.0...v6.0.1) (2019-05-05)


### Bug Fixes

* don't pass args to git rev-parse ([1ac72f7](https://github.com/conventional-changelog/standard-version/commit/1ac72f7))



## [6.0.0](https://github.com/conventional-changelog/standard-version/compare/v5.0.2...v6.0.0) (2019-05-05)


### Bug Fixes

* always pass version to changelog context ([#327](https://github.com/conventional-changelog/standard-version/issues/327)) ([00e3381](https://github.com/conventional-changelog/standard-version/commit/00e3381))
* **deps:** update dependency detect-indent to v6 ([#341](https://github.com/conventional-changelog/standard-version/issues/341)) ([234d9dd](https://github.com/conventional-changelog/standard-version/commit/234d9dd))
* **deps:** update dependency detect-newline to v3 ([#342](https://github.com/conventional-changelog/standard-version/issues/342)) ([02a6093](https://github.com/conventional-changelog/standard-version/commit/02a6093))
* **deps:** update dependency figures to v3 ([#343](https://github.com/conventional-changelog/standard-version/issues/343)) ([7208ded](https://github.com/conventional-changelog/standard-version/commit/7208ded))
* **deps:** update dependency semver to v6 ([#344](https://github.com/conventional-changelog/standard-version/issues/344)) ([c40487a](https://github.com/conventional-changelog/standard-version/commit/c40487a))
* **deps:** update dependency yargs to v13 ([#345](https://github.com/conventional-changelog/standard-version/issues/345)) ([b2c8e59](https://github.com/conventional-changelog/standard-version/commit/b2c8e59))
* prevent duplicate headers from being added ([#305](https://github.com/conventional-changelog/standard-version/issues/305)) ([#307](https://github.com/conventional-changelog/standard-version/issues/307)) ([db2c6e5](https://github.com/conventional-changelog/standard-version/commit/db2c6e5))


### Build System

* add renovate.json ([#273](https://github.com/conventional-changelog/standard-version/issues/273)) ([bf41474](https://github.com/conventional-changelog/standard-version/commit/bf41474))
* drop Node 6 from testing matrix ([#346](https://github.com/conventional-changelog/standard-version/issues/346)) ([6718428](https://github.com/conventional-changelog/standard-version/commit/6718428))


### Features

* adds configurable conventionalcommits preset ([#323](https://github.com/conventional-changelog/standard-version/issues/323)) ([4fcd4a7](https://github.com/conventional-changelog/standard-version/commit/4fcd4a7))
* allow a user to provide a custom changelog header ([#335](https://github.com/conventional-changelog/standard-version/issues/335)) ([1c51064](https://github.com/conventional-changelog/standard-version/commit/1c51064))
* bump minor rather than major, if release is < 1.0.0 ([#347](https://github.com/conventional-changelog/standard-version/issues/347)) ([5d972cf](https://github.com/conventional-changelog/standard-version/commit/5d972cf))
* suggest branch name other than master ([#331](https://github.com/conventional-changelog/standard-version/issues/331)) ([304b49a](https://github.com/conventional-changelog/standard-version/commit/304b49a))
* update commit msg for when using commitAll ([#320](https://github.com/conventional-changelog/standard-version/issues/320)) ([74a040a](https://github.com/conventional-changelog/standard-version/commit/74a040a))


### Tests

* disable gpg signing in temporary test repositories. ([#311](https://github.com/conventional-changelog/standard-version/issues/311)) ([bd0fcdf](https://github.com/conventional-changelog/standard-version/commit/bd0fcdf))
* use const based on new eslint rules ([#329](https://github.com/conventional-changelog/standard-version/issues/329)) ([b6d3d13](https://github.com/conventional-changelog/standard-version/commit/b6d3d13))


### BREAKING CHANGES

* we now bump the minor rather than major if version < 1.0.0; --release-as can be used to bump to 1.0.0.
* tests are no longer run for Node 6
* we now use the conventionalcommits preset by default, which directly tracks conventionalcommits.org.



## [5.0.2](https://github.com/conventional-changelog/standard-version/compare/v5.0.1...v5.0.2) (2019-03-16)



## [5.0.1](https://github.com/conventional-changelog/standard-version/compare/v5.0.0...v5.0.1) (2019-02-28)


### Bug Fixes

* make pattern for finding CHANGELOG sections work for non anchors ([#292](https://github.com/conventional-changelog/standard-version/issues/292)) ([b684c78](https://github.com/conventional-changelog/standard-version/commit/b684c78))



# [5.0.0](https://github.com/conventional-changelog/standard-version/compare/v4.4.0...v5.0.0) (2019-02-14)


### Bug Fixes

* bin now enforces Node.js > 4 ([#274](https://github.com/conventional-changelog/standard-version/issues/274)) ([e1b5780](https://github.com/conventional-changelog/standard-version/commit/e1b5780))
* no --tag prerelease for private module ([#296](https://github.com/conventional-changelog/standard-version/issues/296)) ([27e2ab4](https://github.com/conventional-changelog/standard-version/commit/27e2ab4)), closes [#294](https://github.com/conventional-changelog/standard-version/issues/294)
* show correct pre-release tag in help output ([#259](https://github.com/conventional-changelog/standard-version/issues/259)) ([d90154a](https://github.com/conventional-changelog/standard-version/commit/d90154a))


### chore

* update testing matrix ([1d46627](https://github.com/conventional-changelog/standard-version/commit/1d46627))


### Features

* adds support for bumping for composer versions ([#262](https://github.com/conventional-changelog/standard-version/issues/262)) ([fee872f](https://github.com/conventional-changelog/standard-version/commit/fee872f))
* cli application accept path/preset option ([#279](https://github.com/conventional-changelog/standard-version/issues/279)) ([69c62cf](https://github.com/conventional-changelog/standard-version/commit/69c62cf))
* fallback to tags if no meta-information file found ([#275](https://github.com/conventional-changelog/standard-version/issues/275)) ([844cde6](https://github.com/conventional-changelog/standard-version/commit/844cde6))
* preserve formatting when writing to package.json ([#282](https://github.com/conventional-changelog/standard-version/issues/282)) ([96216da](https://github.com/conventional-changelog/standard-version/commit/96216da))


### BREAKING CHANGES

* if no package.json, bower.json, etc., is found, we now fallback to git tags
* removed Node 4/5 from testing matrix



<a name="4.4.0"></a>
# [4.4.0](https://github.com/conventional-changelog/standard-version/compare/v4.3.0...v4.4.0) (2018-05-21)


### Bug Fixes

* show full tag name in checkpoint ([#241](https://github.com/conventional-changelog/standard-version/issues/241)) ([b4ed4f9](https://github.com/conventional-changelog/standard-version/commit/b4ed4f9))
* use tagPrefix in CHANGELOG lifecycle step ([#243](https://github.com/conventional-changelog/standard-version/issues/243)) ([a56c7ac](https://github.com/conventional-changelog/standard-version/commit/a56c7ac))


### Features

* add prerelease lifecycle script hook (closes [#217](https://github.com/conventional-changelog/standard-version/issues/217)) ([#234](https://github.com/conventional-changelog/standard-version/issues/234)) ([ba4e7f6](https://github.com/conventional-changelog/standard-version/commit/ba4e7f6))
* manifest.json support ([#236](https://github.com/conventional-changelog/standard-version/issues/236)) ([371d992](https://github.com/conventional-changelog/standard-version/commit/371d992))



<a name="4.3.0"></a>
# [4.3.0](https://github.com/conventional-changelog/standard-version/compare/v4.2.0...v4.3.0) (2018-01-03)


### Bug Fixes

* recommend `--tag` prerelease for npm publish of prereleases ([#196](https://github.com/conventional-changelog/standard-version/issues/196)) ([709dae1](https://github.com/conventional-changelog/standard-version/commit/709dae1)), closes [#183](https://github.com/conventional-changelog/standard-version/issues/183)
* use the `skip` default value for skip cli arg ([#211](https://github.com/conventional-changelog/standard-version/issues/211)) ([3fdd7fa](https://github.com/conventional-changelog/standard-version/commit/3fdd7fa))


### Features

* **format-commit-message:** support multiple %s in the message ([45fcad5](https://github.com/conventional-changelog/standard-version/commit/45fcad5))
* do not update/commit files in .gitignore ([#230](https://github.com/conventional-changelog/standard-version/issues/230)) ([4fd3bc2](https://github.com/conventional-changelog/standard-version/commit/4fd3bc2))
* publish only if commit+push succeed ([#229](https://github.com/conventional-changelog/standard-version/issues/229)) ([c5e1ee2](https://github.com/conventional-changelog/standard-version/commit/c5e1ee2))



<a name="4.2.0"></a>
# [4.2.0](https://github.com/conventional-changelog/standard-version/compare/v4.1.0...v4.2.0) (2017-06-12)


### Features

* add support for `package-lock.json` ([#190](https://github.com/conventional-changelog/standard-version/issues/190)) ([bc0fc53](https://github.com/conventional-changelog/standard-version/commit/bc0fc53))



<a name="4.1.0"></a>
# [4.1.0](https://github.com/conventional-changelog/standard-version/compare/v4.0.0...v4.1.0) (2017-06-06)


### Features

* **cli:** print error and don't run with node <4, closes [#124](https://github.com/conventional-changelog/standard-version/issues/124) ([d0d71a5](https://github.com/conventional-changelog/standard-version/commit/d0d71a5))
* add dry-run mode ([#187](https://github.com/conventional-changelog/standard-version/issues/187)) ([d073353](https://github.com/conventional-changelog/standard-version/commit/d073353))
* add prebump, postbump, precommit, lifecycle scripts ([#186](https://github.com/conventional-changelog/standard-version/issues/186)) ([dfd1d12](https://github.com/conventional-changelog/standard-version/commit/dfd1d12))
* add support for `npm-shrinkwrap.json` ([#185](https://github.com/conventional-changelog/standard-version/issues/185)) ([86af7fc](https://github.com/conventional-changelog/standard-version/commit/86af7fc))
* add support for skipping lifecycle steps, polish lifecycle work ([#188](https://github.com/conventional-changelog/standard-version/issues/188)) ([d31dcdb](https://github.com/conventional-changelog/standard-version/commit/d31dcdb))
* allow a version # to be provided for release-as, rather than just major, minor, patch. ([13eb9cd](https://github.com/conventional-changelog/standard-version/commit/13eb9cd))



<a name="4.0.0"></a>
# [4.0.0](https://github.com/conventional-changelog/standard-version/compare/v4.0.0-1...v4.0.0) (2016-12-02)


### Bug Fixes

* include merge commits in the changelog ([#139](https://github.com/conventional-changelog/standard-version/issues/139)) ([b6e1562](https://github.com/conventional-changelog/standard-version/commit/b6e1562))
* should print message before we bump version ([2894bbc](https://github.com/conventional-changelog/standard-version/commit/2894bbc))
* support a wording change made to git status in git v2.9.1 ([#140](https://github.com/conventional-changelog/standard-version/issues/140)) ([80004ec](https://github.com/conventional-changelog/standard-version/commit/80004ec))


### Features

* add support for bumping version # in bower.json ([#148](https://github.com/conventional-changelog/standard-version/issues/148)) ([b788c5f](https://github.com/conventional-changelog/standard-version/commit/b788c5f))
* make tag prefix configurable ([#143](https://github.com/conventional-changelog/standard-version/issues/143)) ([70b20c8](https://github.com/conventional-changelog/standard-version/commit/70b20c8))
* support releasing a custom version, including pre-releases ([#129](https://github.com/conventional-changelog/standard-version/issues/129)) ([068008d](https://github.com/conventional-changelog/standard-version/commit/068008d))


### BREAKING CHANGES

* merge commits are now included in the CHANGELOG.


<a name="3.0.0"></a>
# [3.0.0](https://github.com/conventional-changelog/standard-version/compare/v2.3.0...v3.0.0) (2016-10-06)


### Bug Fixes

* check the private field in package.json([#102](https://github.com/conventional-changelog/standard-version/issues/102)) ([#103](https://github.com/conventional-changelog/standard-version/issues/103)) ([2ce4160](https://github.com/conventional-changelog/standard-version/commit/2ce4160))
* **err:** don't fail on stderr output, but print the output to stderr ([#110](https://github.com/conventional-changelog/standard-version/issues/110)) ([f7a4915](https://github.com/conventional-changelog/standard-version/commit/f7a4915)), closes [#91](https://github.com/conventional-changelog/standard-version/issues/91)


### Chores

* package.json engines field >=4.0, drop Node 0.10 and 0.12 ([28ff65a](https://github.com/conventional-changelog/standard-version/commit/28ff65a))


### Features

* **options:** add --silent flag and option for squelching output ([2a3fa61](https://github.com/conventional-changelog/standard-version/commit/2a3fa61))
* added support for commitAll option in CLI ([#121](https://github.com/conventional-changelog/standard-version/issues/121)) ([a903f4d](https://github.com/conventional-changelog/standard-version/commit/a903f4d))
* separate cli and defaults from base functionality ([34a6a4e](https://github.com/conventional-changelog/standard-version/commit/34a6a4e))


### BREAKING CHANGES

* drop support for Node < 4.0 to enable usage of
new tools and packages.



<a name="2.4.0"></a>
# [2.4.0](https://github.com/conventional-changelog/standard-version/compare/v2.3.1...v2.4.0) (2016-07-13)


### Bug Fixes

* **index.js:** use blue figures.info for last checkpoint ([#64](https://github.com/conventional-changelog/standard-version/issues/64)) ([e600b42](https://github.com/conventional-changelog/standard-version/commit/e600b42))


### Features

* **changelogStream:** use more default opts ([#67](https://github.com/conventional-changelog/standard-version/issues/67)) ([3e0aa84](https://github.com/conventional-changelog/standard-version/commit/3e0aa84))



<a name="2.3.1"></a>
## [2.3.1](https://github.com/conventional-changelog/standard-version/compare/v2.3.0...v2.3.1) (2016-06-15)


### Bug Fixes

* **commit:** fix windows by separating add and commit exec ([#55](https://github.com/conventional-changelog/standard-version/issues/55)) ([f361c46](https://github.com/conventional-changelog/standard-version/commit/f361c46)), closes [#55](https://github.com/conventional-changelog/standard-version/issues/55) [#49](https://github.com/conventional-changelog/standard-version/issues/49)



<a name="2.3.0"></a>
# [2.3.0](https://github.com/conventional-changelog/standard-version/compare/v2.2.1...v2.3.0) (2016-06-02)


### Bug Fixes

* append line feed to end of package.json ([#42](https://github.com/conventional-changelog/standard-version/issues/42))([178e001](https://github.com/conventional-changelog/standard-version/commit/178e001))


### Features

* **index.js:** add checkpoint for publish script after tag successfully ([#47](https://github.com/conventional-changelog/standard-version/issues/47))([e414ed7](https://github.com/conventional-changelog/standard-version/commit/e414ed7))
* add a --no-verify option to prevent git hooks from being verified ([#44](https://github.com/conventional-changelog/standard-version/issues/44))([026d844](https://github.com/conventional-changelog/standard-version/commit/026d844))



<a name="2.2.1"></a>
## [2.2.1](https://github.com/conventional-changelog/standard-version/compare/v2.2.0...v2.2.1) (2016-05-02)


### Bug Fixes

* upgrade to version of nyc that works with new shelljs([c7ac6e2](https://github.com/conventional-changelog/standard-version/commit/c7ac6e2))



<a name="2.2.0"></a>
# [2.2.0](https://github.com/conventional-changelog/standard-version/compare/v2.1.2...v2.2.0) (2016-05-01)


### Bug Fixes

* format the annotated tag message ([#28](https://github.com/conventional-changelog/standard-version/issues/28))([8f02736](https://github.com/conventional-changelog/standard-version/commit/8f02736))
* upgraded dependencies, switched back to angular format (fixes [#27](https://github.com/conventional-changelog/standard-version/issues/27)), pinned shelljs to version that works with nyc ([#30](https://github.com/conventional-changelog/standard-version/issues/30))([3f51e94](https://github.com/conventional-changelog/standard-version/commit/3f51e94))


### Features

* add --sign flag to sign git commit and tag ([#29](https://github.com/conventional-changelog/standard-version/issues/29))([de758bc](https://github.com/conventional-changelog/standard-version/commit/de758bc))



<a name="2.1.2"></a>
## [2.1.2](https://github.com/conventional-changelog/standard-version/compare/v2.1.1...v2.1.2) (2016-04-11)


### Bug Fixes

* we had too many \n characters ([#17](https://github.com/conventional-changelog/standard-version/issues/17)) ([67a01cd](https://github.com/conventional-changelog/standard-version/commit/67a01cd))



<a name="2.1.1"></a>
## [2.1.1](https://github.com/conventional-changelog/standard-version/compare/v2.1.0...v2.1.1) (2016-04-10)


### Bug Fixes

* **docs:** had a bad URL in package.json, which was breaking all of our links ([caa6359](https://github.com/conventional-changelog/standard-version/commit/caa6359))



<a name="2.1.0"></a>
# [2.1.0](https://github.com/conventional-changelog/standard-version/compare/v2.0.0...v2.1.0) (2016-04-10)


### Features

* adds support for GitHub links (see [#13](https://github.com/conventional-changelog/standard-version/issues/13)), great idea [@bcoe](https://github.com/bcoe)! ([7bf6597](https://github.com/conventional-changelog/standard-version/commit/7bf6597))



<a name="2.0.0"></a>
# [2.0.0](https://github.com/conventional-changelog/standard-version/compare/v1.1.0...v2.0.0) (2016-04-09)


* feat(conventional-changelog-standard): Move to conventional-changelog-standard style. This style lifts the character limit on commit messages, and puts us in a position to make more opinionated decisions in the future. ([c7ccadb](https://github.com/conventional-changelog/standard-version/commit/c7ccadb))


### BREAKING CHANGES

* we no longer accept the preset configuration option.


<a name="1.1.0"></a>
# [1.1.0](https://github.com/conventional-changelog/standard-version/compare/v1.0.0...v1.1.0) (2016-04-08)


### Features

* **cli:** use conventional default commit message with version ([9fadc5f](https://github.com/conventional-changelog/standard-version/commit/9fadc5f))
* **rebrand:** rebrand recommended-workflow to standard-version (#9) ([1f673c0](https://github.com/conventional-changelog/standard-version/commit/1f673c0))
* **tests:** adds test suite, fixed several Node 0.10 issues along the way ([03bd86c](https://github.com/conventional-changelog/standard-version/commit/03bd86c))



<a name="1.0.0"></a>
# 1.0.0 (2016-04-04)


### Features

* **initial-release:** adds flag for generating CHANGELOG.md on the first release. ([b812b44](https://github.com/bcoe/conventional-recommended-workflow/commit/b812b44))
