# Changelog

## [4.0.0](https://github.com/SgtPooki/helia/compare/dag-json-v3.0.2...dag-json-v4.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13 and helia v3

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* initial import ([bac0ac5](https://github.com/SgtPooki/helia/commit/bac0ac5f2778f16a3d8219c73a3e6f0665adf3dd))
* update helia to v3 and multiformats to v13 ([#45](https://github.com/SgtPooki/helia/issues/45)) ([3c7d9d4](https://github.com/SgtPooki/helia/commit/3c7d9d4a8e74e1a808c265fbc6ecbdc24f0f3da9))


### Bug Fixes

* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use blockstore interface where possible ([#417](https://github.com/SgtPooki/helia/issues/417)) ([30c8981](https://github.com/SgtPooki/helia/commit/30c8981934ffba72d572a7b8b2712ec93b7f4d31))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* replace references to json with dag-json ([f1944b0](https://github.com/SgtPooki/helia/commit/f1944b04271a599eee987d56d4d8506eaeb8a69d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))
* update tocs ([0b4bac4](https://github.com/SgtPooki/helia/commit/0b4bac4583f790686ceaf89f2f2ab6642677c4fd))


### Dependencies

* bump @helia/interface from 1.2.2 to 2.0.0 ([#32](https://github.com/SgtPooki/helia/issues/32)) ([eb836ef](https://github.com/SgtPooki/helia/commit/eb836ef15f6bc754fbab4fdbe47c76f5492a56d9))
* bump multiformats from 11.0.2 to 12.0.1 ([#8](https://github.com/SgtPooki/helia/issues/8)) ([c89b8f1](https://github.com/SgtPooki/helia/commit/c89b8f12d700f0e23dc574cc32f7726d9c9558de))
* **dev:** bump aegir from 39.0.13 to 40.0.11 ([#28](https://github.com/SgtPooki/helia/issues/28)) ([d126e6a](https://github.com/SgtPooki/helia/commit/d126e6a3c845f25a4910c18fa476304d8534be91))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#36](https://github.com/SgtPooki/helia/issues/36)) ([9f57d11](https://github.com/SgtPooki/helia/commit/9f57d11e461a3b1fddbc2a92e225d31eee56613c))
* The following workspace dependencies were updated
  * dependencies
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
