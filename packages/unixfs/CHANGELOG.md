# Changelog

## [4.0.0](https://github.com/SgtPooki/helia/compare/unixfs-v3.0.3...unixfs-v4.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13 and helia v3

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* add globSource and urlSource ([#53](https://github.com/SgtPooki/helia/issues/53)) ([b490a6e](https://github.com/SgtPooki/helia/commit/b490a6e35cb521c0c29d0f1382fc2e4b3b662b9c))
* add offline option to all operations ([#51](https://github.com/SgtPooki/helia/issues/51)) ([444c8bd](https://github.com/SgtPooki/helia/commit/444c8bd0dd40d8cad7ca12f3fbffaaf19f8e75fc))
* expose progress events from importer, blockstore and bitswap ([#13](https://github.com/SgtPooki/helia/issues/13)) ([de78f4d](https://github.com/SgtPooki/helia/commit/de78f4d03ebafe9ed9a2dfcbfb7a516fa215585c))
* expose unixfs progress events in types ([#14](https://github.com/SgtPooki/helia/issues/14)) ([36cf3b2](https://github.com/SgtPooki/helia/commit/36cf3b2143276a59b685ceb58299c4f881545fee))
* update helia to v3 and multiformats to v13 ([#147](https://github.com/SgtPooki/helia/issues/147)) ([001247c](https://github.com/SgtPooki/helia/commit/001247c6fc38ff3d810736371de901e5e1099f26))


### Bug Fixes

* Add GlobSourceResult to globSource return type in unixfs. ([#475](https://github.com/SgtPooki/helia/issues/475)) ([9ac5909](https://github.com/SgtPooki/helia/commit/9ac59098d3e4c8644756a83b185308d7d91626c1))
* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* convert date to mtime in glob source ([#106](https://github.com/SgtPooki/helia/issues/106)) ([cd9e903](https://github.com/SgtPooki/helia/commit/cd9e903c2ccac61372eaa64a61b4a8f3d79f9d4a))
* correct browser override path for glob-source ([#60](https://github.com/SgtPooki/helia/issues/60)) ([fd0f33b](https://github.com/SgtPooki/helia/commit/fd0f33b2a66e2840b5a03f27a48240b3c5d2b67e))
* export unixfs errors ([#50](https://github.com/SgtPooki/helia/issues/50)) ([8426d65](https://github.com/SgtPooki/helia/commit/8426d650ae4645b7b975331c5fd02f56e390cab6))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use blockstore interface where possible ([#417](https://github.com/SgtPooki/helia/issues/417)) ([30c8981](https://github.com/SgtPooki/helia/commit/30c8981934ffba72d572a7b8b2712ec93b7f4d31))
* use unixfs exporter to traverse DAGs ([#455](https://github.com/SgtPooki/helia/issues/455)) ([6f8c15b](https://github.com/SgtPooki/helia/commit/6f8c15b769c08bf73e7c62dab79909b5ecfc3c93))


### Documentation

* fix typos in example code ([#57](https://github.com/SgtPooki/helia/issues/57)) ([b7625c3](https://github.com/SgtPooki/helia/commit/b7625c3426380e63052968b1476e2d689c9213de))
* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))


### Dependencies

* bump @helia/interface from 1.2.2 to 2.0.0 ([#87](https://github.com/SgtPooki/helia/issues/87)) ([098a305](https://github.com/SgtPooki/helia/commit/098a305241024ed3903b686892ded8abfca55f5f))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#105](https://github.com/SgtPooki/helia/issues/105)) ([2421ee2](https://github.com/SgtPooki/helia/commit/2421ee2b4440446160e1a665bc5ecfc92d2b64de))
* update all deps and fix linting ([d4d6515](https://github.com/SgtPooki/helia/commit/d4d6515f023db339874d34871e69fb7c3fc47f6c))
* update all it-* deps to latest versions ([#25](https://github.com/SgtPooki/helia/issues/25)) ([9388c40](https://github.com/SgtPooki/helia/commit/9388c402462a1d45fcb7ded285262881718b7dd0))
* update helia deps to v1 ([#16](https://github.com/SgtPooki/helia/issues/16)) ([7497590](https://github.com/SgtPooki/helia/commit/74975903ec619a4662e5bfa9546997641e9f8e8c))
* update libp2p patch versions ([917a1bc](https://github.com/SgtPooki/helia/commit/917a1bceb9e9b56428a15dc3377a963f06affd12))
* The following workspace dependencies were updated
  * dependencies
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
