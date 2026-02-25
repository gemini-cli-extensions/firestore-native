# Changelog

## [0.2.0](https://github.com/gemini-cli-extensions/firestore-native/compare/0.1.2...0.2.0) (2026-02-25)


### ⚠ BREAKING CHANGES

* Update/add detailed telemetry for mcp endpoint compliant with OTEL semantic convention ([genai-toolbox#​1987](https://redirect.github.com/googleapis/genai-toolbox/issues/1987)) ([478a0bd](https://redirect.github.com/googleapis/genai-toolbox/commit/478a0bdb59288c1213f83862f95a698b4c2c0aab))
* Update configuration file v2 ([genai-toolbox#​2369](https://redirect.github.com/googleapis/genai-toolbox/issues/2369))([293c1d6](https://redirect.github.com/googleapis/genai-toolbox/commit/293c1d6889c39807855ba5e01d4c13ba2a4c50ce))

### Features

* **cli/invoke:** Add support for direct tool invocation from CLI ([genai-toolbox#​2353](https://redirect.github.com/googleapis/genai-toolbox/issues/2353)) ([6e49ba4](https://redirect.github.com/googleapis/genai-toolbox/commit/6e49ba436ef2390c13feaf902b29f5907acffb57)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **cli/skills:** Add support for generating agent skills from toolset ([genai-toolbox#​2392](https://redirect.github.com/googleapis/genai-toolbox/issues/2392)) ([80ef346](https://redirect.github.com/googleapis/genai-toolbox/commit/80ef34621453b77bdf6a6016c354f102a17ada04)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **cloud-logging-admin:** Add source, tools, integration test and docs ([genai-toolbox#​2137](https://redirect.github.com/googleapis/genai-toolbox/issues/2137)) ([252fc30](https://redirect.github.com/googleapis/genai-toolbox/commit/252fc3091af10d25d8d7af7e047b5ac87a5dd041)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **cockroachdb:** Add CockroachDB integration with cockroach-go ([genai-toolbox#​2006](https://redirect.github.com/googleapis/genai-toolbox/issues/2006)) ([1fdd99a](https://redirect.github.com/googleapis/genai-toolbox/commit/1fdd99a9b609a5e906acce414226ff44d75d5975)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **prebuiltconfigs/alloydb-omni:** Implement Alloydb omni dataplane tools ([genai-toolbox#​2340](https://redirect.github.com/googleapis/genai-toolbox/issues/2340)) ([e995349](https://redirect.github.com/googleapis/genai-toolbox/commit/e995349ea0756c700d188b8f04e9459121219f0c)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* **server:** Add Tool call error categories ([genai-toolbox#​2387](https://redirect.github.com/googleapis/genai-toolbox/issues/2387)) ([32cb4db](https://redirect.github.com/googleapis/genai-toolbox/commit/32cb4db712d27579c1bf29e61cbd0bed02286c28)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* Update configuration file v2 ([genai-toolbox#​2369](https://redirect.github.com/googleapis/genai-toolbox/issues/2369))([293c1d6](https://redirect.github.com/googleapis/genai-toolbox/commit/293c1d6889c39807855ba5e01d4c13ba2a4c50ce)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* Update/add detailed telemetry for mcp endpoint compliant with OTEL semantic convention ([genai-toolbox#​1987](https://redirect.github.com/googleapis/genai-toolbox/issues/1987)) ([478a0bd](https://redirect.github.com/googleapis/genai-toolbox/commit/478a0bdb59288c1213f83862f95a698b4c2c0aab)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))


### Bug Fixes

* **dataplex:** Capture GCP HTTP errors in MCP Toolbox ([genai-toolbox#​2347](https://redirect.github.com/googleapis/genai-toolbox/issues/2347)) ([1d7c498](https://redirect.github.com/googleapis/genai-toolbox/commit/1d7c4981164c34b4d7bc8edecfd449f57ad11e15)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))
* Surface Dataplex API errors in MCP results ([genai-toolbox#​2347](https://redirect.github.com/googleapis/genai-toolbox/pull/2347))([1d7c498](https://redirect.github.com/googleapis/genai-toolbox/commit/1d7c4981164c34b4d7bc8edecfd449f57ad11e15)) ([6d9c082](https://github.com/gemini-cli-extensions/firestore-native/commit/6d9c0820c044b9a3ca70679f75ed7c6876417902))

## [0.1.2](https://github.com/gemini-cli-extensions/firestore-native/compare/0.1.1...0.1.2) (2026-01-29)


### Features

* add clarifying note to setting ([#75](https://github.com/gemini-cli-extensions/firestore-native/issues/75)) ([a4d30bd](https://github.com/gemini-cli-extensions/firestore-native/commit/a4d30bdbc85dad0a04376f583a4b86010b7b5329))
* add Configuration settings ([#71](https://github.com/gemini-cli-extensions/firestore-native/issues/71)) ([ca34ac9](https://github.com/gemini-cli-extensions/firestore-native/commit/ca34ac97889f333d4e8c5a4e9e083209724b613f))
* **deps:** update dependency googleapis/genai-toolbox to v0.25.0 ([#68](https://github.com/gemini-cli-extensions/firestore-native/issues/68)) ([b71762a](https://github.com/gemini-cli-extensions/firestore-native/commit/b71762a544b3ca2f5df91f3769563ce30cf08de6))
* **deps:** update dependency googleapis/genai-toolbox to v0.26.0 ([#73](https://github.com/gemini-cli-extensions/firestore-native/issues/73)) ([06d94ca](https://github.com/gemini-cli-extensions/firestore-native/commit/06d94caad952d03dc83a7a3658408aeb506d28ca))

## [0.1.1](https://github.com/gemini-cli-extensions/firestore-native/compare/0.1.0...0.1.1) (2025-09-30)


### Features

* additional instructions for the context file ([#29](https://github.com/gemini-cli-extensions/firestore-native/issues/29)) ([5433cff](https://github.com/gemini-cli-extensions/firestore-native/commit/5433cff45f707993684204ecc2433eafcc816041))
* standardize mcp server names ([#27](https://github.com/gemini-cli-extensions/firestore-native/issues/27)) ([a4e7d86](https://github.com/gemini-cli-extensions/firestore-native/commit/a4e7d862ee32c08cd176b31ed7b6f13e0e7acf91))

## 0.1.0 (2025-09-21)


### Features

* add Firestore Native Extension ([#11](https://github.com/gemini-cli-extensions/firestore-native/issues/11)) ([facc0dd](https://github.com/gemini-cli-extensions/firestore-native/commit/facc0dd8840e95082c940290b227ddefa2b280fa))
