# Changelog

## [5.0.0](https://github.com/SgtPooki/helia/compare/interface-v4.1.0...interface-v5.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* `helia.pin.add` and `helia.pin.rm` now return `AsyncGenerator<CID>`
* The libp2p API has changed in a couple of places - please see the [upgrade guide](https://github.com/libp2p/js-libp2p/blob/main/doc/migrations/v0.46-v1.0.0.md)
* libp2p has been updated to 0.46.x

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* add block session support to @helia/interface ([#398](https://github.com/SgtPooki/helia/issues/398)) ([5cf216b](https://github.com/SgtPooki/helia/commit/5cf216baa6806cd82f8fcddd1f024ef6a506f667))
* add offline option to blockstore get ([#145](https://github.com/SgtPooki/helia/issues/145)) ([71c5f6b](https://github.com/SgtPooki/helia/commit/71c5f6bc32b324ee237e56c2c5a1ce903b3bdbef))
* configurable block brokers ([#280](https://github.com/SgtPooki/helia/issues/280)) ([0749cbf](https://github.com/SgtPooki/helia/commit/0749cbf99745ea6ab4363f1b5d635634ca0ddcfa))
* expose .dns property on @helia/interface ([#465](https://github.com/SgtPooki/helia/issues/465)) ([8c9bb7d](https://github.com/SgtPooki/helia/commit/8c9bb7d224a1b786cba1fba18bffe07001a3b95d))
* expose configured dag walkers and hashers on helia interface ([#381](https://github.com/SgtPooki/helia/issues/381)) ([843fba4](https://github.com/SgtPooki/helia/commit/843fba467ebb032907c888da499147a5349ec10e)), closes [#375](https://github.com/SgtPooki/helia/issues/375)
* GatewayBlockBroker prioritizes & tries all gateways ([#281](https://github.com/SgtPooki/helia/issues/281)) ([9bad21b](https://github.com/SgtPooki/helia/commit/9bad21bd59fe6d1ba4a137db5a46bd2ead5238c3))
* iterable pinning ([#231](https://github.com/SgtPooki/helia/issues/231)) ([c15c774](https://github.com/SgtPooki/helia/commit/c15c7749294d3d4aea5aef70544d088250336798))
* provide default libp2p instance ([#127](https://github.com/SgtPooki/helia/issues/127)) ([45c9d89](https://github.com/SgtPooki/helia/commit/45c9d896afa27f5ea043cc5f576d50fc4fa556e9)), closes [#121](https://github.com/SgtPooki/helia/issues/121)


### Bug Fixes

* add helia version to agent version ([#128](https://github.com/SgtPooki/helia/issues/128)) ([48e19ec](https://github.com/SgtPooki/helia/commit/48e19ec545cc67157e14ae59054fa377a583cb01)), closes [#122](https://github.com/SgtPooki/helia/issues/122)
* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* create @helia/block-brokers package ([#341](https://github.com/SgtPooki/helia/issues/341)) ([#342](https://github.com/SgtPooki/helia/issues/342)) ([2979147](https://github.com/SgtPooki/helia/commit/297914756fa06dc0c28890a2654d1159d16689c2))
* pass options to blockstore.get during pin.add ([#148](https://github.com/SgtPooki/helia/issues/148)) ([3a5234e](https://github.com/SgtPooki/helia/commit/3a5234e3c2f88f9910678b0cbbac5fd340117cc9))
* update block events ([#58](https://github.com/SgtPooki/helia/issues/58)) ([d33be53](https://github.com/SgtPooki/helia/commit/d33be534972a4c238fc6d43c4284c6bd834ae218))
* update ipns module to v9 and fix double verification of records ([#396](https://github.com/SgtPooki/helia/issues/396)) ([f2853f8](https://github.com/SgtPooki/helia/commit/f2853f8bd5bdcee8ab7a685355b0be47f29620e0))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))
* update generated docs to include version in module names ([#296](https://github.com/SgtPooki/helia/issues/296)) ([0776106](https://github.com/SgtPooki/helia/commit/0776106710d6641ac82b446f7fde6c40d788a0b4))


### Dependencies

* bump multiformats from 12.1.3 to 13.0.0 ([#354](https://github.com/SgtPooki/helia/issues/354)) ([1d16bf8](https://github.com/SgtPooki/helia/commit/1d16bf89acd10ac79baf53f0cbc5f92d0e9d8301))
* **dev:** bump aegir from 39.0.13 to 40.0.8 ([#198](https://github.com/SgtPooki/helia/issues/198)) ([4d75ecf](https://github.com/SgtPooki/helia/commit/4d75ecffb79e5177da35d3106e42dac7bc63153a))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#273](https://github.com/SgtPooki/helia/issues/273)) ([9a9f637](https://github.com/SgtPooki/helia/commit/9a9f63787223eff7eae3b72e59b79b11baa621ea))
* update interface-store to 5.x.x ([#63](https://github.com/SgtPooki/helia/issues/63)) ([5bf11d6](https://github.com/SgtPooki/helia/commit/5bf11d638eee423624ac49af97757d730744f384))
* update libp2p patch versions ([917a1bc](https://github.com/SgtPooki/helia/commit/917a1bceb9e9b56428a15dc3377a963f06affd12))
* update libp2p to 0.46.x ([#215](https://github.com/SgtPooki/helia/issues/215)) ([65b68f0](https://github.com/SgtPooki/helia/commit/65b68f071d04d2f6f0fcf35938b146706b1a3cd0))
* updates to libp2p v1 ([#320](https://github.com/SgtPooki/helia/issues/320)) ([635d7a2](https://github.com/SgtPooki/helia/commit/635d7a2938111ccc53f8defbd9b8f8f8ea3e8e6a))


### Refactors

* use functions for block broker creation ([#286](https://github.com/SgtPooki/helia/issues/286)) ([43932a5](https://github.com/SgtPooki/helia/commit/43932a54036dafdf1265b034b30b12784fd22d82))
