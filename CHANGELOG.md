# Changelog

All notable changes to Shul Widget are documented here.

This project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html). Pre-1.0 releases are pre-production.

## [Unreleased]

- Migrated public distribution to this repo. Source remains in a private repository.

## [v0.0.3] - 2026-06-08

### Added
- Full app shell behind the widget: tap the widget to open a 3-tab app (Today / Schedule / Settings).
- **Today** screen — full chronological list of today's minyanim and shiurim with resolved times, Hebrew + Gregorian date, sunrise/sunset/candle-lighting strip.
- **Schedule** screen — weekly recurring view per tefilla (Shacharis / Mincha / Maariv).
- **Settings** screen — switch shul, manual refresh, check for updates, version info.
- Boot receiver — widget survives device reboot.
- Time / screen-on / date-change receivers — widget repaints on real-world events without waiting for the 30-minute worker tick.
- Stable debug keystore — APK upgrades no longer require uninstalling the previous version.

### Fixed
- Picker save now reliably refreshes the widget (added belt-and-braces `APPWIDGET_UPDATE` broadcast).
- Glance action API resolution (`actionStartActivity(Intent)`).

## [v0.0.2] - 2026-06-08

### Fixed
- `IllegalArgumentException: Only Sp is currently supported for font sizes` Glance crash that left v0.0.1 stuck on "Can't show content". The empty state's `TextUnit.Unspecified` was rejected by Glance's text translator even though it's defined as a no-op default.

## [v0.0.1] - 2026-06-08

First pre-release. Scaffolded:
- Glance widget
- Multi-tenant shul picker (CMH, Khal Yereim, Torah Life Kollel)
- KosherJava zmanim on-device
- WorkManager periodic refresh
- Auto-update from GitHub Releases
- Targets Android 7.1.1+ (API 25)
