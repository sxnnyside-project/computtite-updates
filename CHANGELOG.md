# Changelog

All notable changes to **Computtite** are documented here.

This project follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and [Semantic Versioning](https://semver.org/).

---

## [3.9.1-beta.1] — 2026-11-03

This is a beta. Update to it from Settings → Updates by choosing the beta channel.

### Highlights

- **Documents on every asset** — Attach PDF, Word, Excel and text files to an asset, up to 15 MB each, and open them from the asset's page.
- **Who can see and change them** — Two new permissions, *View documents* and *Edit documents*, can be set in each permission profile. Documents follow the asset: if someone cannot see an asset, they cannot see its files.

### New

- **Documents** in the asset editor: add several files at once (PDF, DOC, DOCX, XLSX and TXT) and remove the ones you no longer need. The page of the asset lists them and opens each one with the program you already use for that file type.
- Files are checked before they are saved, so a renamed or damaged file is refused with a clear message.
- In cloud workspaces documents are stored privately and sync to every device of the people allowed to see them. In local workspaces they stay on your computer.
- **Show files folder** in Settings → Cloud & Storage opens the folder with your photos and documents on this computer (local workspaces).

### Improved

- Asset photos accept JPG, JPEG, JFIF, PNG, WebP and BMP, and the editor now shows the accepted formats. Photos are still resized and compressed automatically.
- The documents card in the editor looks and works like the photo card.

### Fixed

- **Photos and files in the cloud now respect the member's role.** Before, any member could replace or delete other people's photos, viewers included. Now it needs permission to edit (or to create, so a new asset or employee can carry its photo).
- The Integrations page no longer repeats its description, and an empty license list shows a single Add button.

### Heads-up

- Animated GIF images are no longer accepted for photos. Use JPG, PNG, WebP or BMP.
- Only PDF, DOC, DOCX, XLSX and TXT are accepted; macro-enabled files such as .docm and .xlsm are not. Documents always open in your own programs, never inside Computtite.

---

## [3.9.0] — 2026-11-02

### Highlights

- **Send reports where your team works** — The new **Send to…** button sends a report to a new or existing Google Sheet, to Google Drive, or to Notion.
- **License keys on every device** — In cloud workspaces, license keys are stored securely and show up on every device of the people allowed to see them.
- **Works offline, stays in sync** — Employee photos and asset pictures stay available without a connection, and items you delete now disappear on every device.
- **Safer backups and access** — Restoring or importing a backup keeps your latest changes, and only members allowed to manage people can send invitations.

### New

- **Send to…** in Reports: a new Google Sheet, an existing sheet and tab, a file in a *Computtite Reports* folder in Google Drive, or Notion (a new database, a new page with a table, or rows added to an existing database).
- Save to Drive uploads the same PDF or Excel file you download, using your export template.
- Choose which Notion page receives your report, and the app remembers it.
- Employee photos and asset pictures are saved on your device, so they show without a connection.

### Improved

- Opening a cloud workspace works offline and never overwrites changes you made while disconnected.
- Restoring or importing a backup saves a safety copy of your current data first, and keeps your most recent changes.
- Importing a backup now checks that the file is intact and belongs to this workspace before replacing anything, and tells you why when it does not.
- Long reports no longer fail halfway: Google and Notion exports are split into parts and retried when the service asks you to wait.
- Reports use your language for words like *Returned*, *Expired* or *Expiring in 10 days*.
- Creating a local workspace needs a one-time sign-in; after that it works without a connection.

### Fixed

- **Opening a workspace a second time no longer fails.**
- **Deleted items disappear everywhere** — Before, a deletion only reached the device where you made it.
- **Only members allowed to manage people can send or cancel invitations**, and changing a member's role or permission profile works again.
- **Too many wrong passwords now pause sign-in for 15 minutes**, as intended.
- Employees who hold assets with no status now show as having assets.
- Multiple-choice fields no longer break when a saved value is plain text.
- A license key in a cloud workspace is no longer left in the sync queue.
- Smaller fixes and updated components for security.

### Heads-up

- Workspaces created before version 3.5.0 must be opened once with a release from 3.5 to 3.8 before moving to this version.

---

## [3.8.0] — 2026-10-12

### Highlights

- **Licenses in one place** — Add, edit or remove a software license right from an asset's page or from the Licenses tab, and jump from any license straight to its asset.
- **Licenses sync across devices** — Everyone in a cloud workspace sees the same seats and expiry dates.
- **Reports that follow your template** — PDF and Excel reports respect your colors, header, footer and fonts, and long statistics reports continue on the next page instead of cutting content off.
- **Clearer wording** — Buttons use short, familiar words such as Add, Save and Cancel, and English and Spanish are fully aligned.

### New

- Edit a license without recreating it, including licenses on an asset you have not saved yet.
- Choose the **Stable** or **Beta** update channel in **Settings → Updates**.
- On Mac, **New Asset** asks which type to create, and **Export Report** and **Export Inventory** are separate menu items.
- The app now appears only when it is ready, so there is no white flash when it starts.
- Only one Computtite window opens at a time, and links from your email open in the window that is already running.
- If you reset your password from an email link, it now opens the reset form directly.
- Photos you upload are smaller and load faster.

### Improved

- Switching workspaces is cleaner: you no longer see the previous workspace's data while the new one loads.
- When inviting, removing or changing a member fails, you now see what went wrong.
- Menus, buttons and messages are consistent across the whole app, with no mixed English and Spanish.
- A stronger security setup for the app and faster, more reliable updates.

### Fixed

- **Sync no longer gets stuck on "Syncing…"** — If something could not be sent, the app now says so and keeps trying instead of spinning forever.
- **Returning an asset now reaches the cloud** — Closing an assignment in a cloud workspace could fail to sync, even for the owner. It now saves correctly, including for assignments created before cloud sync was turned on.
- **Asset pages no longer go blank** when you open or switch between assets.
- **License and asset changes appear right after syncing**, without reopening the page.
- **Links from a license** now take you to the right asset.
- **Reports with accented characters** (such as é or ñ) no longer cause the app to stop when exporting.
- **Missing or untranslated texts** that showed up as technical codes now read properly.
- **"Reveal in folder"** now selects the file in Finder or Explorer.
- **The What's new window** works again.

---

## [3.7.0] — 2026-09-07

### Added

- **Desktop Magic Pairing for Mobile Companion** — Log in to Computtite Mobile Companion on iOS and Android instantly without typing passwords or email addresses. Open **Profile → Session**, click **Pair Mobile Companion**, and scan the high-contrast QR code with your phone camera to transfer your secure session immediately.
- **Full-Page Settings Hub** — Workspace settings have been reimagined into full-width pages that take advantage of your entire screen, replacing narrow modal popups. Easily navigate from the collapsible sidebar to dedicated sub-pages for *Workspace*, *Members*, *Integraciones*, *Almacenamiento*, *Actualizaciones*, *Apoyo*, and *Zona de Peligro*.
- **Official Account Deletion Workflow** — A new transparent privacy option in *Zona de Peligro* allows workspace members to request permanent account deletion via the official Sxnnyside Project privacy process, with safeguards that prevent leaving active team workspaces without an owner.

### Changed

- **Unconstrained Desktop Window Resizing** — Removed rigid window resolution presets. Computtite can now be freely resized, snapped, maximized, minimized, or tiled across any monitor setup or aspect ratio without restrictions.
- **Collapsible Sidebar Navigation** — The Settings entry in the sidebar now expands to list all configuration sections directly, saving time and clicks.

### Fixed

- **Camera-Optimized QR Recognition** — Upgraded QR generation to standard ISO/IEC 18004 compliance, ensuring immediate optical scanning recognition by all mobile device cameras.
- **Clean Table Empty States** — Normalized empty states across Licenses, Visibility, Profiles, Invitations, and Audit Timeline, eliminating redundant nested buttons and ensuring design consistency.
- **Localization Polish** — Resolved untranslated system labels across administrative panels and confirmation modals for a 100% complete bilingual experience.

---

## [3.6.2] — 2026-09-03

### Fixed

- **Cloud Workspace Sign-in Synchronization** — Resolved an intermittent timing issue during authentication that could prevent cloud workspace users from accessing their workspace after signing in or resuming a session, causing them to stay on the workspace selection screen.
- **Resilient Deep Link Handling** — Hardened deep link callback deduplication at module scope, preventing redundant authorization code exchanges.
- **Release Pipeline Acceleration** — Enabled multithreaded linking on Windows and Linux and integrated compiler caching in our build and distribution infrastructure.

---

## [3.6.1] — 2026-09-03

### Performance & Speed

- **Instant Search & History Loading** — database queries for asset filtering, employee lookups, and audit history now load up to **169x faster** with automatic database indexing. Workspace navigation is completely smooth even with thousands of assets.
- **Faster Application Launch** — the initial app download and parse size is **343 kB lighter** (-36%), helping Computtite open noticeably faster on desktop.
- **Smart Offline Startup** — if your internet connection is slow or unstable, Computtite will no longer freeze waiting on the network. It automatically opens your local workspace within 3 seconds so you can get right to work.

### Added

- **Black Pillar Health & Crash Diagnostics** — an anonymous, privacy-focused diagnostic system from Sxnnyside Project that automatically reports technical crashes, freezes, and panics so we can fix them immediately.
  - No personal data, asset names, emails, or IP addresses are ever collected.
  - Includes a simple toggle in **Profile → Privacy** to turn it on or off at any time without affecting any feature of the app.

### Fixed

- **Password reset reliability** — clicking password reset links from your email or browser now reliably opens Computtite and directs you straight to the reset screen.
- **Plugin Store browsing for all members** — workspace members can now freely browse and discover available plugins in the Plugin Store (installation and configuration remains reserved for administrators).
- **Accurate report assignments** — all generated reports (inventory, maintenance, departments, and employee lists) now correctly map the currently assigned user for every asset.
- **Clear reconnection errors** — reconnecting Google Workspace and Notion now clearly explains any configuration or OAuth issue instead of failing silently.

---

## [3.6.0] — 2026-08-26

### Added

- **First-Party Plugin Ecosystem & Plugin Store** — Computtite now features a dedicated Plugin Store page where you can manage and inspect official extensions with granular permission controls. The initial launch includes six built-in plugins:
  - *Copy to Clipboard* — instant one-click copying for asset identifiers and field values.
  - *Custom Layouts* — choose between Standard, Bento, and Mixed card layouts in the asset detail view.
  - *Custom Export Templates* — save and apply custom field presets and column orders for your exports.
  - *Stats Export* — export comprehensive workspace statistics reports directly to PDF.
  - *QR Generator* — generate high-resolution QR codes encoding asset UUIDs for instant scanning.
  - *Barcode Generator* — generate canonical Code-128 linear barcodes compatible with handheld barcode readers and Computtite Mobile Companion.
- **Revamped Statistics Hub** — transform your workspace data into actionable insights with core inventory KPIs, valuation summaries, interactive distribution charts by status and type, and native PDF exports.
- **Extensible Asset Detail View** — dynamic layout customization, field action buttons, and direct code-generation modals in the asset detail header.

### Changed

- **Optimized Performance & Bundle Footprint** — dynamic code-splitting for heavy export libraries (ExcelJS, pdf-lib) and optimized vector asset caching for a faster, lighter desktop experience.

### Fixed

- **Window Resolution Presets & Resizing** — resolved window sizing issues across desktop operating systems when switching resolution presets, with improved window dragging ergonomics on macOS.
- **Integration Stability** — enhanced reliability for Google Drive, Google Sheets, and Notion connections with native CORS-free networking.

---

## [3.5.3] — 2026-06-26

### Added

- **More field formats** — text fields now support six additional formats: IPv6, CIDR (network ranges), hostname, port number, semantic version, and license key; each one validates what you type so only correct values are accepted
- **Options editor for select and multi-select fields** — add, remove, and manage the list of choices for a select or multi-select field directly inside the field editor, without leaving the page
- **Integer-only number fields** — number fields can now be restricted to whole numbers only, useful for quantities, seat counts, and similar fields where decimals don't apply
- **Open URLs in one click** — fields that store a web address now show a button to open it in your browser directly from the asset detail view

### Fixed

- Asset type icons now display correctly throughout the app — in the sidebar and on the workspace home screen; previously some icons fell back to a generic placeholder
- Anonymous usage data from users who had opted in was not reaching its destination; this has been corrected

---

## [3.5.2] — 2026-06-25

### Added

- **Interactive tutorial** — a step-by-step walkthrough for first-time users to help you get started with the workspace
- **"What's New" screen** — see the latest features and changes right inside the app after installing an update
- **Real-time role updates** — changes to a member's role or permission profile now apply instantly without requiring them to restart the app
- **Activity tracking** — actions are now securely audited in the background

### Changed

- **Improved Assets view** — the Licenses and Layouts tabs now use a more powerful data table for easier reading and interaction
- **Expanded translations** — improved Spanish and English translations across the app, including the settings and onboarding screens
- **Profile page improvements** — better avatar handling and updated support links

### Fixed

- Resolved a minor memory issue that could occur after printing reports
- Fixed a rare issue where user roles could display incorrectly on the workspace page

---

## [3.5.1] — 2026-06-22

### Added

- **Actionable Workspace Health** — clicking a health alert (such as items needing maintenance, unassigned assets, or license issues) now takes you directly to a filtered view of exactly those items
- **License filtering** — the Licenses tab now features summary cards at the top (active, expiring soon, expired) that let you instantly filter the list
- **Seat overage alerts** — Computtite will now warn you if a software license has more seats assigned than you own, displaying this both in Workspace Health and the Licenses tab

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

[Unreleased]: https://github.com/SxnnysideProject/computtite-updates/compare/v3.7.0...HEAD
[3.9.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.9.0
[3.8.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.8.0
[3.7.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.7.0
[3.6.2]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.6.2
[3.6.1]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.6.1
[3.6.0]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.6.0
[3.5.3]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.5.3
[3.5.2]: https://github.com/SxnnysideProject/computtite-updates/releases/tag/v3.5.2
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
