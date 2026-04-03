# Changelog

## [0.2.1](https://github.com/gemini-cli-extensions/firestore-native/compare/0.2.0...0.2.1) (2026-03-03)


### Features

* **dataproc:** Add dataproc source and list/get clusters/jobs tools ([mcp-toolbox#​2407](https://redirect.github.com/googleapis/mcp-toolbox/issues/2407)) ([cc05e57](https://redirect.github.com/googleapis/mcp-toolbox/commit/cc05e5745d1c25a6088702b827cd098250164b7e)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **ui:** Make tool list panel resizable ([mcp-toolbox#​2253](https://redirect.github.com/googleapis/mcp-toolbox/issues/2253)) ([276cf60](https://redirect.github.com/googleapis/mcp-toolbox/commit/276cf604a2bb41861639ed6881557e38dd97a614)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* Add polling system to dynamic reloading ([mcp-toolbox#​2466](https://redirect.github.com/googleapis/mcp-toolbox/issues/2466)) ([fcaac9b](https://redirect.github.com/googleapis/mcp-toolbox/commit/fcaac9bb957226ee3db1baea24330f337ba88ab7)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* Added basic template for sdks doc migrate ([mcp-toolbox#​1961](https://redirect.github.com/googleapis/mcp-toolbox/issues/1961)) ([87f2eaf](https://redirect.github.com/googleapis/mcp-toolbox/commit/87f2eaf79cdecca7b939151e1543eccf2f812a69)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))


### Bug Fixes

* **ci:** Add path for forked PR unit test runs ([mcp-toolbox#​2540](https://redirect.github.com/googleapis/mcp-toolbox/issues/2540)) ([04dd2a7](https://redirect.github.com/googleapis/mcp-toolbox/commit/04dd2a77603c7babf01da724dfb77808e3f25fe5)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **docs/adk:** Resolve dependency duplication ([mcp-toolbox#​2418](https://redirect.github.com/googleapis/mcp-toolbox/issues/2418)) ([4d44abb](https://redirect.github.com/googleapis/mcp-toolbox/commit/4d44abb4638926ca50b0fa4dcf10a03e7fab657f)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **docs/langchain:** Fix core at 0.3.0 and align compatible dependencies ([mcp-toolbox#​2426](https://redirect.github.com/googleapis/mcp-toolbox/issues/2426)) ([36edfd3](https://redirect.github.com/googleapis/mcp-toolbox/commit/36edfd3d506e839c092d04cbca1799b5ebc38160)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **oracle:** Enable DML operations and resolve incorrect array type error ([mcp-toolbox#​2323](https://redirect.github.com/googleapis/mcp-toolbox/issues/2323)) ([72146a4](https://redirect.github.com/googleapis/mcp-toolbox/commit/72146a4b1605bcdd3e1038106bfb1f899e677e39)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **server/mcp:** Guard nil dereference in sseManager.get ([mcp-toolbox#​2557](https://redirect.github.com/googleapis/mcp-toolbox/issues/2557)) ([e534196](https://redirect.github.com/googleapis/mcp-toolbox/commit/e534196303c2b8d9b6e599ac25add337e6fc9b8f)), closes [mcp-toolbox#​2548](https://redirect.github.com/googleapis/mcp-toolbox/issues/2548) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **tests:** Resolve LlamaIndex dependency conflict in JS quickstart ([mcp-toolbox#​2597](https://redirect.github.com/googleapis/mcp-toolbox/issues/2597)) ([ac11f5a](https://redirect.github.com/googleapis/mcp-toolbox/commit/ac11f5af9c7bcf228d667e1b8e08b5dc49ad91a0)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **tests/postgres:** Implement uuid-based isolation and reliable resource cleanup ([mcp-toolbox#​2377](https://redirect.github.com/googleapis/mcp-toolbox/issues/2377)) ([8a96fb1](https://redirect.github.com/googleapis/mcp-toolbox/commit/8a96fb1a8874baa3688e566f3dea8a0912fcf2df)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* **tests/postgres:** Restore list\_schemas test and implement dynamic owner ([mcp-toolbox#​2521](https://redirect.github.com/googleapis/mcp-toolbox/issues/2521)) ([7041e79](https://redirect.github.com/googleapis/mcp-toolbox/commit/7041e797347f337d6f7f44ca051ae31acd58babe)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* Deflake alloydb omni ([mcp-toolbox#​2431](https://redirect.github.com/googleapis/mcp-toolbox/issues/2431)) ([62b8309](https://redirect.github.com/googleapis/mcp-toolbox/commit/62b830987d65c3573214d04e50742476097ee9e9)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))
* Enforce required validation for explicit null parameter values ([mcp-toolbox#​2519](https://redirect.github.com/googleapis/mcp-toolbox/issues/2519)) ([d5e9512](https://redirect.github.com/googleapis/mcp-toolbox/commit/d5e9512a237e658f9b9127fdd8c174ec023c3310)) ([9495d0e](https://github.com/gemini-cli-extensions/firestore-native/commit/9495d0e8752714f979a3796775f89ad03bf3a828))

## [0.2.0](https://github.com/gemini-cli-extensions/firestore-native/compare/0.1.2...0.2.0) (2026-02-25)


### ⚠ BREAKING CHANGES

* Update/add detailed telemetry for mcp endpoint compliant with OTEL semantic convention ([mcp-toolbox#​1987](https://redirect.github.com/googleapis/mcp-toolbox/issues/1987)) ([478a0bd](https://redirect.github.com/googleapis/mcp-toolbox/commit/478a0bdb59288c1213f83862f95a698b4c2c0aab))
* Update configuration file v2 ([mcp-toolbox#​2369](https://redirect.github.com/googleapis/mcp-toolbox/issues/2369))([293c1d6](https://redirect.github.com/googleapis/mcp-toolbox/commit/293c1d6889c39807855ba5e01d4c13ba2a4c50ce))

### Features

* **cli/invoke:** Add support for direct tool invocation from CLI ([mcp-toolbox#​2353](https://redirect.github.com/googleapis/mcp-toolbox/issues/2353)) ([6e49ba4](https://redirect.github.com/googleapis/mcp-toolbox/commit/6e49ba436ef2390c13feaf902b29f5907acffb57)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **cli/skills:** Add support for generating agent skills from toolset ([mcp-toolbox#​2392](https://redirect.github.com/googleapis/mcp-toolbox/issues/2392)) ([80ef346](https://redirect.github.com/googleapis/mcp-toolbox/commit/80ef34621453b77bdf6a6016c354f102a17ada04)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **cloud-logging-admin:** Add source, tools, integration test and docs ([mcp-toolbox#​2137](https://redirect.github.com/googleapis/mcp-toolbox/issues/2137)) ([252fc30](https://redirect.github.com/googleapis/mcp-toolbox/commit/252fc3091af10d25d8d7af7e047b5ac87a5dd041)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **cockroachdb:** Add CockroachDB integration with cockroach-go ([mcp-toolbox#​2006](https://redirect.github.com/googleapis/mcp-toolbox/issues/2006)) ([1fdd99a](https://redirect.github.com/googleapis/mcp-toolbox/commit/1fdd99a9b609a5e906acce414226ff44d75d5975)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **prebuiltconfigs/alloydb-omni:** Implement Alloydb omni dataplane tools ([mcp-toolbox#​2340](https://redirect.github.com/googleapis/mcp-toolbox/issues/2340)) ([e995349](https://redirect.github.com/googleapis/mcp-toolbox/commit/e995349ea0756c700d188b8f04e9459121219f0c)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **server:** Add Tool call error categories ([mcp-toolbox#​2387](https://redirect.github.com/googleapis/mcp-toolbox/issues/2387)) ([32cb4db](https://redirect.github.com/googleapis/mcp-toolbox/commit/32cb4db712d27579c1bf29e61cbd0bed02286c28)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* Update configuration file v2 ([mcp-toolbox#​2369](https://redirect.github.com/googleapis/mcp-toolbox/issues/2369))([293c1d6](https://redirect.github.com/googleapis/mcp-toolbox/commit/293c1d6889c39807855ba5e01d4c13ba2a4c50ce)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* Update/add detailed telemetry for mcp endpoint compliant with OTEL semantic convention ([mcp-toolbox#​1987](https://redirect.github.com/googleapis/mcp-toolbox/issues/1987)) ([478a0bd](https://redirect.github.com/googleapis/mcp-toolbox/commit/478a0bdb59288c1213f83862f95a698b4c2c0aab)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))


### Bug Fixes

* **dataplex:** Capture GCP HTTP errors in MCP Toolbox ([mcp-toolbox#​2347](https://redirect.github.com/googleapis/mcp-toolbox/issues/2347)) ([1d7c498](https://redirect.github.com/googleapis/mcp-toolbox/commit/1d7c4981164c34b4d7bc8edecfd449f57ad11e15)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* Surface Dataplex API errors in MCP results ([mcp-toolbox#​2347](https://redirect.github.com/googleapis/mcp-toolbox/pull/2347))([1d7c498](https://redirect.github.com/googleapis/mcp-toolbox/commit/1d7c4981164c34b4d7bc8edecfd449f57ad11e15)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))

## [0.1.2](https://github.com/gemini-cli-extensions/firestore-native/compare/0.1.1...0.1.2) (2026-01-29)


### Features

* add clarifying note to setting ([#75](https://github.com/gemini-cli-extensions/firestore-native/issues/75)) ([a4d30bd](https://github.com/gemini-cli-extensions/firestore-native/commit/a4d30bdbc85dad0a04376f583a4b86010b7b5329))
* add Configuration settings ([#71](https://github.com/gemini-cli-extensions/firestore-native/issues/71)) ([ca34ac9](https://github.com/gemini-cli-extensions/firestore-native/commit/ca34ac97889f333d4e8c5a4e9e083209724b613f))
* **deps:** update dependency googleapis/mcp-toolbox to v0.25.0 ([#68](https://github.com/gemini-cli-extensions/firestore-native/issues/68)) ([b71762a](https://github.com/gemini-cli-extensions/firestore-native/commit/b71762a544b3ca2f5df91f3769563ce30cf08de6))
* **deps:** update dependency googleapis/mcp-toolbox to v0.26.0 ([#73](https://github.com/gemini-cli-extensions/firestore-native/issues/73)) ([06d94ca](https://github.com/gemini-cli-extensions/firestore-native/commit/06d94caad952d03dc83a7a3658408aeb506d28ca))

## [0.1.1](https://github.com/gemini-cli-extensions/firestore-native/compare/0.1.0...0.1.1) (2025-09-30)


### Features

* additional instructions for the context file ([#29](https://github.com/gemini-cli-extensions/firestore-native/issues/29)) ([5433cff](https://github.com/gemini-cli-extensions/firestore-native/commit/5433cff45f707993684204ecc2433eafcc816041))
* standardize mcp server names ([#27](https://github.com/gemini-cli-extensions/firestore-native/issues/27)) ([a4e7d86](https://github.com/gemini-cli-extensions/firestore-native/commit/a4e7d862ee32c08cd176b31ed7b6f13e0e7acf91))

## 0.1.0 (2025-09-21)


### Features

* add Firestore Native Extension ([#11](https://github.com/gemini-cli-extensions/firestore-native/issues/11)) ([facc0dd](https://github.com/gemini-cli-extensions/firestore-native/commit/facc0dd8840e95082c940290b227ddefa2b280fa))
