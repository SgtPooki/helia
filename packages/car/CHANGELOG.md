# Changelog

## [4.0.0](https://github.com/SgtPooki/helia/compare/car-v3.1.2...car-v4.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13 and helia v3

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* expose configured dag walkers and hashers on helia interface ([#381](https://github.com/SgtPooki/helia/issues/381)) ([843fba4](https://github.com/SgtPooki/helia/commit/843fba467ebb032907c888da499147a5349ec10e)), closes [#375](https://github.com/SgtPooki/helia/issues/375)
* initial import ([95e68a1](https://github.com/SgtPooki/helia/commit/95e68a12ac7f829b7aa455b571f942dfc82394ed))
* stream car file bytes from @helia/car ([#444](https://github.com/SgtPooki/helia/issues/444)) ([7c07e11](https://github.com/SgtPooki/helia/commit/7c07e113d644a1efc32b7fd0c268f5f892256ce9))
* update helia to v3 and multiformats to v13 ([#52](https://github.com/SgtPooki/helia/issues/52)) ([6405c34](https://github.com/SgtPooki/helia/commit/6405c3487879614dc4dd7308b15c946d644e0488))


### Bug Fixes

* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* import from multiformats/cid for smaller bundles ([0857d1f](https://github.com/SgtPooki/helia/commit/0857d1f76cd7403dbea46cf3d9c891543fc83fe1))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use blockstore interface where possible ([#417](https://github.com/SgtPooki/helia/issues/417)) ([30c8981](https://github.com/SgtPooki/helia/commit/30c8981934ffba72d572a7b8b2712ec93b7f4d31))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* fs already defined in example ([#1](https://github.com/SgtPooki/helia/issues/1)) ([356797a](https://github.com/SgtPooki/helia/commit/356797a9493c7753178b5f343962951bc9cd3052))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))


### Dependencies

* bump @helia/interface from 1.2.2 to 2.0.0 ([#32](https://github.com/SgtPooki/helia/issues/32)) ([68656a8](https://github.com/SgtPooki/helia/commit/68656a81b7cd1238641a41573915635905e4a6ed))
* bump cborg from 1.10.2 to 2.0.5 ([#35](https://github.com/SgtPooki/helia/issues/35)) ([10994ea](https://github.com/SgtPooki/helia/commit/10994ea9abdff8906ae8c3f7d0ff5f50b50d9e60))
* bump multiformats from 11.0.2 to 12.0.1 ([#4](https://github.com/SgtPooki/helia/issues/4)) ([50bed0f](https://github.com/SgtPooki/helia/commit/50bed0f32b3c07111de804b0e6471e36d8e66626))
* **dev:** bump aegir from 39.0.13 to 40.0.11 ([#30](https://github.com/SgtPooki/helia/issues/30)) ([ea26a0b](https://github.com/SgtPooki/helia/commit/ea26a0bd14137eb1de6ab282cdcecd55578064ab))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#41](https://github.com/SgtPooki/helia/issues/41)) ([e8fc99f](https://github.com/SgtPooki/helia/commit/e8fc99f4e372eaf72c2598f5a7a9942143c6d788))
* The following workspace dependencies were updated
  * dependencies
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
  * devDependencies
    * @helia/unixfs bumped from ^3.0.3 to ^4.0.0
