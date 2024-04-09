# Changelog

## [4.0.0](https://github.com/SgtPooki/helia/compare/json-v3.0.2...json-v4.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13 and helia v3

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* inital import ([78ad71b](https://github.com/SgtPooki/helia/commit/78ad71b02ac136b704aa3d7a56e4d6d1c9c93f8e))
* update helia to v3 and multiformats to v13 ([#46](https://github.com/SgtPooki/helia/issues/46)) ([e3dc586](https://github.com/SgtPooki/helia/commit/e3dc5867ffc4de0dd3b05b56eb1b0ce98d50dcb1))


### Bug Fixes

* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use blockstore interface where possible ([#417](https://github.com/SgtPooki/helia/issues/417)) ([30c8981](https://github.com/SgtPooki/helia/commit/30c8981934ffba72d572a7b8b2712ec93b7f4d31))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))
* update comment ([1e0d49a](https://github.com/SgtPooki/helia/commit/1e0d49a4ecb94b1ef07b8a814a095cea533222a3))


### Dependencies

* bump @helia/interface from 1.2.2 to 2.0.0 ([#34](https://github.com/SgtPooki/helia/issues/34)) ([d48f2c5](https://github.com/SgtPooki/helia/commit/d48f2c58338af0d096a1f855ab85a621fce1cc01))
* bump multiformats from 11.0.2 to 12.0.1 ([#8](https://github.com/SgtPooki/helia/issues/8)) ([c2a2ee3](https://github.com/SgtPooki/helia/commit/c2a2ee38cc8fa76c8a6d0c92c44023c148148a7e))
* **dev:** bump aegir from 39.0.13 to 40.0.11 ([#26](https://github.com/SgtPooki/helia/issues/26)) ([37b6ba1](https://github.com/SgtPooki/helia/commit/37b6ba14e085073b966fced3c3777519601d0a81))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#36](https://github.com/SgtPooki/helia/issues/36)) ([ca3f05a](https://github.com/SgtPooki/helia/commit/ca3f05a74316f53b0e44f5edd6e303b6e8463bf2))
* The following workspace dependencies were updated
  * dependencies
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
