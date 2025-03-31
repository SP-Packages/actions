# 🚀 GitHub Actions and Workflows

<p align="center">
<a href="https://github.com/SP-Packages/actions/actions"><img src="https://github.com/SP-Packages/actions/actions/workflows/release.yml/badge.svg" alt="build status"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="license"></a>
  <a href="https://github.com/semantic-release/semantic-release"><img src="https://img.shields.io/badge/semantic--release-conventionalcommits-e10079?logo=semantic-release" alt="semantic-release"></a>
  <a href="https://prettier.io/"><img src="https://img.shields.io/badge/code_style-prettier-ff69b4.svg" alt="Prettier"></a>
  <a href="https://github.com/SP-Packages/actions/pulls"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs welcome"></a>
  <a href="https://github.com/sponsors/iamsenthilprabu"><img src="https://img.shields.io/badge/Sponsor-%E2%9D%A4-pink?logo=github" alt="Sponsor"></a>
</p>

This repository provides a collection of **reusable workflows** and **composite actions** for GitHub Actions, designed to streamline CI/CD processes across multiple projects.

## 📦 Available Actions

### 🛠️ Setup Environment

Sets up the environment with Git, Node.js, and dependency management configurations.

| Input                      | Type      | Default | Required | Description                          |
| -------------------------- | --------- | ------- | -------- | ------------------------------------ |
| `FETCH_DEPTH`              | `number`  | `1`     | No       | Git fetch depth (0 for full history) |
| `SETUP_NODE`               | `boolean` | `false` | No       | Enable Node.js setup                 |
| `NODE_VERSION`             | `string`  | `21`    | No       | Node.js version                      |
| `CACHE_KEY_PREFIX`         | `string`  | `deps`  | No       | Cache key prefix                     |
| `INSTALL_DEPENDENCIES`     | `boolean` | `false` | No       | Install dependencies                 |
| `INSTALL_DEV_DEPENDENCIES` | `boolean` | `false` | No       | Install dev dependencies             |

## 🔄 Reusable Workflows

### 1. Code Quality 🧹

Executes code quality checks using `@sp-packages/lintrc`.

- Supports Node.js 18, 20, and 21
- Input: `VERBOSE` (boolean, default: false)

### 2. Code Testing 🧪

Runs tests and manages Codecov coverage reporting.

| Input/Secret    | Type     | Required | Description             |
| --------------- | -------- | -------- | ----------------------- |
| `SLUG`          | `string` | No       | Codecov repository slug |
| `CODECOV_TOKEN` | `secret` | No       | Codecov upload token    |

### 3. Rebase Develop 🔄

Automatically rebases `develop` onto `main` branch.

1. Git user configuration
2. Branch fetching
3. Rebase execution
4. Force push updates

### 4. Semantic Release 📦

Handles versioning and package publishing.

| Input/Secret       | Type      | Required | Description               |
| ------------------ | --------- | -------- | ------------------------- |
| `DRY_RUN`          | `boolean` | No       | Test mode                 |
| `PREPARE_DEST_DIR` | `boolean` | No       | Build and zip dist folder |
| `GH_TOKEN`         | `secret`  | Yes      | GitHub authentication     |
| `NPM_TOKEN`        | `secret`  | Yes      | NPM publishing access     |

## 📚 Usage Example

```yaml
jobs:
  quality:
    uses: SP-Packages/actions/.github/workflows/code-quality.yml@main
    with:
      VERBOSE: true
```

## 🤝 Contributing

Contributions are welcome! Please check our [Contributing Guidelines](CONTRIBUTING.md) before submitting issues or pull requests.

## 📜 License

Licensed under the [MIT License](LICENSE).
