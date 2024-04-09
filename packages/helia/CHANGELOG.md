# Changelog

## [5.0.0](https://github.com/SgtPooki/helia/compare/helia-v4.1.0...helia-v5.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* remove gossipsub from default libp2p services ([#401](https://github.com/SgtPooki/helia/issues/401))
* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* `helia.pin.add` and `helia.pin.rm` now return `AsyncGenerator<CID>`
* The libp2p API has changed in a couple of places - please see the [upgrade guide](https://github.com/libp2p/js-libp2p/blob/main/doc/migrations/v0.46-v1.0.0.md)
* libp2p has been updated to 0.46.x

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* add offline option to blockstore get ([#145](https://github.com/SgtPooki/helia/issues/145)) ([71c5f6b](https://github.com/SgtPooki/helia/commit/71c5f6bc32b324ee237e56c2c5a1ce903b3bdbef))
* allow passing partial libp2p config to helia factory ([#140](https://github.com/SgtPooki/helia/issues/140)) ([33a75d5](https://github.com/SgtPooki/helia/commit/33a75d5f80e2f211440c087806f463525de910d9))
* configurable block brokers ([#280](https://github.com/SgtPooki/helia/issues/280)) ([0749cbf](https://github.com/SgtPooki/helia/commit/0749cbf99745ea6ab4363f1b5d635634ca0ddcfa))
* expose .dns property on @helia/interface ([#465](https://github.com/SgtPooki/helia/issues/465)) ([8c9bb7d](https://github.com/SgtPooki/helia/commit/8c9bb7d224a1b786cba1fba18bffe07001a3b95d))
* GatewayBlockBroker prioritizes & tries all gateways ([#281](https://github.com/SgtPooki/helia/issues/281)) ([9bad21b](https://github.com/SgtPooki/helia/commit/9bad21bd59fe6d1ba4a137db5a46bd2ead5238c3))
* iterable pinning ([#231](https://github.com/SgtPooki/helia/issues/231)) ([c15c774](https://github.com/SgtPooki/helia/commit/c15c7749294d3d4aea5aef70544d088250336798))
* provide default libp2p instance ([#127](https://github.com/SgtPooki/helia/issues/127)) ([45c9d89](https://github.com/SgtPooki/helia/commit/45c9d896afa27f5ea043cc5f576d50fc4fa556e9)), closes [#121](https://github.com/SgtPooki/helia/issues/121)
* re-export types from @helia/interface ([#232](https://github.com/SgtPooki/helia/issues/232)) ([09c1e47](https://github.com/SgtPooki/helia/commit/09c1e4787a506d34a00d9ce7852d73471d47db1b))
* use trustless-gateway.link by default ([#299](https://github.com/SgtPooki/helia/issues/299)) ([bf11efa](https://github.com/SgtPooki/helia/commit/bf11efa4875f3b8f844511d70122983fc46b4f88))


### Bug Fixes

* add a test for reading the peer id from the datastore ([#397](https://github.com/SgtPooki/helia/issues/397)) ([4836d52](https://github.com/SgtPooki/helia/commit/4836d52bf721bc0c3e5920ebd0a05186fb19c6c6))
* add dag walker for json codec ([#247](https://github.com/SgtPooki/helia/issues/247)) ([5c4b570](https://github.com/SgtPooki/helia/commit/5c4b5709e6b98de5efc9bed388942e367f5874e7)), closes [#246](https://github.com/SgtPooki/helia/issues/246)
* add dht validators/selectors for ipns ([#135](https://github.com/SgtPooki/helia/issues/135)) ([2c8e6b5](https://github.com/SgtPooki/helia/commit/2c8e6b51b3c401a0472a024b8dac3d3ba735d74c))
* add helia version to agent version ([#128](https://github.com/SgtPooki/helia/issues/128)) ([48e19ec](https://github.com/SgtPooki/helia/commit/48e19ec545cc67157e14ae59054fa377a583cb01)), closes [#122](https://github.com/SgtPooki/helia/issues/122)
* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* create @helia/block-brokers package ([#341](https://github.com/SgtPooki/helia/issues/341)) ([#342](https://github.com/SgtPooki/helia/issues/342)) ([2979147](https://github.com/SgtPooki/helia/commit/297914756fa06dc0c28890a2654d1159d16689c2))
* dedupe bootstrap list ([#129](https://github.com/SgtPooki/helia/issues/129)) ([bb5d1e9](https://github.com/SgtPooki/helia/commit/bb5d1e91daae9f6c399e0fdf974318a4a7353fb9))
* enable dcutr by default ([#239](https://github.com/SgtPooki/helia/issues/239)) ([7431f09](https://github.com/SgtPooki/helia/commit/7431f09aef332dc142a5f7c2c59c9410e4529a92))
* ensure pinned blocks are present ([#141](https://github.com/SgtPooki/helia/issues/141)) ([271c403](https://github.com/SgtPooki/helia/commit/271c403009d378a35375a9468e41388ebb978f54))
* export libp2p service return type ([#263](https://github.com/SgtPooki/helia/issues/263)) ([76769cf](https://github.com/SgtPooki/helia/commit/76769cf33e06746f998b4f16b52d3e2a6a7a20a8))
* helia init should extend base helia init ([#464](https://github.com/SgtPooki/helia/issues/464)) ([a64e5de](https://github.com/SgtPooki/helia/commit/a64e5de937fbbade035657a18e07bcad4de0a53f))
* ignore libp2p start param in helia factory ([#382](https://github.com/SgtPooki/helia/issues/382)) ([c8d2fac](https://github.com/SgtPooki/helia/commit/c8d2fac002ef73fc3eba83914de12d2e73074c64)), closes [#344](https://github.com/SgtPooki/helia/issues/344)
* listen on ip6 addresses ([#271](https://github.com/SgtPooki/helia/issues/271)) ([7ef5e79](https://github.com/SgtPooki/helia/commit/7ef5e79620f043522ff0dacc260af1fe83e5d77e))
* pass options to blockstore.get during pin.add ([#148](https://github.com/SgtPooki/helia/issues/148)) ([3a5234e](https://github.com/SgtPooki/helia/commit/3a5234e3c2f88f9910678b0cbbac5fd340117cc9))
* remove extra interface ([d577c61](https://github.com/SgtPooki/helia/commit/d577c61bcc6e4805d214b3ec4a39d78ee752a21e))
* remove gossipsub from default libp2p services ([#401](https://github.com/SgtPooki/helia/issues/401)) ([99c94f4](https://github.com/SgtPooki/helia/commit/99c94f4b85c4ed826a6195207e3545cbbc87a6d1))
* remove trustless-gateway.link ([#301](https://github.com/SgtPooki/helia/issues/301)) ([0343725](https://github.com/SgtPooki/helia/commit/03437255213b14f5931aed91e8555d7fb7f92926))
* replace IPNI gateway with delegated routing client ([#297](https://github.com/SgtPooki/helia/issues/297)) ([57d580d](https://github.com/SgtPooki/helia/commit/57d580da26c5e28852cc9fe4d0d80adb36699ece))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* try circuit relay transport first ([#267](https://github.com/SgtPooki/helia/issues/267)) ([d5e9c3c](https://github.com/SgtPooki/helia/commit/d5e9c3c45c8dc3e63969105b785f6a836820a1f8))
* **types:** Add missing types ([#95](https://github.com/SgtPooki/helia/issues/95)) ([e858b8d](https://github.com/SgtPooki/helia/commit/e858b8dbbff548b42dde225db674f0edd1990ed3))
* update attempt to add helia to identify agent version ([#268](https://github.com/SgtPooki/helia/issues/268)) ([6dc7d55](https://github.com/SgtPooki/helia/commit/6dc7d55cd3099785417a7a2c99db755e856bd59a))
* update ipns module to v9 and fix double verification of records ([#396](https://github.com/SgtPooki/helia/issues/396)) ([f2853f8](https://github.com/SgtPooki/helia/commit/f2853f8bd5bdcee8ab7a685355b0be47f29620e0))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use release version of libp2p ([#59](https://github.com/SgtPooki/helia/issues/59)) ([a3a7c9c](https://github.com/SgtPooki/helia/commit/a3a7c9c2d81f2068fee85eeeca7425919f09e182))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))
* update generated docs to include version in module names ([#296](https://github.com/SgtPooki/helia/issues/296)) ([0776106](https://github.com/SgtPooki/helia/commit/0776106710d6641ac82b446f7fde6c40d788a0b4))


### Dependencies

* bump @chainsafe/libp2p-noise from 14.1.0 to 15.0.0 ([#393](https://github.com/SgtPooki/helia/issues/393)) ([4943c5b](https://github.com/SgtPooki/helia/commit/4943c5b7e8779bc326ee156b1d80152225189343))
* bump @libp2p/ipni-content-routing from 1.0.2 to 2.0.0 ([#227](https://github.com/SgtPooki/helia/issues/227)) ([a33cb3e](https://github.com/SgtPooki/helia/commit/a33cb3ef2dd21a55b598f206e8d4295935ea2bcc))
* bump cborg from 2.0.5 to 4.0.1 ([#260](https://github.com/SgtPooki/helia/issues/260)) ([230b15b](https://github.com/SgtPooki/helia/commit/230b15b7aa1c5403abdeed81710c7d6d0862f041))
* bump ipns from 6.0.7 to 7.0.1 ([#266](https://github.com/SgtPooki/helia/issues/266)) ([373a22c](https://github.com/SgtPooki/helia/commit/373a22c342401f7ad8b85d5f082d66934eddaa70))
* bump it-all from 2.0.1 to 3.0.1 ([#72](https://github.com/SgtPooki/helia/issues/72)) ([e7ce5bc](https://github.com/SgtPooki/helia/commit/e7ce5bc0e0db0a6b41920a3c36b95eeea1863183))
* bump it-drain from 2.0.1 to 3.0.1 ([#71](https://github.com/SgtPooki/helia/issues/71)) ([c6eaca1](https://github.com/SgtPooki/helia/commit/c6eaca1d21cf16527851fffc2411a8e3bd651f34))
* bump it-filter from 2.0.2 to 3.0.1 ([#74](https://github.com/SgtPooki/helia/issues/74)) ([3402724](https://github.com/SgtPooki/helia/commit/340272484df47d2f70f870d375ebb4235fb165a0))
* bump it-foreach from 1.0.1 to 2.0.2 ([#75](https://github.com/SgtPooki/helia/issues/75)) ([6f5f059](https://github.com/SgtPooki/helia/commit/6f5f0592edd44257092d0b70dd364096864495bf))
* bump multiformats from 12.1.3 to 13.0.0 ([#354](https://github.com/SgtPooki/helia/issues/354)) ([1d16bf8](https://github.com/SgtPooki/helia/commit/1d16bf89acd10ac79baf53f0cbc5f92d0e9d8301))
* bump uint8arrays from 4.0.10 to 5.0.0 ([#339](https://github.com/SgtPooki/helia/issues/339)) ([299bb09](https://github.com/SgtPooki/helia/commit/299bb0942bbfae492db938c4ccad4e835bab2dbd))
* **dev:** bump aegir from 39.0.13 to 40.0.8 ([#198](https://github.com/SgtPooki/helia/issues/198)) ([4d75ecf](https://github.com/SgtPooki/helia/commit/4d75ecffb79e5177da35d3106e42dac7bc63153a))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#273](https://github.com/SgtPooki/helia/issues/273)) ([9a9f637](https://github.com/SgtPooki/helia/commit/9a9f63787223eff7eae3b72e59b79b11baa621ea))
* **dev:** bump delay from 5.0.0 to 6.0.0 ([#130](https://github.com/SgtPooki/helia/issues/130)) ([d087ffc](https://github.com/SgtPooki/helia/commit/d087ffcb8074b41781346d09101b2b7bc64768d2))
* **dev:** bump libp2p from 0.43.4 to 0.44.0 ([#96](https://github.com/SgtPooki/helia/issues/96)) ([6e37d9f](https://github.com/SgtPooki/helia/commit/6e37d9f8be58955c5ddc5472fe3adb4bd9a0459c))
* **dev:** bump sinon from 15.2.0 to 16.0.0 ([#262](https://github.com/SgtPooki/helia/issues/262)) ([fb3081a](https://github.com/SgtPooki/helia/commit/fb3081adc3e6cfcb16ff0b11f340848b7568863b))
* **dev:** bump sinon from 16.1.3 to 17.0.0 ([#288](https://github.com/SgtPooki/helia/issues/288)) ([ecdb46e](https://github.com/SgtPooki/helia/commit/ecdb46e0d40df86a59e58fcdfb701db6e36d36e6))
* **dev:** bump sinon-ts from 1.0.2 to 2.0.0 ([#298](https://github.com/SgtPooki/helia/issues/298)) ([dbbee17](https://github.com/SgtPooki/helia/commit/dbbee17959c0a737f196c468eb06cc055bbc9711))
* update interface-store to 5.x.x ([#63](https://github.com/SgtPooki/helia/issues/63)) ([5bf11d6](https://github.com/SgtPooki/helia/commit/5bf11d638eee423624ac49af97757d730744f384))
* update libp2p patch versions ([917a1bc](https://github.com/SgtPooki/helia/commit/917a1bceb9e9b56428a15dc3377a963f06affd12))
* update libp2p to 0.46.x ([#215](https://github.com/SgtPooki/helia/issues/215)) ([65b68f0](https://github.com/SgtPooki/helia/commit/65b68f071d04d2f6f0fcf35938b146706b1a3cd0))
* update sibling dependencies ([07847bb](https://github.com/SgtPooki/helia/commit/07847bb60b9ebd26497080373e45871abb4b82dd))
* update sibling dependencies ([beb10b5](https://github.com/SgtPooki/helia/commit/beb10b5590d66d1d5bef9b5e890b888263df2c92))
* update sibling dependencies ([aa249bc](https://github.com/SgtPooki/helia/commit/aa249bca021ca513c7847331970219e4a36dee97))
* update sibling dependencies ([89df3fe](https://github.com/SgtPooki/helia/commit/89df3fe803daa3228290bef105ce5d0b769dc3a0))
* update sibling dependencies ([0970da7](https://github.com/SgtPooki/helia/commit/0970da79e974a4c172e8fdfb7c207d5ba8152a83))
* update sibling dependencies ([5850e51](https://github.com/SgtPooki/helia/commit/5850e513c486f6d20e23c04936bbf843653cb5e4))
* update sibling dependencies ([2c52da3](https://github.com/SgtPooki/helia/commit/2c52da3957d56fe4e3ff6f161f9bec814abd5d8c))
* update sibling dependencies ([9139f30](https://github.com/SgtPooki/helia/commit/9139f30e857f4e247202e0d113027190a04892ba))
* update sibling dependencies ([99a5115](https://github.com/SgtPooki/helia/commit/99a5115713d2f17f17820f661dd22a87262c654b))
* update sibling dependencies ([64e300c](https://github.com/SgtPooki/helia/commit/64e300c289f4bfe4b72607d86ab9e83a1ac3c8d3))
* update sibling dependencies ([f7cb076](https://github.com/SgtPooki/helia/commit/f7cb076e9356535164812229eff22c5c0e052674))
* update sibling dependencies ([634ca4f](https://github.com/SgtPooki/helia/commit/634ca4faf5caf448bd068a78101ac0070145518e))
* update sibling dependencies ([3323a5c](https://github.com/SgtPooki/helia/commit/3323a5cd518c63cb67e8eaef0cb64c542982b603))
* update sibling dependencies ([671ec87](https://github.com/SgtPooki/helia/commit/671ec874e90fbdcaf79d9d8253822fd85cee8bc5))
* update sibling dependencies ([a349576](https://github.com/SgtPooki/helia/commit/a34957650715efc45382dc005feea6162398b8f9))
* update sibling dependencies ([fcee11e](https://github.com/SgtPooki/helia/commit/fcee11eadb7edfa327e3f0bd586e20ea5dc06c8a))
* update sibling dependencies ([c936ba6](https://github.com/SgtPooki/helia/commit/c936ba63a75276e206d804cf0ef35c3f9bf67f10))
* update sibling dependencies ([f565ffd](https://github.com/SgtPooki/helia/commit/f565ffdcf6923b78326ed4cb00be93083b45ccca))
* update sibling dependencies ([1ac389c](https://github.com/SgtPooki/helia/commit/1ac389c6fd8f276daf33c8a61849f3657cf88a10))
* update sibling dependencies ([ed49856](https://github.com/SgtPooki/helia/commit/ed4985677b62021f76541354ad06b70bd53e929a))
* update sibling dependencies ([d33c843](https://github.com/SgtPooki/helia/commit/d33c84378c02f34277178e6553090b92b0eabe0b))
* update sibling dependencies ([ac28d38](https://github.com/SgtPooki/helia/commit/ac28d3878f98a780fc57702921924fa92bd592a0))
* updates to libp2p v1 ([#320](https://github.com/SgtPooki/helia/issues/320)) ([635d7a2](https://github.com/SgtPooki/helia/commit/635d7a2938111ccc53f8defbd9b8f8f8ea3e8e6a))
## [5.0.0](https://github.com/SgtPooki/helia/compare/helia-v4.1.0...helia-v5.0.0) (2024-04-09)


### ⚠ BREAKING CHANGES

* remove gossipsub from default libp2p services ([#401](https://github.com/SgtPooki/helia/issues/401))
* the `libp2p` property has been removed from the `Helia` interface in `@helia/interface` - it is still present on the return type of `createHelia` from the `helia` module
* `helia.pin.add` and `helia.pin.rm` now return `AsyncGenerator<CID>`
* The libp2p API has changed in a couple of places - please see the [upgrade guide](https://github.com/libp2p/js-libp2p/blob/main/doc/migrations/v0.46-v1.0.0.md)
* libp2p has been updated to 0.46.x

### Features

* add @helia/http to monorepo ([#372](https://github.com/SgtPooki/helia/issues/372)) ([76220cd](https://github.com/SgtPooki/helia/commit/76220cd5adf45af7fa61fd0a1321de4722b744d6))
* add offline option to blockstore get ([#145](https://github.com/SgtPooki/helia/issues/145)) ([71c5f6b](https://github.com/SgtPooki/helia/commit/71c5f6bc32b324ee237e56c2c5a1ce903b3bdbef))
* allow passing partial libp2p config to helia factory ([#140](https://github.com/SgtPooki/helia/issues/140)) ([33a75d5](https://github.com/SgtPooki/helia/commit/33a75d5f80e2f211440c087806f463525de910d9))
* configurable block brokers ([#280](https://github.com/SgtPooki/helia/issues/280)) ([0749cbf](https://github.com/SgtPooki/helia/commit/0749cbf99745ea6ab4363f1b5d635634ca0ddcfa))
* expose .dns property on @helia/interface ([#465](https://github.com/SgtPooki/helia/issues/465)) ([8c9bb7d](https://github.com/SgtPooki/helia/commit/8c9bb7d224a1b786cba1fba18bffe07001a3b95d))
* GatewayBlockBroker prioritizes & tries all gateways ([#281](https://github.com/SgtPooki/helia/issues/281)) ([9bad21b](https://github.com/SgtPooki/helia/commit/9bad21bd59fe6d1ba4a137db5a46bd2ead5238c3))
* iterable pinning ([#231](https://github.com/SgtPooki/helia/issues/231)) ([c15c774](https://github.com/SgtPooki/helia/commit/c15c7749294d3d4aea5aef70544d088250336798))
* provide default libp2p instance ([#127](https://github.com/SgtPooki/helia/issues/127)) ([45c9d89](https://github.com/SgtPooki/helia/commit/45c9d896afa27f5ea043cc5f576d50fc4fa556e9)), closes [#121](https://github.com/SgtPooki/helia/issues/121)
* re-export types from @helia/interface ([#232](https://github.com/SgtPooki/helia/issues/232)) ([09c1e47](https://github.com/SgtPooki/helia/commit/09c1e4787a506d34a00d9ce7852d73471d47db1b))
* use trustless-gateway.link by default ([#299](https://github.com/SgtPooki/helia/issues/299)) ([bf11efa](https://github.com/SgtPooki/helia/commit/bf11efa4875f3b8f844511d70122983fc46b4f88))


### Bug Fixes

* add a test for reading the peer id from the datastore ([#397](https://github.com/SgtPooki/helia/issues/397)) ([4836d52](https://github.com/SgtPooki/helia/commit/4836d52bf721bc0c3e5920ebd0a05186fb19c6c6))
* add dag walker for json codec ([#247](https://github.com/SgtPooki/helia/issues/247)) ([5c4b570](https://github.com/SgtPooki/helia/commit/5c4b5709e6b98de5efc9bed388942e367f5874e7)), closes [#246](https://github.com/SgtPooki/helia/issues/246)
* add dht validators/selectors for ipns ([#135](https://github.com/SgtPooki/helia/issues/135)) ([2c8e6b5](https://github.com/SgtPooki/helia/commit/2c8e6b51b3c401a0472a024b8dac3d3ba735d74c))
* add helia version to agent version ([#128](https://github.com/SgtPooki/helia/issues/128)) ([48e19ec](https://github.com/SgtPooki/helia/commit/48e19ec545cc67157e14ae59054fa377a583cb01)), closes [#122](https://github.com/SgtPooki/helia/issues/122)
* add sideEffects: false to package.json ([#485](https://github.com/SgtPooki/helia/issues/485)) ([8c45267](https://github.com/SgtPooki/helia/commit/8c45267a474ab10b2faadfebdab33cfe446e8c03))
* create @helia/block-brokers package ([#341](https://github.com/SgtPooki/helia/issues/341)) ([#342](https://github.com/SgtPooki/helia/issues/342)) ([2979147](https://github.com/SgtPooki/helia/commit/297914756fa06dc0c28890a2654d1159d16689c2))
* dedupe bootstrap list ([#129](https://github.com/SgtPooki/helia/issues/129)) ([bb5d1e9](https://github.com/SgtPooki/helia/commit/bb5d1e91daae9f6c399e0fdf974318a4a7353fb9))
* enable dcutr by default ([#239](https://github.com/SgtPooki/helia/issues/239)) ([7431f09](https://github.com/SgtPooki/helia/commit/7431f09aef332dc142a5f7c2c59c9410e4529a92))
* ensure pinned blocks are present ([#141](https://github.com/SgtPooki/helia/issues/141)) ([271c403](https://github.com/SgtPooki/helia/commit/271c403009d378a35375a9468e41388ebb978f54))
* export libp2p service return type ([#263](https://github.com/SgtPooki/helia/issues/263)) ([76769cf](https://github.com/SgtPooki/helia/commit/76769cf33e06746f998b4f16b52d3e2a6a7a20a8))
* helia init should extend base helia init ([#464](https://github.com/SgtPooki/helia/issues/464)) ([a64e5de](https://github.com/SgtPooki/helia/commit/a64e5de937fbbade035657a18e07bcad4de0a53f))
* ignore libp2p start param in helia factory ([#382](https://github.com/SgtPooki/helia/issues/382)) ([c8d2fac](https://github.com/SgtPooki/helia/commit/c8d2fac002ef73fc3eba83914de12d2e73074c64)), closes [#344](https://github.com/SgtPooki/helia/issues/344)
* listen on ip6 addresses ([#271](https://github.com/SgtPooki/helia/issues/271)) ([7ef5e79](https://github.com/SgtPooki/helia/commit/7ef5e79620f043522ff0dacc260af1fe83e5d77e))
* pass options to blockstore.get during pin.add ([#148](https://github.com/SgtPooki/helia/issues/148)) ([3a5234e](https://github.com/SgtPooki/helia/commit/3a5234e3c2f88f9910678b0cbbac5fd340117cc9))
* remove extra interface ([d577c61](https://github.com/SgtPooki/helia/commit/d577c61bcc6e4805d214b3ec4a39d78ee752a21e))
* remove gossipsub from default libp2p services ([#401](https://github.com/SgtPooki/helia/issues/401)) ([99c94f4](https://github.com/SgtPooki/helia/commit/99c94f4b85c4ed826a6195207e3545cbbc87a6d1))
* remove trustless-gateway.link ([#301](https://github.com/SgtPooki/helia/issues/301)) ([0343725](https://github.com/SgtPooki/helia/commit/03437255213b14f5931aed91e8555d7fb7f92926))
* replace IPNI gateway with delegated routing client ([#297](https://github.com/SgtPooki/helia/issues/297)) ([57d580d](https://github.com/SgtPooki/helia/commit/57d580da26c5e28852cc9fe4d0d80adb36699ece))
* support reading identity cids ([#429](https://github.com/SgtPooki/helia/issues/429)) ([98308f7](https://github.com/SgtPooki/helia/commit/98308f77488b8196b2d18f78f05ecd2d37456834))
* try circuit relay transport first ([#267](https://github.com/SgtPooki/helia/issues/267)) ([d5e9c3c](https://github.com/SgtPooki/helia/commit/d5e9c3c45c8dc3e63969105b785f6a836820a1f8))
* **types:** Add missing types ([#95](https://github.com/SgtPooki/helia/issues/95)) ([e858b8d](https://github.com/SgtPooki/helia/commit/e858b8dbbff548b42dde225db674f0edd1990ed3))
* update attempt to add helia to identify agent version ([#268](https://github.com/SgtPooki/helia/issues/268)) ([6dc7d55](https://github.com/SgtPooki/helia/commit/6dc7d55cd3099785417a7a2c99db755e856bd59a))
* update ipns module to v9 and fix double verification of records ([#396](https://github.com/SgtPooki/helia/issues/396)) ([f2853f8](https://github.com/SgtPooki/helia/commit/f2853f8bd5bdcee8ab7a685355b0be47f29620e0))
* update project deps and docs ([77e34fc](https://github.com/SgtPooki/helia/commit/77e34fc115cbfb82585fd954bcf389ecebf655bc))
* use release version of libp2p ([#59](https://github.com/SgtPooki/helia/issues/59)) ([a3a7c9c](https://github.com/SgtPooki/helia/commit/a3a7c9c2d81f2068fee85eeeca7425919f09e182))


### Documentation

* fixing changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* merge [#1](https://github.com/SgtPooki/helia/issues/1) from SgtPooki/docs/fixing-changelogs ([9e7caa1](https://github.com/SgtPooki/helia/commit/9e7caa10e85a00b41482c4165f2d83d39668e46d))
* rm changelog to try to generate new ones ([71c0821](https://github.com/SgtPooki/helia/commit/71c0821d43e725961cd381070c0dc37846e305fe))
* update generated docs to include version in module names ([#296](https://github.com/SgtPooki/helia/issues/296)) ([0776106](https://github.com/SgtPooki/helia/commit/0776106710d6641ac82b446f7fde6c40d788a0b4))


### Dependencies

* bump @chainsafe/libp2p-noise from 14.1.0 to 15.0.0 ([#393](https://github.com/SgtPooki/helia/issues/393)) ([4943c5b](https://github.com/SgtPooki/helia/commit/4943c5b7e8779bc326ee156b1d80152225189343))
* bump @libp2p/ipni-content-routing from 1.0.2 to 2.0.0 ([#227](https://github.com/SgtPooki/helia/issues/227)) ([a33cb3e](https://github.com/SgtPooki/helia/commit/a33cb3ef2dd21a55b598f206e8d4295935ea2bcc))
* bump cborg from 2.0.5 to 4.0.1 ([#260](https://github.com/SgtPooki/helia/issues/260)) ([230b15b](https://github.com/SgtPooki/helia/commit/230b15b7aa1c5403abdeed81710c7d6d0862f041))
* bump ipns from 6.0.7 to 7.0.1 ([#266](https://github.com/SgtPooki/helia/issues/266)) ([373a22c](https://github.com/SgtPooki/helia/commit/373a22c342401f7ad8b85d5f082d66934eddaa70))
* bump it-all from 2.0.1 to 3.0.1 ([#72](https://github.com/SgtPooki/helia/issues/72)) ([e7ce5bc](https://github.com/SgtPooki/helia/commit/e7ce5bc0e0db0a6b41920a3c36b95eeea1863183))
* bump it-drain from 2.0.1 to 3.0.1 ([#71](https://github.com/SgtPooki/helia/issues/71)) ([c6eaca1](https://github.com/SgtPooki/helia/commit/c6eaca1d21cf16527851fffc2411a8e3bd651f34))
* bump it-filter from 2.0.2 to 3.0.1 ([#74](https://github.com/SgtPooki/helia/issues/74)) ([3402724](https://github.com/SgtPooki/helia/commit/340272484df47d2f70f870d375ebb4235fb165a0))
* bump it-foreach from 1.0.1 to 2.0.2 ([#75](https://github.com/SgtPooki/helia/issues/75)) ([6f5f059](https://github.com/SgtPooki/helia/commit/6f5f0592edd44257092d0b70dd364096864495bf))
* bump multiformats from 12.1.3 to 13.0.0 ([#354](https://github.com/SgtPooki/helia/issues/354)) ([1d16bf8](https://github.com/SgtPooki/helia/commit/1d16bf89acd10ac79baf53f0cbc5f92d0e9d8301))
* bump uint8arrays from 4.0.10 to 5.0.0 ([#339](https://github.com/SgtPooki/helia/issues/339)) ([299bb09](https://github.com/SgtPooki/helia/commit/299bb0942bbfae492db938c4ccad4e835bab2dbd))
* **dev:** bump aegir from 39.0.13 to 40.0.8 ([#198](https://github.com/SgtPooki/helia/issues/198)) ([4d75ecf](https://github.com/SgtPooki/helia/commit/4d75ecffb79e5177da35d3106e42dac7bc63153a))
* **dev:** bump aegir from 40.0.13 to 41.0.0 ([#273](https://github.com/SgtPooki/helia/issues/273)) ([9a9f637](https://github.com/SgtPooki/helia/commit/9a9f63787223eff7eae3b72e59b79b11baa621ea))
* **dev:** bump delay from 5.0.0 to 6.0.0 ([#130](https://github.com/SgtPooki/helia/issues/130)) ([d087ffc](https://github.com/SgtPooki/helia/commit/d087ffcb8074b41781346d09101b2b7bc64768d2))
* **dev:** bump libp2p from 0.43.4 to 0.44.0 ([#96](https://github.com/SgtPooki/helia/issues/96)) ([6e37d9f](https://github.com/SgtPooki/helia/commit/6e37d9f8be58955c5ddc5472fe3adb4bd9a0459c))
* **dev:** bump sinon from 15.2.0 to 16.0.0 ([#262](https://github.com/SgtPooki/helia/issues/262)) ([fb3081a](https://github.com/SgtPooki/helia/commit/fb3081adc3e6cfcb16ff0b11f340848b7568863b))
* **dev:** bump sinon from 16.1.3 to 17.0.0 ([#288](https://github.com/SgtPooki/helia/issues/288)) ([ecdb46e](https://github.com/SgtPooki/helia/commit/ecdb46e0d40df86a59e58fcdfb701db6e36d36e6))
* **dev:** bump sinon-ts from 1.0.2 to 2.0.0 ([#298](https://github.com/SgtPooki/helia/issues/298)) ([dbbee17](https://github.com/SgtPooki/helia/commit/dbbee17959c0a737f196c468eb06cc055bbc9711))
* update interface-store to 5.x.x ([#63](https://github.com/SgtPooki/helia/issues/63)) ([5bf11d6](https://github.com/SgtPooki/helia/commit/5bf11d638eee423624ac49af97757d730744f384))
* update libp2p patch versions ([917a1bc](https://github.com/SgtPooki/helia/commit/917a1bceb9e9b56428a15dc3377a963f06affd12))
* update libp2p to 0.46.x ([#215](https://github.com/SgtPooki/helia/issues/215)) ([65b68f0](https://github.com/SgtPooki/helia/commit/65b68f071d04d2f6f0fcf35938b146706b1a3cd0))
* update sibling dependencies ([07847bb](https://github.com/SgtPooki/helia/commit/07847bb60b9ebd26497080373e45871abb4b82dd))
* update sibling dependencies ([beb10b5](https://github.com/SgtPooki/helia/commit/beb10b5590d66d1d5bef9b5e890b888263df2c92))
* update sibling dependencies ([aa249bc](https://github.com/SgtPooki/helia/commit/aa249bca021ca513c7847331970219e4a36dee97))
* update sibling dependencies ([89df3fe](https://github.com/SgtPooki/helia/commit/89df3fe803daa3228290bef105ce5d0b769dc3a0))
* update sibling dependencies ([0970da7](https://github.com/SgtPooki/helia/commit/0970da79e974a4c172e8fdfb7c207d5ba8152a83))
* update sibling dependencies ([5850e51](https://github.com/SgtPooki/helia/commit/5850e513c486f6d20e23c04936bbf843653cb5e4))
* update sibling dependencies ([2c52da3](https://github.com/SgtPooki/helia/commit/2c52da3957d56fe4e3ff6f161f9bec814abd5d8c))
* update sibling dependencies ([9139f30](https://github.com/SgtPooki/helia/commit/9139f30e857f4e247202e0d113027190a04892ba))
* update sibling dependencies ([99a5115](https://github.com/SgtPooki/helia/commit/99a5115713d2f17f17820f661dd22a87262c654b))
* update sibling dependencies ([64e300c](https://github.com/SgtPooki/helia/commit/64e300c289f4bfe4b72607d86ab9e83a1ac3c8d3))
* update sibling dependencies ([f7cb076](https://github.com/SgtPooki/helia/commit/f7cb076e9356535164812229eff22c5c0e052674))
* update sibling dependencies ([634ca4f](https://github.com/SgtPooki/helia/commit/634ca4faf5caf448bd068a78101ac0070145518e))
* update sibling dependencies ([3323a5c](https://github.com/SgtPooki/helia/commit/3323a5cd518c63cb67e8eaef0cb64c542982b603))
* update sibling dependencies ([671ec87](https://github.com/SgtPooki/helia/commit/671ec874e90fbdcaf79d9d8253822fd85cee8bc5))
* update sibling dependencies ([a349576](https://github.com/SgtPooki/helia/commit/a34957650715efc45382dc005feea6162398b8f9))
* update sibling dependencies ([fcee11e](https://github.com/SgtPooki/helia/commit/fcee11eadb7edfa327e3f0bd586e20ea5dc06c8a))
* update sibling dependencies ([c936ba6](https://github.com/SgtPooki/helia/commit/c936ba63a75276e206d804cf0ef35c3f9bf67f10))
* update sibling dependencies ([f565ffd](https://github.com/SgtPooki/helia/commit/f565ffdcf6923b78326ed4cb00be93083b45ccca))
* update sibling dependencies ([1ac389c](https://github.com/SgtPooki/helia/commit/1ac389c6fd8f276daf33c8a61849f3657cf88a10))
* update sibling dependencies ([ed49856](https://github.com/SgtPooki/helia/commit/ed4985677b62021f76541354ad06b70bd53e929a))
* update sibling dependencies ([d33c843](https://github.com/SgtPooki/helia/commit/d33c84378c02f34277178e6553090b92b0eabe0b))
* update sibling dependencies ([ac28d38](https://github.com/SgtPooki/helia/commit/ac28d3878f98a780fc57702921924fa92bd592a0))
* updates to libp2p v1 ([#320](https://github.com/SgtPooki/helia/issues/320)) ([635d7a2](https://github.com/SgtPooki/helia/commit/635d7a2938111ccc53f8defbd9b8f8f8ea3e8e6a))


### Refactors

* use functions for block broker creation ([#286](https://github.com/SgtPooki/helia/issues/286)) ([43932a5](https://github.com/SgtPooki/helia/commit/43932a54036dafdf1265b034b30b12784fd22d82))


### Refactors

* use functions for block broker creation ([#286](https://github.com/SgtPooki/helia/issues/286)) ([43932a5](https://github.com/SgtPooki/helia/commit/43932a54036dafdf1265b034b30b12784fd22d82))
