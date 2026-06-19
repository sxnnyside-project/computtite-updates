# Computtite

![Version](https://img.shields.io/badge/version-3.5.0-blue)
![License](https://img.shields.io/badge/license-SPUL-purple)

<p align="center">
  <strong>IT Asset Management ✦ Governance ✦ Local &amp; Cloud</strong><br>
  <em>Official release channel for Computtite — a free desktop ITAM platform by Sxnnyside Project.</em>
</p>

<p align="center">
  <a href="#about">About</a> ✦
  <a href="#features">Features</a> ✦
  <a href="#installation">Installation</a> ✦
  <a href="#usage">Usage</a> ✦
  <a href="#contributing">Contributing</a>
</p>

---

## About

**Computtite** is a free IT Asset Management platform for teams, organizations, and IT professionals. It runs as a native desktop application on macOS, Windows, and Linux.

Most ITAM tools are expensive, cloud-dependent, or built for enterprises that can afford dedicated IT software departments. Computtite is built for everyone else — teams that need organized asset tracking without licensing fees or mandatory cloud dependencies.

Computtite works fully offline with local storage, or connected to the cloud for team sync. Core functionality is never gated behind subscriptions.

### Philosophy

> *"Software should be an experience — personal, evolving, and built for the people who use it."*

Computtite is developed and maintained by Sxnnyside Project under the SaaX (Software as an Experience) model. Funding is voluntary. The platform evolves through community participation and direct user support.

## Features

- **Asset tracking**: create and manage any type of technology asset — computers, servers, phones, printers, and more — with fully configurable field schemas
- **Governance**: role-based access control with Permission Profiles that allow fine-grained capability management per team member
- **Asset Visibility**: control who can see each asset — everyone, administrators only, or specific permission profiles
- **Workspace organization**: isolated workspaces, each with their own storage; switch between clients or projects without losing data
- **Local & Cloud modes**: work fully offline or sync your workspace across your team via the cloud
- **People & departments**: structured employee records and department organization with relational integrity
- **Integrations**: export reports directly to Google Sheets or Notion databases via OAuth
- **Reporting & export**: generate inventory and assignment reports; export to Excel, CSV, or JSON
- **Statistics**: charts and summaries for asset counts, type distribution, department coverage, and license status
- **Backup & Recovery**: automatic scheduled backups with integrity verification and corruption recovery
- **Auto-updates**: receive and install updates directly from this repository; choose between stable and beta channels
- **Bilingual**: full English and Spanish support throughout

## Installation

### Supported Platforms

| Platform       | Architecture       | Format          |
|----------------|--------------------|-----------------|
| macOS          | Apple Silicon (M1+)| `.dmg`          |
| Windows        | x64                | `.msi` / `.exe` |
| Linux          | x64                | `.AppImage`     |

### Download

Download the latest release from the [Releases page](https://github.com/SxnnysideProject/computtite-updates/releases).

1. Choose the installer for your platform
2. On macOS: open the `.dmg` and drag Computtite to Applications
3. On Windows: run the `.msi` installer
4. On Linux: make the `.AppImage` executable and run it

### Release Channels

Computtite offers two update channels, configurable inside the application:

- **Stable** — recommended for most users; releases are tested and signed
- **Beta** — access upcoming features earlier; may include rough edges

The active channel can be changed at any time in **Settings → Updates**.

## Usage

Once installed, Computtite runs as a standalone desktop application. No account is required for local use.

**Local mode** — create a workspace and start tracking assets immediately. All data stays on your machine. Automatic backups run according to your configured schedule.

**Cloud mode** — connect a Supabase-backed workspace to sync data across your team. Cloud workspaces require an account and workspace invitation.

**Receiving updates** — Computtite checks for updates automatically. When an update is available, a notification appears in the application. Updates can also be checked manually in **Settings → Updates**. The updater downloads, verifies, and installs the new version; a restart prompt is shown when the install is ready.

## Contributing

This repository is the public release channel for Computtite. Source code and development work live in the main Computtite Desktop repository.

**Report a bug** — open an issue using the bug report template. Include your platform, version, and steps to reproduce.

**Request a feature** — open an issue using the feature request template.

**Security vulnerabilities** — see [SECURITY.md](SECURITY.md). Do not open a public issue for security vulnerabilities.

**Support Computtite** — Computtite is free and voluntarily funded. If it helps your work, consider [supporting on Patreon](https://www.patreon.com/c/sxnnysideproject/membership).

## License

This project is licensed under the Sxnnyside Personal Use License (SPUL) — see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  <strong>Computtite</strong> — Sxnnyside Project<br>
  <em>&copy; 2026 Sxnnyside Project</em>
</p>
