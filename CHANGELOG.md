# Changelog

All notable changes to Shul Widget are documented here.

This project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html). Pre-1.0 releases are pre-production.

## [Unreleased]

- v0.0.6: Events table, item-type icons (book/person), team chat with OS notifications, 6 more daily zmanim.

## [v1.0.3] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.3) for the APK.


## [v1.0.2] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.2) for the APK.


## [v1.0.1] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.1) for the APK.


## [v1.0.0] - 2026-06-09

**First stable release.**

### Notes
- Promoted v0.0.7's binary from pre-release to stable so the in-app `/releases/latest` updater can resolve it. (GitHub's API silently skips pre-releases.)
- `BuildConfig.VERSION_NAME` inside the APK is still `0.0.7-debug`; v1.0.1 will bump it to `1.0.1` to break the spurious "newer version available" loop on installed v1.0.0 phones.

### Bundles everything from v0.0.1 through v0.0.7.

## [v0.0.7] - 2026-06-09

### Added
- **Open-Meteo weather** — new Weather tab + separate weather widget. Free, no API key.
- **Events** — `shul_<prefix>_events` table support. Non-tefilla recurring items appear in Today + widget; `is_header` rows render as section dividers.
- **Admin → Events tab** — full CRUD form, `is_header` toggle collapses time fields.
- **Item-type icons** on Today + widget: book for minyanim, person for shiurim, calendar for events. Toggle in Settings.
- **6 more zmanim**: Plag Hamincha (MGA), Bain Hashmashos (RT 13.24°), Tzais 60, Tzais 72, Tzais (Rabbeinu Tam), Chatzos Halayla.

### Changed
- **Admin tab row** is now a horizontally-scrolling LazyRow of FilterChips — fits on narrow phones without truncation.
- **Widget large layout** rewritten with Glance LazyColumn — scrolls through the full chronological day.

## [v0.0.6] - 2026-06-09

### Added
- **Admin tab in bottom navigation** — appears automatically when signed in.
- **Date picker on Today** — calendar icon top-right, pick any date.

### Changed
- **Widget refresh on shul switch** — reliably repaints with the new shul's data.

### Fixed
- `release-to-public.yml` workflow — replaced broken Python heredocs with awk + sed.

## [v0.0.5] - 2026-06-09

### Added
- **Admin login + RBAC** — Sign in with your shul Supabase email/password. Owner / admin roles unlock the admin shell.
- **Admin CRUD** — minyanim, shiurim, exceptions, and basic settings, all editable from the phone via the Supabase REST API.
- **Kiosk preview** — landscape-locked WebView of your shul's public kiosk page (Settings → Open kiosk preview).
- **"Open full admin in browser"** — deep link to your shul's web admin for tenant-specific features (TLK audio uploads, CMH custom hero, …).
- **Report a bug** — pre-filled GitHub issue with app/Android/shul diagnostics.
- **Shul logos** — pulled from registry into pickers, screens, and headers via Coil.
- **SK Luach app icon** — custom adaptive icon.
- **David Libre Hebrew font** — embedded.
- **Zmanim 6 → 14** — added Alos, Misheyakir, Sof Zman Shma / Tfila (MGA + GRA), Chatzos, Mincha Ketana.

### Changed
- **Widget UI** — always-light cream surface, navy + gold text, bigger fonts, responsive small/medium/large layouts.
- **Candle lighting** — now only shows on Friday.
- **Settings "Check for updates"** — bypasses the 6-hour throttle so manual taps actually hit the API.

### Fixed
- **Khal Yereim load failure** — handle nullable `tefilla` / `day_pattern` / `anchor` in resolver.

## [v0.0.4] - 2026-06-09

### Added
- **Zmanim tab** — 4th tab showing all selected zmanim. Customize which ones in Settings → Zmanim displayed.
- **Boot + tick receivers** — widget repaints on reboot, screen-on, time/date change without waiting for the 30-minute worker.
- **Stable debug keystore** — APK upgrades no longer require uninstalling.
- **Widget rewrite** — responsive small/medium/large layouts; explicit error and empty states (no more silent dashes).

### Changed
- Refined Material 3 theme, PullToRefresh on Today, SegmentedButton on Schedule, shared empty/loading/error states with proper icons, fade transitions.

### Fixed
- Picker save now reliably refreshes the widget (extra `APPWIDGET_UPDATE` broadcast).
- Glance action API resolution (`actionStartActivity(Intent)`).

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
