# Changelog

All notable changes to `Majo.LineEditing` are documented in this file.

## 0.0.4 - 2026-10-04

### Fixed

- Clear the active input on both Windows and POSIX when `ReadLineAsync` is interrupted with `Ctrl+C`.

## 0.0.3 - 2026-10-01

### Changed

- Renamed the project, NuGet package, assembly, and namespaces from `Majo.LineEditor` to `Majo.LineEditing`, while keeping `LineEditor` as the primary public type.
- Marked `Wcwidth` as an implementation-only dependency so its compile-time assets are no longer exposed to package consumers.

### Fixed

- Fixed cancellation cleanup on both Windows and POSIX so an active input line is cleared when `ReadLineAsync` is canceled instead of leaving partially rendered input in the terminal.

## 0.0.2 - 2026-09-24

### Added

- Added a dedicated NuGet README for the package.
- Added NuGet package links, a NuGet badge, and installation instructions to the GitHub README files.

### Changed

- Updated NuGet packaging and CI validation to use `README.nuget.md` instead of the GitHub repository README.

## 0.0.1 - 2026-09-24

- Initial release.