# Changelog

<!-- markdownlint-disable MD024 -->

All notable changes to this project will be documented in this file.

The format is based on **[Keep a Changelog](https://keepachangelog.com/en/1.1.0/)**
and this project adheres to **[Semantic Versioning](https://semver.org/spec/v2.0.0.html)**.

---

## [Unreleased]

---

## [0.1.0] - 2026-10-08

### Added

- Initial draft, informed by BootLoops
- Added `protocols/independent-review/SKILL.md` - currently used during 2026-Oct update
- Added `protocols/referee-sim/SKILL.md`
- Added `protocols/source-audit/SKILL.md`
- Added `protocols/theory-acceptance/SKILL.md`
- Added `protocols/theory-construction/SKILL.md` - currently used during 2026-Oct update

---

## Notes on versioning and releases

- We use **SemVer**:
  - **MAJOR** - breaking changes
  - **MINOR** - backward-compatible additions
  - **PATCH** - fixes, documentation, tooling
- Versions are driven by git tags.
- Tag `vX.Y.Z` to release.

## Release Procedure (Required)

Follow these steps exactly when creating a new release.

### Task 1. Update release metadata (manual edits)

1.1. CITATION.cff: update version and date-released
1.3. CHANGELOG.md: add section, move unreleased entries, update links
1.4. As needed: pyproject.toml: update version (near top of the file)

### Task 2. Set up and Validate

```shell
# set up or update Python environment
# Run repository checks.
.\sit.ps1

# Update GitHub Actions and pin all action references to immutable SHAs.
uvx gha-tools autoupdate --pin=all --write .github/workflows

# Audit the resulting GitHub configuration for security findings.
# NO .github\workflows\deploy-zensical.yml
# YES  .github\workflows\deploy-zensical-lean.yml
uvx zizmor@latest .github/

# Validate.
uvx cffconvert --validate
uvx se-manifest-schema validate-manifest --strict

# Format Markdown.
npx markdownlint-cli2 --fix
```

Review all generated and modified files before committing.

### Task 3. Commit, tag, push

```shell
git add -A
git commit -m "Prep X.Y.Z"
git push -u origin main
```

Verify actions run on GitHub. After success:

```shell
git tag vX.Y.Z -m "X.Y.Z"
git push origin vX.Y.Z
```

## Only As Needed (delete a tag)

```shell
git tag -d vX.Z.Y
git push origin :refs/tags/vX.Z.Y
```

## Links

[Unreleased]: https://github.com/structural-explainability/se-theory-identity-regimes/compare/v0.1.1...HEAD
[0.1.0]: https://github.com/structural-explainability/se-theory-identity-regimes/releases/tag/v0.1.0
