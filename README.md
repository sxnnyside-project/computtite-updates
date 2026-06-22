# Computtite

![Version](https://img.shields.io/badge/version-3.5.0-blue)
![License](https://img.shields.io/badge/license-SPUL-purple)

<p align="center">
  <strong>IT Asset Management ✦ Free, No Subscriptions ✦ Local &amp; Cloud</strong><br>
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

**Computtite** is a free desktop application for tracking the technology assets your team uses every day — computers, phones, servers, licenses, and more. It runs natively on macOS, Windows, and Linux, with no browser required and no data sent anywhere you don't control.

Most ITAM tools are expensive, cloud-only, or built for enterprises with dedicated IT departments. Computtite is for everyone else — teams replacing spreadsheets, small IT shops that need structure without overhead, and organizations that want control over their own data.

Computtite works fully offline, or connected to the cloud for team sync. Everything works without a subscription. Nothing is locked behind a paywall.

### Philosophy

> *"Software should be an experience — personal, evolving, and built for the people who use it."*

Computtite is developed and maintained by Sxnnyside Project under the SaaX (Software as an Experience) model. Funding is voluntary. The platform evolves based on real usage — shaped by the people who use it, not by a product roadmap written for investors.

## Features

- **Asset tracking**: track any type of technology asset your team owns or manages — computers, servers, phones, printers, licenses, and more; fields and structure adapt to your inventory, not the other way around
- **Access control**: decide who can see, edit, or export assets; assign roles to team members and fine-tune their permissions with named profiles
- **Asset Visibility**: control who can see each asset — everyone, administrators only, or specific permission profiles
- **Workspace organization**: isolated workspaces, each with their own storage; switch between clients or projects without losing data
- **Local & Cloud modes**: work fully offline or sync your workspace across your team via the cloud
- **People & departments**: structured employee records and department organization with relational integrity
- **Integrations**: export reports directly to Google Sheets or Notion databases via OAuth
- **Reporting & export**: generate inventory and assignment history reports; export to Excel, CSV, or JSON — or push directly to Google Sheets or Notion
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

Once installed, Computtite runs as a native desktop application. An account is required to create and access a workspace — it is used to identify your workspace, not to gate features or collect your data.

**Local mode** — your asset data is stored exclusively on your machine. Computtite uses your account only to identify the workspace; no asset data is sent to any server. Automatic backups run according to your configured schedule.

**Cloud mode** — connect a Supabase-backed workspace to sync data across your team. Asset data is stored in your cloud workspace and shared with invited members according to their roles and visibility settings.

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
