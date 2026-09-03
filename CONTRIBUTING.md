# Contributing to Computtite Updates

Contributions are welcome — bug reports, release documentation improvements, or issue triage.
This document covers how to work with the project as a contributor.

---

## Before You Start

- Search [existing issues](https://github.com/Sxnnyside-Project/computtite-updates/issues) before opening a new one.
- For feature proposals or desktop application code changes, please note that core development happens in the Computtite Desktop repository.
- Read the [Code of Conduct](CODE_OF_CONDUCT.md). It applies to all interactions in this project.

---

## Reporting a Bug

Open a [GitHub Issue](https://github.com/Sxnnyside-Project/computtite-updates/issues/new/choose) using the bug report template.

Include:
- What you expected to happen
- What actually happened
- Steps to reproduce
- Environment details (OS, Computtite version, Workspace mode)

---

## Proposing a Feature

Open a [GitHub Issue](https://github.com/Sxnnyside-Project/computtite-updates/issues/new/choose) using the feature request template.

For desktop features, an issue discussion first avoids wasted effort on both sides.

---

## Workflow

1. Fork the repository and create a branch from `main`.
2. Name your branch descriptively — `fix/typo-in-docs`, `docs/installation-guide`.
3. Make your changes.
4. Open a pull request against `main` with a clear description of what changed and why.

---

## Pull Request Checklist

Before submitting:

- [ ] Changes are described in [CHANGELOG.md](CHANGELOG.md) under `[Unreleased]` if applicable
- [ ] The PR description explains what changed and why
- [ ] Commits follow Conventional Commits

---

## Commit Style

This project uses [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). Every commit message must follow the format:

```
<type>: <description>

[optional body]
[optional footer]
```

Accepted types:

| Type       | Use for                                          |
|------------|--------------------------------------------------|
| `feat`     | New functionality                                |
| `fix`      | Bug fixes                                        |
| `docs`     | Documentation only                               |
| `style`    | Formatting, whitespace — no logic changes        |
| `refactor` | Code restructure without behavior change         |
| `test`     | Adding or updating tests                         |
| `chore`    | Build process, tooling, dependencies             |
| `perf`     | Performance improvements                         |

Examples:

```
docs: update release notes for v3.6.1
fix: correct typo in download instructions
chore: bump release metadata
```

---

## Questions

If something about the distribution channel is unclear, open an issue with the `question` label.

---

*Computtite Updates is a Sxnnyside Project release. Part of the [Sxnnyside Project](https://sxnnysideproject.com).*
