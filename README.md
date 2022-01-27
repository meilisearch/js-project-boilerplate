<p align="center">
  <img src="https://raw.githubusercontent.com/meilisearch/integration-guides/main/assets/logos/meilisearch_js.svg" alt="Meilisearch" width="200" height="200" />
</p>

<h1 align="center">JavaScript project boilerplate</h1>

<h4 align="center">
  <a href="https://github.com/meilisearch/meilisearch">Meilisearch</a> |
  <a href="https://docs.meilisearch.com">Documentation</a> |
  <a href="https://slack.meilisearch.com">Slack</a> |
  <a href="https://www.meilisearch.com">Website</a> |
  <a href="https://docs.meilisearch.com/faq">FAQ</a>
</h4>

<p align="center">
  <a href="https://app.bors.tech/repositories/34942"><img src="https://bors.tech/images/badge_small.svg" alt="Bors enabled"></a>
    <a href="https://github.com/meilisearch/js-project-boilerplate/actions"><img src="https://github.com/meilisearch/js-project-boilerplate/workflows/Tests/badge.svg" alt="Tests"></a>
  <a href="https://github.com/meilisearch/js-project-boilerplate/blob/main/LICENCE"><img src="https://img.shields.io/badge/license-MIT-informational" alt="License"></a>
</p>
<br/>

<p align="center" style="font-weight:bold;" >A boilerplate to start a JavaScript project</p>
<p align="center">The boilerplate provides the base needs we require from every JavaScript project</p>

<br/>

To start your project, clone this repository and remove git from it. After which, you can create a new GitHub project that starts with this base.

## Table of Contents

- [✨ Linter](#-linter)
- [🔧 Github Actions](#-github-actions)
- [🙈 gitignore](#-gitignore)
- [📄 License](#-license)
- [🖇 bors](#-bors)
- [🎳 Editor Config](#-editor-config)
- [⚠️ Project Settings](#-project-settings)

## ✨ Linter

JavaScript project follow linting and format rules.

The linting rules are applied by [`eslint`](https://github.com/eslint/eslint), we follow their [recommended rules](https://eslint.org/docs/rules/).

The formatting is provided by [`prettier`](https://github.com/prettier/prettier).

To check if your code is well linted, you can use the following command:

```
yarn lint
```

To fix and format your code, you can use the following command:

```
yarn lint:fix
```

## 🔧 Github Actions

In the `.github` the following GitHub actions are present:

- Templates suggesting formatting of issues in the repository (`ISSUE_TEMPLATE`)
- A release drafter that will automatically update your GitHub release body with the merged PR's.
- Tests that will run on each PR. It only tests the linting in this project, but you should add more jobs.
- A `dependabot` configuration to determine when and how `dependabot` suggests package updates. The configuration should not change unless it was decided.

## 🙈 gitignore

The `.gitignore` ignores the most frequent directories and file naming that should not be pushed to GitHub. It should be updated accordingly to your needs.

## 📄 License

The licensing file contains the license Meilisearch used across our projects. The years should be updated accordingly to the current year.

### 🖇 Bors

A testing and merging tool used to merge PR's. Please refer to [this documentation](https://github.com/meilisearch/integration-guides/blob/main/guides/bors.md).

### 🎳 Editor Config

An `.editorconfig` file that follows some style rules used accros all JavaScript projects.

### ⚠️ Project Settings


What this boilerplate does not provide are the repositories settings that should be manually configurated:
<br>

⚠️ Entering the settings should be done after consultation with the person in charge ⚠️

- Project access management.
- Enable dependabot security alerts, updates and graph.
- Main branch protection.
- Add project in bors.
