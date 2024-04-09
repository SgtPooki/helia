# Changelog

## [4.0.0](https://github.com/SgtPooki/helia/compare/strings-v3.0.2...strings-v4.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13 and helia v3

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* initial import ([23a13d8](https://github.com/SgtPooki/helia/commit/23a13d844c3b9adfdea13214d974f1c7e1d7539d))
* update helia to v3 and multiformats to v13 ([#87](https://github.com/SgtPooki/helia/issues/87)) ([ae7cbc9](https://github.com/SgtPooki/helia/commit/ae7cbc9a16a267cb0f6d7cecd381f919430afaea))


### Bug Fixes

* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* linting and deps ([22d3900](https://github.com/SgtPooki/helia/commit/22d3900c15b0876419460c4db57b41f91e78d52f))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use blockstore interface where possible ([#417](https://github.com/SgtPooki/helia/issues/417)) ([30c8981](https://github.com/SgtPooki/helia/commit/30c8981934ffba72d572a7b8b2712ec93b7f4d31))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))
* update readme ([#6](https://github.com/SgtPooki/helia/issues/6)) ([c62f784](https://github.com/SgtPooki/helia/commit/c62f78499d75ba96da60a4de2f6a0ae3f007abfb))
* update readmes ([2a700dc](https://github.com/SgtPooki/helia/commit/2a700dc30945857e5ec596a8551adf488dc18009))
* update tocs ([3d4573d](https://github.com/SgtPooki/helia/commit/3d4573d9bc22bdd79043b6fec570e8410c8d1228))


### Dependencies

* bump @helia/interface from 1.2.2 to 2.0.0 ([#39](https://github.com/SgtPooki/helia/issues/39)) ([7c9bc2e](https://github.com/SgtPooki/helia/commit/7c9bc2e9f99ccbaec1d8c25c900585deb5f6a327))
* The following workspace dependencies were updated
  * dependencies
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
