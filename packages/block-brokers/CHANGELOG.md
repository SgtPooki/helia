# Changelog

## [3.0.0](https://github.com/SgtPooki/helia/compare/block-brokers-v2.0.3...block-brokers-v3.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module

### Features

* add @helia/bitswap with sessions ([#409](https://github.com/SgtPooki/helia/issues/409)) ([e582c63](https://github.com/SgtPooki/helia/commit/e582c63ca296c789312f5fcf5e3e18f267f74c03))
* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* add block session support to @helia/interface ([#398](https://github.com/SgtPooki/helia/issues/398)) ([5cf216b](https://github.com/SgtPooki/helia/commit/5cf216baa6806cd82f8fcddd1f024ef6a506f667))
* add sessions to trustless gateways ([#459](https://github.com/SgtPooki/helia/issues/459)) ([6ddefb0](https://github.com/SgtPooki/helia/commit/6ddefb01154b970f5ab7ec7cb7445d9eedbc5474))
* expose configured dag walkers and hashers on helia interface ([#381](https://github.com/SgtPooki/helia/issues/381)) ([843fba4](https://github.com/SgtPooki/helia/commit/843fba467ebb032907c888da499147a5349ec10e)), closes [#375](https://github.com/SgtPooki/helia/issues/375)


### Bug Fixes

* @helia/block-brokers gateways uses path gateways ([#374](https://github.com/SgtPooki/helia/issues/374)) ([94b0cd1](https://github.com/SgtPooki/helia/commit/94b0cd162ce864d44726a1d486389b0a1fdd3efc))
* create @helia/block-brokers package ([#341](https://github.com/SgtPooki/helia/issues/341)) ([#342](https://github.com/SgtPooki/helia/issues/342)) ([2979147](https://github.com/SgtPooki/helia/commit/297914756fa06dc0c28890a2654d1159d16689c2))
* remove w3s.link default block-broker ([#371](https://github.com/SgtPooki/helia/issues/371)) ([5c4fd54](https://github.com/SgtPooki/helia/commit/5c4fd54207384165c4e6309ec7663e996d7d66d4))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))


### Dependencies

* update libp2p patch versions ([917a1bc](https://github.com/SgtPooki/helia/commit/917a1bceb9e9b56428a15dc3377a963f06affd12))
* The following workspace dependencies were updated
  * dependencies
    * @helia/bitswap bumped from ^0.0.0 to ^1.0.0
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
