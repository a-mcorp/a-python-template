# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!--
Template
## [{project-version}] - {YYYY-MM-DD}

### Added
### Changed
### Deprecated
### Removed
### Fixed
### Security
-->

## [1.1.0] - 2026-11-21

### Changed
- Links to the repositories point to the 'a-mcorp' organisation on GitHub.
- `.github/pull_request_template.md` and `PULL_REQUEST_TEMPLATE/Default.md`: a checkbox in the Comments section marks when an assistant helped to write the changes.
- Licence changed from GPL-3.0-or-later to MIT No Attribution (MIT-0), so projects created from the template choose their own licence; `README.md`, `pyproject.toml` and the AppImage `appdata.xml` follow it, with the AppStream `metadata_license` set to CC0-1.0, since AppStream requires a permissive licence for metadata.
- `README.md` layout
  - Features and two example screenshots combined in one table: the features span the full width, with the screenshots side by side below (`{example-N-title}` and `{example-N-image}` placeholders, images in `docs/`).
  - Dependencies and Usage placed side by side in a two-column table, keeping their list formatting; the separate Example section was removed, and Repository structure became a level 3 heading.

## [1.0.0] - 2026-11-10

### Added
- Project setup
  - `pyproject.toml` with placeholder project metadata, keywords and classifiers, installable as-is.
  - Python `.gitignore`, including an `*.AppImage` rule.
  - `LICENSE` (GPL-3.0).
- Code quality (local CI)
  - `.pre-commit-config.yaml` with `pre-commit-hooks`, `ruff` and `mypy` hooks.
  - `ruff` (formatting, isort rules, PEP 257 docstrings) and `mypy` configuration in `pyproject.toml`.
- Packaging (local CD)
  - AppImage recipe in `AppImage/Recipe`: entrypoint, desktop entry with `X-AppImage-Version`, AppStream metadata and icon.
  - `AppImage/README.md` build guide and `docs/python-appimage.png` example.
- Documentation
  - `README.md` with Metadata, Features, Setup (Dependencies, Installation, Usage, Repository structure), Example and a commented-out Troubleshooting section.
  - `CHANGELOG.md` and its template `.github/CHANGELOG_TEMPLATE/CHANGELOG.md`, based on Keep a Changelog.
  - `TO-DO.md`.
- GitHub repository templates
  - Default pull request template `.github/pull_request_template.md` and `.github/PULL_REQUEST_TEMPLATE/Default.md`.
  - `.github/CODEOWNERS`, its template `.github/CODEOWNERS_TEMPLATE/CODEOWNERS` and the GitHub sample `.github/CODEOWNERS_TEMPLATE/CODEOWNERS_SCHEMA`.
- Template conventions
  - Standardised kebab-case placeholder names (`{project-*}`, `{author-*}`, `{dependency-N-*}`, `{python-*}`, `{issue-*}`) across all template files.
  - Compatibility with 'a-skills'.
