# Changelog — NanaZip Rev

All notable changes made by this fork on top of upstream are documented here.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project uses a fork-suffix in the human-readable version string
(e.g., `7.0.1845.0+rev.3`) while keeping the MSIX `<Identity Version>`
compliant as `Major.Minor.Build.Revision` (four non-negative integers).

## [Unreleased]

### Added
- Fork metadata: this `CHANGELOG.md`, updated `ReadMe.md`.
- `.workbuddy/` added to `.gitignore`.

### Changed
- MSIX manifest `Identity` from upstream `40174MouriNaruto.NanaZipPreview`
  to `kaixinol.NanaZipRev`. Publisher switched from
  `CN=E310A153-74A9-4D81-800B-857A8D58408A` (Kenji Mouri's cert) to
  `CN=kaixinol` (self-signed).
- MSIX `<Identity Version>` bumped from `7.0.1845.0` to `7.0.1848.0`,
  layering the following fork commits on top of the three listed under
  `7.0.1848-rev.0` below:
  - [`420ba09c`](https://github.com/kaixinol/NanaZipRev/commit/420ba09c) — Add Ctrl+W shortcut to close the File Manager window
  - [`d12f5851`](https://github.com/kaixinol/NanaZipRev/commit/d12f5851) — Add an in-app inverted dark/light theme for File Manager
  - [`464b7bdf`](https://github.com/kaixinol/NanaZipRev/commit/464b7bdf) — Move the fork's new Settings control identifiers to the 35xx range
  - [`82fa7494`](https://github.com/kaixinol/NanaZipRev/commit/82fa7494) — Tidy up the inverted theme support
- `<DisplayName>`, `<PublisherDisplayName>`, `<ShortName>` updated to
  reflect "NanaZip Rev" branding.
- `NanaZip.Modern.vcxproj` `MileProjectCompanyName`,
  `MileProjectFileDescription`, `MileProjectLegalCopyright`,
  `MileProjectProductName` updated for fork branding.

## [7.0.1848-rev.0] - 2026-10-01

### Notes
- **Base**: upstream `a6fc1284` at fork establishment.
- **Default branch renamed**: `main` → `nanazip-rev` (GitHub UI step;
  the local branch already exists).

### Cherry-picked from upstream / unsynced
- [`1523f181`](https://github.com/kaixinol/NanaZipRev/commit/1523f181) — FileManager: add ShowFileSizeUnits setting and IEC size formatter
- [`4cde93a1`](https://github.com/kaixinol/NanaZipRev/commit/4cde93a1) — Add language selection to Modern File Manager
- [`3ea6e958`](https://github.com/kaixinol/NanaZipRev/commit/3ea6e958) — Add warning for 7z compression methods unsupported by upstream 7-Zip