# Changelog

All notable changes to **Computtite** are documented here.

This project follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and [Semantic Versioning](https://semver.org/).

---

## [3.5.0] — 2026-06-19

### Added

- **Permission Profiles** — create named permission sets and assign them to workspace members; profiles let administrators restrict or expand specific capabilities within a member's role, without changing the role itself
- **Asset Visibility** — control who can see each asset: everyone (default), administrators only, or a specific set of permission profiles; cloud workspaces only
- **Workspace governance hub** — expanded Administration area with dedicated tabs for Permission Profiles, Asset Visibility, member invitations, and workspace overview
- **Automatic backups** — configure daily or weekly automatic backups per workspace; backups are verified for integrity before being saved and pruned automatically based on your retention setting (5, 10, or 20 backups)
- **Backup retention policy** — choose how many backups to keep; older backups are removed automatically
- **Restore with safety checkpoint** — when restoring from a backup, a safety copy of the current database is created first so you can recover if anything goes wrong during the restore
- **Corruption recovery** — if Computtite detects a damaged workspace database on startup, it shows a recovery screen listing available backups to restore from
- **Settings → Cloud & Storage → Backup & Recovery** — new section for managing backup schedules, retention, and viewing or restoring individual backup files
- **Google Sheets integration** — export any report directly to a new Google Sheet from the Audit page; connects via your Google account
- **Notion integration** — push asset data and reports to Notion databases from the Audit page; connects via your Notion account
- **Integration health status** — each connected service in Settings → Integrations shows a live status indicator; re-check the connection at any time
- **Statistics dashboard** — view asset counts by type, department coverage, license status, and activity over time; filter by date range
- **Settings → Support** — a funding and transparency page with information about Computtite's development, the SaaX philosophy, and voluntary support options including Patreon; locale-aware links to Sxnnyside Project and Computtite websites; no dark patterns

### Changed

- **Excel export** — reports exported to Excel are now generated using an improved library with better compatibility and an open license; output is identical to previous releases
- All outbound links on the Support page adjust automatically based on your language setting

### Removed

- Internal Excel dependency replaced; no user-facing behavior change

### Security

- Integration credentials (Google, Notion) are stored with strong encryption; long-lived tokens are kept server-side and never stored in the application bundle
- Google and Notion connections use secure OAuth flows; no credentials are stored in plain text
- Automated security checks now run on every release to scan Rust and JavaScript dependencies for known vulnerabilities
- Workspace database integrity is verified on every automatic backup; corrupted backup files are discarded automatically

---

## [3.4.0] — 2026-06-04

### Added

- **Native application menus** — full menu bar integration on macOS and Windows (`Computtite / File / Edit / Window / Help`) with standard OS behaviors including About, Hide, Minimize, Copy, Paste, Undo, and Quit
- **Native keyboard shortcuts** — `⌘,` opens Settings, `⌘N` creates a new asset, `⌘M` minimizes the window; shortcuts work even when focus is inside a text field
- **macOS traffic light integration** — the window's close/minimize/maximize controls are positioned naturally over the sidebar; the sidebar area can be used to drag the window
- **Window state persistence** — window size, position, and maximized state are remembered between sessions and restored before the application loads
- **Native OS notifications** — system notifications for backup completion, report export, and available updates

### Changed

- Release pipeline updated: version consistency is verified across all package files before any build starts; releases are published only after all platform builds succeed
- macOS builds now target Apple Silicon exclusively

---

## [3.3.3] — 2026-02-26

### Added

- **Asset license management** — attach software licenses to tracked assets; record license name, vendor, key, expiry date, and seat count
- **Auto-update system** — Computtite checks for updates automatically and notifies you when one is available; updates download and install with a single click and a restart
- **Update channels** — choose between Stable (recommended) and Beta channels in Settings → Updates
- **Update UI** — a non-intrusive notification when an update is available; a full dialog with release notes, download progress, and restart prompt

---

## [3.2.2] — 2026-02-26

### Added

- **Anonymous usage analytics** — opt-in only; tracks general usage patterns to guide development; no personal data, asset data, or business data is ever collected
- **Telemetry controls** — enable or disable analytics independently in Profile; your installation ID is shown so you know exactly what's associated with your data

### Security

- Analytics data is sanitized and stripped of any sensitive fields before storage
- Disabling analytics clears any locally queued data immediately

---

## [3.2.1] — 2026-02-26

### Added

- **Background sync engine** — cloud workspaces now sync changes to and from the server continuously in the background; changes made offline are queued and sent when connectivity is restored
- **Conflict resolution** — when the same record is changed in multiple places, the most recent change wins; no data is silently discarded

---

## [3.2.0] — 2026-02-25

### Added

- **Multiple workspaces** — create and manage multiple independent workspaces; each workspace has its own isolated data; switch between them without logging out
- **Workspace roles** — four roles: Owner, Admin, Member, and Viewer; each role has appropriate read/write capabilities enforced throughout the application
- **Team invitations** — owners and admins can invite team members by email
- **Ownership transfer** — transfer workspace ownership to another member
- **Viewer read-only mode** — viewers can browse all data but cannot create, edit, or delete records

### Security

- Workspace data is isolated at the database level; members can only access workspaces they belong to
- Exactly one owner per workspace is enforced at the database level

---

## [3.1.2] — 2026-02-25

### Security

- License verification moved server-side with a 24-hour offline cache for resilience
- Login rate limiting: five failed attempts trigger a 15-minute lockout with a live countdown
- Backup import validates file integrity before overwriting any existing data

---

## [3.1.1] — 2026-02-25

### Security

- Content Security Policy enabled and hardened
- All diagnostic logs that could expose workspace or user information are restricted to development builds only
- Development server restricted to local connections only

---

## [3.1.0] — 2026-02-24

### Added

- **Workspace licensing** — license verification with offline enforcement
- **Account system** — email and password login with session persistence and offline fallback
- **Local / Cloud mode** — explicit mode selection per workspace; cloud workspaces use Supabase for storage and sync
- **Data migration** — migrate an existing local workspace to cloud with progress tracking
- **Privacy Policy & Terms of Service** — accessible from Profile, available in English and Spanish

---

## [3.0.0] — 2026-02-23

### Added

- **Computtite Forge** — guided workspace setup with templates for IT, Education, Corporate, and Custom environments
- **Asset types** — create any category of asset with custom fields per type
- **Employee records** — track employees with name, email, role, and department
- **Department organization** — group employees and assets by department
- **Assignment history** — complete audit trail showing who used each asset, when, and in which department
- **Reports and export** — generate inventory and assignment reports; export to CSV or JSON
- **Account login** — email and password authentication with password reset
- **Offline mode** — full local workspace with no network requirement
- **Guided onboarding** — step-by-step tour on first launch
- **Window size presets** — Compact, Default, Large, Full HD
- **English and Spanish** — full bilingual support

---

## [2.x] — Legacy

Previous versions of Computtite were built on Electron. Version 3.0.0 was a complete rewrite as a native Tauri application.

---

[Unreleased]: https://github.com/SxnnysideProject/computtite-updates/compare/v3.5.0...HEAD
[3.5.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.5.0
[3.4.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.4.0
[3.3.3]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.3.3
[3.2.2]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.2.2
[3.2.1]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.2.1
[3.2.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.2.0
[3.1.2]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.1.2
[3.1.1]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.1.1
[3.1.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.1.0
[3.0.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.0.0
