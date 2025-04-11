## [1.1.3](https://github.com/SP-Packages/actions/compare/v1.1.2...v1.1.3) (2025-04-11)

### Bug Fixes

* **workflows:** update permissions for release and pr-labeler jobs ([56fbb14](https://github.com/SP-Packages/actions/commit/56fbb14f1d018c09f20d9fe0f1b21e711c7bf23c))

## [1.1.2](https://github.com/SP-Packages/actions/compare/v1.1.1...v1.1.2) (2025-04-01)

### Bug Fixes

* **workflows:** add check for dist directory before zipping ([3b530a9](https://github.com/SP-Packages/actions/commit/3b530a90dbf801d96ab8e829d07f48e8a86adb4d))
* **workflows:** remove PREPARE_DEST_DIR input and adjust build script ([9e55d59](https://github.com/SP-Packages/actions/commit/9e55d59cce4b89a809d3f26b9b2cb98c63445c8f))
* **workflows:** update condition for running build script ([12d3541](https://github.com/SP-Packages/actions/commit/12d354127e9d31fc1542e91c01ff5691e01a8fea))

## [1.1.1](https://github.com/SP-Packages/actions/compare/v1.1.0...v1.1.1) (2025-03-31)

### Bug Fixes

* **workflows:** set default value of PREPARE_DEST_DIR to true ([38d7925](https://github.com/SP-Packages/actions/commit/38d7925aa0f5dac39540a44d408d2fe3e13f6b99))

## [1.1.0](https://github.com/SP-Packages/actions/compare/v1.0.0...v1.1.0) (2025-03-31)

### Features

* **workflows:** refactor labeler workflow to use a separate file ([65c9aad](https://github.com/SP-Packages/actions/commit/65c9aad42b7449dff56c2e3fffb1c41b1efd3ab2))

## 1.0.0 (2025-03-31)

### Features

* **code-quality:** add flags for Codecov reporting in workflow ([b937c68](https://github.com/SP-Packages/actions/commit/b937c68209824c336be6376823e977145949d750))
* **code-quality:** add linting step to code quality workflow ([66627cf](https://github.com/SP-Packages/actions/commit/66627cf116690fbc1a6ac248704297ae3614f541))
* **code-quality:** add slug input to Codecov workflow configuration ([f23de62](https://github.com/SP-Packages/actions/commit/f23de6209352cd20cf183b03d3ebb1fc987b1ccf))
* **code-quality:** update permissions for code quality workflow ([6682ff6](https://github.com/SP-Packages/actions/commit/6682ff646b74d13e68c6855be9412b457528859e))
* **code-quality:** upgrade Codecov action to version 5 ([c6cb013](https://github.com/SP-Packages/actions/commit/c6cb01329f7cb5dd9b7f8ea84f4b63a159c6c746))
* **config:** add configuration files for linting and formatting ([e6e3543](https://github.com/SP-Packages/actions/commit/e6e3543da482b52610dad8bad9c20d0e8b32c260))
* **semantic-release:** add debug permissions step to workflow ([b6cd5b3](https://github.com/SP-Packages/actions/commit/b6cd5b312e9003b9f5900bded86f1cbc2d7f72ab))
* **semantic-release:** remove debug permissions step from workflow ([a106089](https://github.com/SP-Packages/actions/commit/a1060898bf57863ccf564380b3e65caf59eae814))
* **semantic-release:** update build script execution conditions ([4c4be82](https://github.com/SP-Packages/actions/commit/4c4be82a797f3d3c4abe0dfbcb368662b4d52b7d))
* **setup-environment:** add build script execution to workflow ([8568750](https://github.com/SP-Packages/actions/commit/85687503160a3a2c4e045150840ee7afac8925d4))
* **setup-environment:** add npm registry URL and zip dist folder ([1462529](https://github.com/SP-Packages/actions/commit/1462529d3da8ec3aa9694ee2559bf54bf316d2fc))
* **setup-environment:** change fetch depth to zero for full history ([123fd8b](https://github.com/SP-Packages/actions/commit/123fd8b5361040d84bad962cca93e1c5263a9a88))
* **setup-environment:** conditionally run build script based on inputs ([796eb2a](https://github.com/SP-Packages/actions/commit/796eb2af3950d57a22cb1e542c1c29e53ec7dee5))
* **setup-environment:** enhance inputs for flexibility and caching ([c79e490](https://github.com/SP-Packages/actions/commit/c79e490d778c6db4c637002d20d9e3d551986cd5))
* **setup-environment:** optimize npm caching and dependency installation ([7ec8d99](https://github.com/SP-Packages/actions/commit/7ec8d9941ac86c838dcfd4569d016d21092d7f10))
* **workflows:** add conditional build script execution in workflows ([6a786eb](https://github.com/SP-Packages/actions/commit/6a786ebeaf61d2ea54573b2e6011316cf7904e8a))
* **workflows:** add setup environment and code quality workflows ([754db3a](https://github.com/SP-Packages/actions/commit/754db3a7831ae03734f43b9f48c6065227112ee8))
* **workflows:** refactor code quality and testing workflow ([b7726b5](https://github.com/SP-Packages/actions/commit/b7726b56a1fad0042a33a76fe7f390fe79bd9ca5))

### Bug Fixes

* **release.config:** update repository URL for semantic release ([6cc903d](https://github.com/SP-Packages/actions/commit/6cc903d278e8add3ee530b42308887249e9738fb))
