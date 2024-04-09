# Changelog

## [4.0.0](https://github.com/SgtPooki/helia/compare/dag-cbor-v3.0.2...dag-cbor-v4.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* uses multiformats v13 and helia v3

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* initial commit ([ed4c319](https://github.com/SgtPooki/helia/commit/ed4c319a67c18a3dd65e18f18aa12e82080b3fdc))
* update helia to v3 and multiformats to v13 ([#45](https://github.com/SgtPooki/helia/issues/45)) ([f078447](https://github.com/SgtPooki/helia/commit/f078447b6eba4c3d404d62bb930757aa1c0efe74))


### Bug Fixes

* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use blockstore interface where possible ([#417](https://github.com/SgtPooki/helia/issues/417)) ([30c8981](https://github.com/SgtPooki/helia/commit/30c8981934ffba72d572a7b8b2712ec93b7f4d31))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))


### Dependencies

* bump @helia/interface from 1.2.2 to 2.0.0 ([#30](https://github.com/SgtPooki/helia/issues/30)) ([aa6ebcf](https://github.com/SgtPooki/helia/commit/aa6ebcf9f58eebf842113985adee4710b009562d))
* bump multiformats from 11.0.2 to 12.0.1 ([#8](https://github.com/SgtPooki/helia/issues/8)) ([7a842d3](https://github.com/SgtPooki/helia/commit/7a842d3cc4cd97e02e5a196aa512cfe36be4c388))
* **dev:** bump aegir from 39.0.13 to 40.0.11 ([#29](https://github.com/SgtPooki/helia/issues/29)) ([973bb5b](https://github.com/SgtPooki/helia/commit/973bb5b6c8db0fedd70e4058f97bc339018a8193))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#36](https://github.com/SgtPooki/helia/issues/36)) ([77e29bc](https://github.com/SgtPooki/helia/commit/77e29bcdda33387b8bf15124bc316ef03b434433))
* The following workspace dependencies were updated
  * dependencies
    * @helia/interface bumped from ^4.1.0 to ^5.0.0
