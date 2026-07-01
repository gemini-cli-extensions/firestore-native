# Changelog

## [0.3.3](https://github.com/gemini-cli-extensions/firestore-native/compare/0.3.2...0.3.3) (2026-07-01)


### Features

* **release:** Add digital signature to Toolbox binaries ([mcp-toolbox#​3528](https://redirect.github.com/googleapis/mcp-toolbox/issues/3528)) ([3f0f0af](https://redirect.github.com/googleapis/mcp-toolbox/commit/3f0f0af29007929b01e95ee2caef4fd2015d5f12)) ([6023cc5](https://github.com/gemini-cli-extensions/firestore-native/commit/6023cc546e03ec1e489b1960d232063294403c38))
* Support MCP 2026 draft specs ([mcp-toolbox#​3544](https://redirect.github.com/googleapis/mcp-toolbox/issues/3544)) ([d12eaa8](https://redirect.github.com/googleapis/mcp-toolbox/commit/d12eaa856bad70b49ba2b7b9f2882cffbf81220f)) ([6023cc5](https://github.com/gemini-cli-extensions/firestore-native/commit/6023cc546e03ec1e489b1960d232063294403c38))

## [0.3.2](https://github.com/gemini-cli-extensions/firestore-native/compare/0.3.1...0.3.2) (2026-06-22)


### Features

* **auth/google:** Require audience or clientId for mcpEnabled ([mcp-toolbox#​3450](https://redirect.github.com/googleapis/mcp-toolbox/issues/3450)) ([59f7b6e](https://redirect.github.com/googleapis/mcp-toolbox/commit/59f7b6e8eaceffca042cb7e2f2b6e5e9284b6bc3)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **mcp:** Add URL parameter binding for HTTP transport ([mcp-toolbox#​3112](https://redirect.github.com/googleapis/mcp-toolbox/issues/3112)) ([0cc7b37](https://redirect.github.com/googleapis/mcp-toolbox/commit/0cc7b37b733b6a99dad5281af4024b26d730106a)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **scylladb:** Adding support for ScyllaDB source and tool ([mcp-toolbox#​3119](https://redirect.github.com/googleapis/mcp-toolbox/issues/3119)) ([2dada83](https://redirect.github.com/googleapis/mcp-toolbox/commit/2dada8306c8737e445c4f8cd3d213b72713c1834)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **server:** Add support for toolset filtering in prebuilt CLI flag ([mcp-toolbox#​3245](https://redirect.github.com/googleapis/mcp-toolbox/issues/3245)) ([7cc4f65](https://redirect.github.com/googleapis/mcp-toolbox/commit/7cc4f65a8e767e0da37cf21f0ff2568b38d32b8e)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **skills:** Generate skills offline without live source connections ([mcp-toolbox#​3388](https://redirect.github.com/googleapis/mcp-toolbox/issues/3388)) ([4c860b6](https://redirect.github.com/googleapis/mcp-toolbox/commit/4c860b66b03f0ebf86205e73cd8521ad90ccebe4)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **skills:** Tolerate missing env vars during offline skills-generate ([mcp-toolbox#​3399](https://redirect.github.com/googleapis/mcp-toolbox/issues/3399)) ([ea5d3e5](https://redirect.github.com/googleapis/mcp-toolbox/commit/ea5d3e5b9e60bf808e10d21b522954d76f7741b6)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **tools:** Decouple tool initialization from sources ([mcp-toolbox#​3355](https://redirect.github.com/googleapis/mcp-toolbox/issues/3355)) ([32a24e3](https://redirect.github.com/googleapis/mcp-toolbox/commit/32a24e35b5bf107bcf5e89af2a9b7af3740747ee)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* Enable per source level flags for sql commenter ([mcp-toolbox#​3465](https://redirect.github.com/googleapis/mcp-toolbox/issues/3465)) ([ecce6b7](https://redirect.github.com/googleapis/mcp-toolbox/commit/ecce6b7bb551b947b0951cd684cce627a4b6cf1b)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))


### Bug Fixes

* **auth/dataplex:** Fix failing source with service account credentials ([mcp-toolbox#​3369](https://redirect.github.com/googleapis/mcp-toolbox/issues/3369)) ([ba4deef](https://redirect.github.com/googleapis/mcp-toolbox/commit/ba4deef140358e5876d73d355d664f629f7aeccc)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **bigquery:** Wire maximumBytesBilled into prebuilt config ([mcp-toolbox#​3385](https://redirect.github.com/googleapis/mcp-toolbox/issues/3385)) ([4abbf6e](https://redirect.github.com/googleapis/mcp-toolbox/commit/4abbf6e82cc4af4c1903d9143337c965987475a9)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **config:** Add doc/line context to parse errors ([mcp-toolbox#​2957](https://redirect.github.com/googleapis/mcp-toolbox/issues/2957)) ([4b097da](https://redirect.github.com/googleapis/mcp-toolbox/commit/4b097daa2143817e55a9e557e8c1dea054bfc7b8)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **npm:** Source binary version from cmd/version.txt ([mcp-toolbox#​3417](https://redirect.github.com/googleapis/mcp-toolbox/issues/3417)) ([6ffbdec](https://redirect.github.com/googleapis/mcp-toolbox/commit/6ffbdecaea98db5c16dc9eeca8fb73e4bbc48102)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **prebuilt/alloydb-omni:** Require password env var explicitly ([mcp-toolbox#​3398](https://redirect.github.com/googleapis/mcp-toolbox/issues/3398)) ([fcbe3e7](https://redirect.github.com/googleapis/mcp-toolbox/commit/fcbe3e70d3d4e671e97e424187dba907d7c5b10b)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **server:** Fail if MCP auth is enabled together with enable-api ([mcp-toolbox#​3435](https://redirect.github.com/googleapis/mcp-toolbox/issues/3435)) ([a6ff910](https://redirect.github.com/googleapis/mcp-toolbox/commit/a6ff910a602adece11f0a6581d6211e5927f7182)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* **server:** Return errors instead of panicking in InitializeConfigs ([mcp-toolbox#​3397](https://redirect.github.com/googleapis/mcp-toolbox/issues/3397)) ([f48b01d](https://redirect.github.com/googleapis/mcp-toolbox/commit/f48b01dc1775e4583a06689a2e67fb06e5dd3c68)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* Bound MCP HTTP body size ([mcp-toolbox#​3216](https://redirect.github.com/googleapis/mcp-toolbox/issues/3216)) ([d4f4342](https://redirect.github.com/googleapis/mcp-toolbox/commit/d4f434251392fb597779a90a12c63d21533ea187)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))
* Escape delimiter characters in applyEscape to prevent SQL injection ([mcp-toolbox#​2811](https://redirect.github.com/googleapis/mcp-toolbox/issues/2811)) ([932519a](https://redirect.github.com/googleapis/mcp-toolbox/commit/932519a9551861bf5f18787dc43b20d06350343f)) ([f7b99cf](https://github.com/gemini-cli-extensions/firestore-native/commit/f7b99cfd5dd3e99901a24df3df1ef48b29df0717))

## [0.3.1](https://github.com/gemini-cli-extensions/firestore-native/compare/0.3.0...0.3.1) (2026-06-12)


### Features

* **auth:** Implement MCP auth tool-level scopes validation ([mcp-toolbox#​3049](https://redirect.github.com/googleapis/mcp-toolbox/issues/3049)) ([c528985](https://redirect.github.com/googleapis/mcp-toolbox/commit/c528985149060adb648f85b5486391bd72d6727e)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* **ci:** Add support for windows/arm64 binary distribution ([mcp-toolbox#​3231](https://redirect.github.com/googleapis/mcp-toolbox/issues/3231)) ([10abf3b](https://redirect.github.com/googleapis/mcp-toolbox/commit/10abf3b9e195a03f535e3807b7df9883899ef7c0)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **datalineage:** Add Data Lineage integration ([mcp-toolbox#​3285](https://redirect.github.com/googleapis/mcp-toolbox/issues/3285)) ([19353c3](https://redirect.github.com/googleapis/mcp-toolbox/commit/19353c37e17ab1f3599cafa04337a32a7baec1c3)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **looker:** Propagate client IP from incoming MCP requests to downstream SDK calls ([mcp-toolbox#​3253](https://redirect.github.com/googleapis/mcp-toolbox/issues/3253)) ([75da6c2](https://redirect.github.com/googleapis/mcp-toolbox/commit/75da6c21dd29d7e8e70eac1b747e3946097e7459)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* **server:** Ignore unknown tools at startup with `--ignore-unknown-tools` flag ([mcp-toolbox#​3353](https://redirect.github.com/googleapis/mcp-toolbox/issues/3353)) ([5f0304f](https://redirect.github.com/googleapis/mcp-toolbox/commit/5f0304f71231cce322ab2a3e458af07b392a06fc)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* Add support for HTTPS/TLS listener ([mcp-toolbox#​3126](https://redirect.github.com/googleapis/mcp-toolbox/issues/3126)) ([8bc385d](https://redirect.github.com/googleapis/mcp-toolbox/commit/8bc385d7d6fd9ed2ad13503d9feb503de0b512b1)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* Setup SQLCommenter and allow client metadata  ([mcp-toolbox#​3064](https://redirect.github.com/googleapis/mcp-toolbox/issues/3064)) ([9f1f9b3](https://redirect.github.com/googleapis/mcp-toolbox/commit/9f1f9b321dcd05cce55dbff1bbaebfc44a4c9907)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))


### Bug Fixes

* **auth:** Separate Google and Generic MCP OAuth verification ([mcp-toolbox#​3341](https://redirect.github.com/googleapis/mcp-toolbox/issues/3341)) ([dfd66ee](https://redirect.github.com/googleapis/mcp-toolbox/commit/dfd66ee7de6fe9750d932d30bf3b67a2f4d2a176)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **auth/generic:** Enforce issuer presence in opaque token validation ([mcp-toolbox#​3360](https://redirect.github.com/googleapis/mcp-toolbox/issues/3360)) ([1d8df0d](https://redirect.github.com/googleapis/mcp-toolbox/commit/1d8df0df590383ba56091b6e4d7c37ab7d7d9749)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **auth/generic:** Fix generic auth expiration field and integration with `authRequired` ([mcp-toolbox#​3251](https://redirect.github.com/googleapis/mcp-toolbox/issues/3251)) ([f4d16c0](https://redirect.github.com/googleapis/mcp-toolbox/commit/f4d16c09b12c4d3297a9aedca706c9830382a4e3)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* **mcp:** Implement router-level logger injection for MCP auth ([mcp-toolbox#​3067](https://redirect.github.com/googleapis/mcp-toolbox/issues/3067)) ([ccc7cf5](https://redirect.github.com/googleapis/mcp-toolbox/commit/ccc7cf5ee8a1bacb6b57faf41ae5a1cc3da5299e)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* **mcp:** Support annotations and metadata within Tools to earlier MCP schemas ([mcp-toolbox#​3300](https://redirect.github.com/googleapis/mcp-toolbox/issues/3300)) ([9a88c72](https://redirect.github.com/googleapis/mcp-toolbox/commit/9a88c72792563e4868c82a4f3be55e6af25c1477)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **oracle:** Remove trailing semicolons from prebuilt tools ([mcp-toolbox#​3215](https://redirect.github.com/googleapis/mcp-toolbox/issues/3215)) ([fcad02d](https://redirect.github.com/googleapis/mcp-toolbox/commit/fcad02de73ffe9c6ecf29572f0f92674aacbe493)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **server:** Return null id for batch request rejection ([mcp-toolbox#​3333](https://redirect.github.com/googleapis/mcp-toolbox/issues/3333)) ([0b18d58](https://redirect.github.com/googleapis/mcp-toolbox/commit/0b18d58aea131baceb1c70f300879de8ecdf569e)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **server/auth:** Centralize tool scopes validation ([mcp-toolbox#​3335](https://redirect.github.com/googleapis/mcp-toolbox/issues/3335)) ([adce4ab](https://redirect.github.com/googleapis/mcp-toolbox/commit/adce4abb27327aae4e9736581df7a544b55c939e)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **telemetry:** Allow GCP project override ([mcp-toolbox#​2960](https://redirect.github.com/googleapis/mcp-toolbox/issues/2960)) ([3c83ba5](https://redirect.github.com/googleapis/mcp-toolbox/commit/3c83ba5ab1d2ab38369e0b5c47396fabf6ecabef)) ([d7f4242](https://github.com/gemini-cli-extensions/firestore-native/commit/d7f42424cfddfb567efbae100023b94dfb4571be))
* **tools:** Initialize query result slices to empty array ([mcp-toolbox#​3250](https://redirect.github.com/googleapis/mcp-toolbox/issues/3250)) ([60ddf48](https://redirect.github.com/googleapis/mcp-toolbox/commit/60ddf487468bfd11c7f9346f16a33a8986f89f84)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* Allow converting string literal block with list ([mcp-toolbox#​3050](https://redirect.github.com/googleapis/mcp-toolbox/issues/3050)) ([36ab2a9](https://redirect.github.com/googleapis/mcp-toolbox/commit/36ab2a98f9f2d03c27eea389d2281bfc4581ffa1)), closes [mcp-toolbox#​3023](https://redirect.github.com/googleapis/mcp-toolbox/issues/3023) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* Prevent test.db from being created during unit tests ([mcp-toolbox#​3042](https://redirect.github.com/googleapis/mcp-toolbox/issues/3042)) ([d10d2ca](https://redirect.github.com/googleapis/mcp-toolbox/commit/d10d2caeb7c9eda7d17d6dbd9f63363b2bc23a7a)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))
* Remove hardcoded \* allowed origin for sse ([mcp-toolbox#​3054](https://redirect.github.com/googleapis/mcp-toolbox/issues/3054)) ([c4c7bd9](https://redirect.github.com/googleapis/mcp-toolbox/commit/c4c7bd917e686de68e2be866cfe3872c3439efae)) ([0291742](https://github.com/gemini-cli-extensions/firestore-native/commit/02917420f4f69b3b5f91a1f76fdd9d94e8c3dbaf))

## [0.3.0](https://github.com/gemini-cli-extensions/firestore-native/compare/0.2.1...0.3.0) (2026-04-16)


### ⚠ BREAKING CHANGES

* add support for skills ([#105](https://github.com/gemini-cli-extensions/firestore-native/issues/105)) ([da51057](https://github.com/gemini-cli-extensions/firestore-native/commit/da51057d4ccf454a0336b46d36f61e230dbeeb6f))
* **firestore:** restructure prebuilt toolsets ([mcp-toolbox#​2636](https://redirect.github.com/googleapis/mcp-toolbox/issues/2636))
* update repo name ([mcp-toolbox#​2968](https://redirect.github.com/googleapis/mcp-toolbox/issues/2968))

### Features

* **skill:** Attach user agent metadata for generated skill ([mcp-toolbox#​2697](https://redirect.github.com/googleapis/mcp-toolbox/issues/2697)) ([9598a6a](https://redirect.github.com/googleapis/mcp-toolbox/commit/9598a6a32597b9c9abdb0f20c06d86a01b0d011f)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skill:** Update skill generation logic ([mcp-toolbox#​2646](https://redirect.github.com/googleapis/mcp-toolbox/issues/2646)) ([c233eee](https://redirect.github.com/googleapis/mcp-toolbox/commit/c233eee98cd9621526cb286245f3874f5bd6e7da)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e)) ([mcp-toolbox#​2733](https://redirect.github.com/googleapis/mcp-toolbox/issues/2733)) ([5b85c65](https://redirect.github.com/googleapis/mcp-toolbox/commit/5b85c65960dba9bfaf4cadca6d44532a153976e1)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skills:** Add Claude Code support to generated scripts ([mcp-toolbox#​2966](https://redirect.github.com/googleapis/mcp-toolbox/issues/2966)) ([a1609e1](https://redirect.github.com/googleapis/mcp-toolbox/commit/a1609e10a2eaf4ea68eae36acec3eed355b8a052)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skills:** Add codex user agent ([mcp-toolbox#​2973](https://redirect.github.com/googleapis/mcp-toolbox/issues/2973)) ([070e939](https://redirect.github.com/googleapis/mcp-toolbox/commit/070e9399c02f088d43175ce6bf343378beb7f584)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skills:** Tool invocation via npx ([mcp-toolbox#​2916](https://redirect.github.com/googleapis/mcp-toolbox/issues/2916)) ([377dc5b](https://redirect.github.com/googleapis/mcp-toolbox/commit/377dc5b00145a0044eef39314dd6b0ef5966fcd7)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* add Claude code plugin config ([#107](https://github.com/gemini-cli-extensions/firestore-native/issues/107)) ([f616fb1](https://github.com/gemini-cli-extensions/firestore-native/commit/f616fb103fc8a5020379c8d0d39eb0f823ee5efe))
* add Codex plugin config ([#108](https://github.com/gemini-cli-extensions/firestore-native/issues/108)) ([cf4506c](https://github.com/gemini-cli-extensions/firestore-native/commit/cf4506cc198f5b2169c17debd892a85d74c7cf0d))


### Bug Fixes

* **skill:** Fix env variable propagation ([mcp-toolbox#​2645](https://redirect.github.com/googleapis/mcp-toolbox/issues/2645)) ([5271368](https://redirect.github.com/googleapis/mcp-toolbox/commit/52713687208994c423da64333cb0a04fb483f794)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skills:** Fix integer parameter parsing through agent skills ([mcp-toolbox#​2847](https://redirect.github.com/googleapis/mcp-toolbox/issues/2847)) ([4564efe](https://redirect.github.com/googleapis/mcp-toolbox/commit/4564efe75436b4081d9f3d1f7c912bc64c13f850)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skills:** Fix skill generation template ([mcp-toolbox#​2914](https://redirect.github.com/googleapis/mcp-toolbox/issues/2914)) ([a01a15e](https://redirect.github.com/googleapis/mcp-toolbox/commit/a01a15ed1aa9a83eda8362578fed2e3a3c8dde99)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skills:** Improve flag validation and silence unit test output ([mcp-toolbox#​2759](https://redirect.github.com/googleapis/mcp-toolbox/issues/2759)) ([f3da6aa](https://redirect.github.com/googleapis/mcp-toolbox/commit/f3da6aa5e23b609a1ac9ecc098bccea02f2388ab)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))
* **skills:** Prevent empty strings overriding optional env vars in node scripts ([mcp-toolbox#​2963](https://redirect.github.com/googleapis/mcp-toolbox/issues/2963)) ([c52adeb](https://redirect.github.com/googleapis/mcp-toolbox/commit/c52adeba76fc13d0e6e415f6393def0648e478d6)) ([ac552d0](https://github.com/gemini-cli-extensions/firestore-native/commit/ac552d0702430782ab452dbd8f29f9f8532b645e))

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
