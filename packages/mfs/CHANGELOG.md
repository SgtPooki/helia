# Changelog

## [4.0.0](https://github.com/SgtPooki/helia/compare/mfs-v3.0.3...mfs-v4.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* initial import ([a70f4eb](https://github.com/SgtPooki/helia/commit/a70f4eb982e377eeeeb6fd4a53f7baf40c09641b))
* update helia to v3 and multiformats to v13 ([9f7dc0a](https://github.com/SgtPooki/helia/commit/9f7dc0a0581524531501fc062fefb6ba26d99c02))


### Bug Fixes

* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use blockstore interface where possible ([#417](https://github.com/SgtPooki/helia/issues/417)) ([30c8981](https://github.com/SgtPooki/helia/commit/30c8981934ffba72d572a7b8b2712ec93b7f4d31))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))
* update docs to use MFS style API ([#4](https://github.com/SgtPooki/helia/issues/4)) ([88b23b0](https://github.com/SgtPooki/helia/commit/88b23b0db4ac9da2a9e94291f2db7b10f436ce00))


### Dependencies

* bump @helia/interface from 1.2.2 to 2.0.0 ([#2](https://github.com/SgtPooki/helia/issues/2)) ([351fae7](https://github.com/SgtPooki/helia/commit/351fae7a129e642a6f312c9a61609273dec190bf))
* **dev:** bump helia from 2.0.1 to 2.0.3 ([#10](https://github.com/SgtPooki/helia/issues/10)) ([6911470](https://github.com/SgtPooki/helia/commit/6911470cb43720798fca571669a166eb3689dad2))
* update libp2p patch versions ([917a1bc](https://github.com/SgtPooki/helia/commit/917a1bceb9e9b56428a15dc3377a963f06affd12))
* The following workspace dependencies were updated
  * dependencies
    * @helia/unixfs bumped from ^3.0.3 to ^4.0.0
