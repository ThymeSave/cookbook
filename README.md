Cookbook
===
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
[![pre-commit](https://img.shields.io/badge/%E2%9A%93%20%20pre--commit-enabled-success)](https://pre-commit.com/)

Documentation for everything around ThymeSave.

# Development

## Required tools

- Python 3
- pip3

## Setup

To set up the project locally:

1. Install dependencies: `pip3 install -r requirements.txt`
2. Serve documentation: `mkdocs serve`

## Commit Message Convention

This repository follows [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

### Format

`<type>(optional scope): <description>`
Example: `feat(pre-event): Add speakers section`

### 1. Type

Available types are:

- feat → Changes about addition or removal of a feature. Ex: `feat: Add table on landing page`
  , `feat: Remove table from landing page`
- fix → Bug fixing, followed by the bug. Ex: `fix: Illustration overflows in mobile view`
- docs → Update documentation (README.md)
- style → Updating style, and not changing any logic in the code (reorder imports, fix whitespace, remove comments)
- chore → Installing new dependencies, or bumping deps
- refactor → Changes in code, same output, but different approach
- ci → Update github workflows, husky
- test → Update testing suite, cypress files
- revert → when reverting commits
- perf → Fixing something regarding performance (deriving state, using memo, callback)
- vercel → Blank commit to trigger vercel deployment. Ex: `vercel: Trigger deployment`

### 2. Optional Scope

Labels per page Ex: `feat(pre-event): Add date label`

*If there is no scope needed, you don't need to write it*

### 3. Description

Description must fully explain what is being done.

Add BREAKING CHANGE in the description if there is a significant change.

**If there are multiple changes, then commit one by one**

- After colon, there are a single space Ex: `feat: Add something`
- When using `fix` type, state the issue Ex: `fix: File size limiter not working`
- Use imperative, dan present tense: "change" not "changed" or "changes"
- Use capitals in front of the sentence
- Don't add full stop (.) at the end of the sentence

## Contributing

### [Code of Conduct](https://github.com/ThymeSave/.github/blob/main/CODE-OF-CONDUCT.md)

ThymeSave has adopted a Code of Conduct that we expect project participants to adhere to. Please read the full text so
that you can understand what actions will and will not be tolerated.

### [Contributing Guide](./CONTRIBUTING.md)

Read our contributing guide to learn about how to propose bugfixes and improvements and contribute to ThymeSave!

