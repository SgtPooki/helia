# Changelog

## [8.0.0](https://github.com/SgtPooki/helia/compare/ipns-v7.2.0...ipns-v8.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* requires @helia/interface@4.1.x or later, `resolveDns` has been renamed `resolveDNSLink`
* to support paths in `@helia/ipns`, the return type of `ipns.resolve` is now `{ path: string, cid: CID }` instead of just `CID`
* remove gossipsub from default libp2p services ([#401](https://github.com/SgtPooki/helia/issues/401))
* `helia.routing` is the default routing used, the `libp2p` routing has been removed as it is redundant
* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13 and helia v3, renames `dht` routing to `libp2p`
* alters the options object passed to the `ipns` factory function
* the `IPNSRecord` type returned from the `publish` method has changed

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* add `record`/`answer` fields to IPNS results ([#471](https://github.com/SgtPooki/helia/issues/471)) ([b6765fe](https://github.com/SgtPooki/helia/commit/b6765fe7632231407c4a8506015ac07e30152190))
* add cache control to IPNS ([#473](https://github.com/SgtPooki/helia/issues/473)) ([b00f682](https://github.com/SgtPooki/helia/commit/b00f682647d3687e54bd48f8f68ab79d1e4e96cc))
* allow publish/resolve using only local datastore ([#15](https://github.com/SgtPooki/helia/issues/15)) ([43e32a2](https://github.com/SgtPooki/helia/commit/43e32a20f44fffd533531a57e6d60883cebc55ca))
* support DNS over HTTPS and DNS-JSON over HTTPS ([#55](https://github.com/SgtPooki/helia/issues/55)) ([2ac0e8b](https://github.com/SgtPooki/helia/commit/2ac0e8b26556b73961e67191c564ac2b18d32b31))
* support paths in @helia/ipns ([#410](https://github.com/SgtPooki/helia/issues/410)) ([ca8d5eb](https://github.com/SgtPooki/helia/commit/ca8d5ebdf587574c7fb84517b558226c3479caa9))
* update helia to v3 and multiformats to v13 ([#167](https://github.com/SgtPooki/helia/issues/167)) ([a0381b9](https://github.com/SgtPooki/helia/commit/a0381b95051bbf3edfa4f53e0ae2d5f43c1e4382))
* use custom DNS resolver in @helia/ipns for DNSLink ([#466](https://github.com/SgtPooki/helia/issues/466)) ([2c71b6e](https://github.com/SgtPooki/helia/commit/2c71b6ec8d34dcc722a3914702f67603492c335f)), closes [#369](https://github.com/SgtPooki/helia/issues/369)
* use helia router for IPNS put/get ([#387](https://github.com/SgtPooki/helia/issues/387)) ([ce74026](https://github.com/SgtPooki/helia/commit/ce740268e83f50e6f144b74969a98d54005cd852))


### Bug Fixes

* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* cache IPNS entries after resolving ([#35](https://github.com/SgtPooki/helia/issues/35)) ([704b413](https://github.com/SgtPooki/helia/commit/704b41355768b3e8723560c5f7ed3d7c12b58c3b)), closes [#20](https://github.com/SgtPooki/helia/issues/20)
* export IPNSRoutingEvents ([#407](https://github.com/SgtPooki/helia/issues/407)) ([44f4e88](https://github.com/SgtPooki/helia/commit/44f4e88030a21d86b2a8473d3d00efb624cfce8f))
* make @libp2p/interface a dependency ([#159](https://github.com/SgtPooki/helia/issues/159)) ([546ecf0](https://github.com/SgtPooki/helia/commit/546ecf023bd619d32e187fa6a55d39fcf12e4bbe)), closes [#158](https://github.com/SgtPooki/helia/issues/158)
* remove gossipsub from default libp2p services ([#401](https://github.com/SgtPooki/helia/issues/401)) ([99c94f4](https://github.com/SgtPooki/helia/commit/99c94f4b85c4ed826a6195207e3545cbbc87a6d1))
* remove is-ipfs from @helia/ipns dependencies ([#421](https://github.com/SgtPooki/helia/issues/421)) ([3851fe2](https://github.com/SgtPooki/helia/commit/3851fe2df6af337b7e2cabe694bd3dba17748fce))
* respect the IPNS TTL field ([#482](https://github.com/SgtPooki/helia/issues/482)) ([1561e4a](https://github.com/SgtPooki/helia/commit/1561e4a106074b94e421a77b0b8776b065e48bc5))
* update ipns module to v9 and fix double verification of records ([#396](https://github.com/SgtPooki/helia/issues/396)) ([f2853f8](https://github.com/SgtPooki/helia/commit/f2853f8bd5bdcee8ab7a685355b0be47f29620e0))
* update libp2p interfaces ([#109](https://github.com/SgtPooki/helia/issues/109)) ([514b6e1](https://github.com/SgtPooki/helia/commit/514b6e1e4192f700a6f0e769d52a4ec5dfe757ec))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use the content routing api for get/put operations ([#34](https://github.com/SgtPooki/helia/issues/34)) ([55208cc](https://github.com/SgtPooki/helia/commit/55208ccfdc4f3a799736f29e614910cbd8375a9d))


### Documentation

* fix typo ([#113](https://github.com/SgtPooki/helia/issues/113)) ([d732db9](https://github.com/SgtPooki/helia/commit/d732db9f4fea23aa11456d451f02d4f143846ba3))
* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))


### Dependencies

* bump @libp2p/logger from 2.1.1 to 3.0.2 ([#87](https://github.com/SgtPooki/helia/issues/87)) ([b2886b9](https://github.com/SgtPooki/helia/commit/b2886b9598a66a31c69ee0c3c7e13748614be37e))
* bump multiformats from 11.0.2 to 12.0.1 ([#57](https://github.com/SgtPooki/helia/issues/57)) ([6f93e51](https://github.com/SgtPooki/helia/commit/6f93e51e9b6f603f7c1d396705dc5b190108fe79))
* **dev:** bump aegir from 39.0.13 to 40.0.8 ([#65](https://github.com/SgtPooki/helia/issues/65)) ([174987b](https://github.com/SgtPooki/helia/commit/174987b2817cfe99cbabb9835dd6a2d99c1c35a9))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#107](https://github.com/SgtPooki/helia/issues/107)) ([5402d30](https://github.com/SgtPooki/helia/commit/5402d30de1437052e9e9b955d9be3c2898515447))
* **dev:** bump libp2p from 0.45.9 to 0.46.6 ([#92](https://github.com/SgtPooki/helia/issues/92)) ([efe02e5](https://github.com/SgtPooki/helia/commit/efe02e5b38992189edb40cd34d79e76dca4c34a3))
* **dev:** bump sinon from 15.2.0 to 16.0.0 ([#105](https://github.com/SgtPooki/helia/issues/105)) ([231ebbd](https://github.com/SgtPooki/helia/commit/231ebbd4cda2196d7914a81aa1b0d79473c3a325))
* **dev:** bump sinon from 16.1.3 to 17.0.0 ([#108](https://github.com/SgtPooki/helia/issues/108)) ([530aeff](https://github.com/SgtPooki/helia/commit/530aeff8af103c9126411cc1b035ee106f113f1f))
* update all deps and fix linting ([4cdba4f](https://github.com/SgtPooki/helia/commit/4cdba4fda743e7805725f4155242b93bc74ba4ae))
* update ipns to 6.x.x ([#12](https://github.com/SgtPooki/helia/issues/12)) ([6866638](https://github.com/SgtPooki/helia/commit/6866638830f32442f9cfeadbde795e74b0865e00))
* update ipns to v7.x.x ([#106](https://github.com/SgtPooki/helia/issues/106)) ([83a1d14](https://github.com/SgtPooki/helia/commit/83a1d147e8ba758efd7d2574ea486218bd1f3df2))
* update libp2p patch versions ([917a1bc](https://github.com/SgtPooki/helia/commit/917a1bceb9e9b56428a15dc3377a963f06affd12))
* The following workspace dependencies were updated
  * dependencies
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
