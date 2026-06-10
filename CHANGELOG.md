# Changelog

All notable changes to [Shul Widget](https://github.com/Shalom-Karr/Shul-Widget-Published-App) are documented here. APKs for every tagged release live on the [Releases page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases).

This project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html). Pre-1.0 releases are pre-production.

## [Unreleased]

## [v2.2.1] - 2026-06-09

Smoother shul switching + a cleaner default nav.

- **Switching shuls is instant** — every screen (Today, Schedule, Zmanim, Weather) now reloads the moment you switch shuls, and widgets re-render reliably right after you pick one.
- **Admin tab hidden by default** — most users aren't gabbais; re-enable it in Settings → Visible tabs to sign in.
- **Zmanim** — "Sunrise (Hanetz)" relabeled "Sunrise (Neitz)".

See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v2.2.1) for the APK.


## [v2.2.0] - 2026-06-09

Per-widget shul, a working Custom widget, widget sizing, and a Shabbos view.

### Widgets

- **Each widget can show a different shul** — pick the shul per widget when you place it (Next Up, Zmanim, Full Day, Full Screen, Custom, Weather); its zmanim and times follow that shul. The global shul stays the default.
- **The Custom widget really customizes now** — choose which sections show (Header / Next / Schedule / Zmanim) and reorder them top-to-bottom. Fixes a bug where it always showed everything regardless of your choices.
- **Better sizing** — the widgets now lay out for their actual placed size and re-render when you resize them.

### App

- **See Shabbos** — a new view (twilight icon on the Today screen) showing the upcoming Erev Shabbos (Friday from Mincha onward + candle lighting) and Shabbos, with the **parsha** and Shabbos-ends time.

See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v2.2.0) for the APK.


## [v2.1.1] - 2026-06-09

Wider Next Up widget + zmanim fixes.

- **Next Up widget** is now wide and short (defaults to 3×2, resizable down to 1 tall) instead of a tall narrow box.
- **Tzais Hakochavim** now uses the Geonim 8.5° shita; the separate Rabbeinu Tam entry was removed (the 72-minute entry is labeled "Tzais 72 (Rabbeinu Tam)") and Bein Hashmashos was removed from the list.

See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v2.1.1) for the APK.


## [v2.1.0] - 2026-06-09

Device location for weather.

- **Use device location for weather** (Settings) — the weather screen and weather widget can follow your phone's GPS location instead of the shul's. Zmanim **always** stay on the shul's location (they're halachically tied to where you daven).

See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v2.1.0) for the APK.


## [v2.0.1] - 2026-06-09

Notification settings.

- **Notification settings** (Settings → Notification settings) — pick a custom reminder alarm sound, toggle vibration, and jump to the system per-channel settings. (The alarm channel regenerates so a new sound actually takes effect on Android O+.)

See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v2.0.1) for the APK.


## [v2.0.0] - 2026-06-09

A widget family and a themed UI refresh.

### Widgets — five new types

- **Next Up** — small widget showing just the next minyan/shiur with its time and a live countdown.
- **Zmanim** — today's zmanim, honoring your Settings → Zmanim selection (change it in the app and the widget follows).
- **Full Day** — the whole day's chronological schedule plus a zmanim strip, sized larger than the 3×2 schedule widget.
- **Full Screen** — a big "next" hero + the full schedule + zmanim, sized to fill a maximized home-screen page.
- **Custom** — choose which sections show (Next / Schedule / Zmanim) when you place it, and resize it however you like; each copy is configured independently.

### App

- Brand-themed UI refresh — cohesive navy/gold/cream palette, redesigned Today and Zmanim hero cards, and dynamic color turned off so the Luach identity always shows.

See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v2.0.0) for the APK.


## [v1.0.6] - 2026-06-09

## [v1.3.0] - 2026-06-09

Minyan/zman reminders and a live widget countdown.

- **Reminders** (Settings → Reminders) — get an alarm (vibration + alarm sound) a set number of minutes before a minyan or zman you choose. Repeats every day the time occurs, survives reboots, and uses exact alarms so it lands on the minute.
- **Live widget countdown** — the schedule widget's "NEXT" now reads "in 25 min" / "now", accurate whenever you glance at your phone.
- **Richer widget preview** in the widget picker and during the first-load flash.
- Faster weather refresh (pooled HTTP client).

See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.3.0) for the APK.


## [v1.2.5] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.2.5) for the APK.


## [v1.2.4] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.2.4) for the APK.


## [v1.2.3] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.2.3) for the APK.


## [v1.2.2] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.2.2) for the APK.


## [v1.2.1] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.2.1) for the APK.


## [v1.2.0] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.2.0) for the APK.


## [v1.1.0] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.1.0) for the APK.


## [v1.0.9] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.9) for the APK.


## [v1.0.8] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.8) for the APK.


## [v1.0.7] - 2026-06-09

Released 2026-06-09. See the [release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.7) for the APK.


[Release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.6)

### Changed
- **ABI splits** — CI now produces 4 APKs (`armeabi-v7a`, `arm64-v8a`, `x86_64`, plus a universal fallback). The in-app updater picks the slice matching `Build.SUPPORTED_ABIS`, so a TracFone (armv7) downloads ~25% of what a modern phone does. The universal APK keeps the legacy `shul-widget-vX.Y.Z.apk` filename so v1.0.5 clients with the old asset picker still upgrade safely.
- **R8 on debug builds** — strips ~29,975 unused `material-icons-extended` entries plus other dead code. ~35% APK size cut overall.

### Fixed
- Install time on Android 7.1.1 drops from ~3 minutes to ~30 seconds (smaller APK → less `dex2oat` work).

## [v1.0.5] - 2026-06-09

[Release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.5)

### Changed
- **Settings → Zmanim displayed** moved to a dedicated sub-page. The chip grid no longer clutters the Settings root.
- **Chat composer polish** — `FilledIconButton` fixed at 48dp, smaller progress spinner, rounded TextField, vertically centred alignment.

### Fixed
- **Chat send button stuck loading** — `refresh()`'s `wasSending` preservation was keeping the spinner forever after a successful send. Sending now clears explicitly before refresh.

## [v1.0.4] - 2026-06-09

[Release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.4)

### Added
- **Weather day-detail screen** — tap any day card to open hourly breakdown (temperature, conditions, precipitation chance) plus a sunrise/sunset card and a daily summary.

### Changed
- Open-Meteo hourly forecast now covers all 5 days (was capped at 24h).

## [v1.0.3] - 2026-06-09

[Release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.3)

### Fixed
- **Self-update install dialog** finally appears on Android 7.1.1. `ApkInstaller` is now branched by API level:
  - API < 26: fires `ACTION_VIEW` with a `FileProvider` URI — the legacy path the OS install confirmation reliably honours.
  - API ≥ 26: uses `PackageInstaller.Session` with a new `InstallStatusReceiver` that catches `STATUS_PENDING_USER_ACTION` and launches the confirm intent.
- Both paths post a high-priority notification fallback so the install never gets stuck silent again.
- **UI fixes from the Explore-agent audit:** `ChatScreen` substring crash (replaced with `take`), `KioskPreview` no longer hardcodes `Color.Black/White` (uses theme `scrim` / `inverseOnSurface`), 4 admin form `OutlinedTextField`s now have `imeAction = Done` so the keyboard's Done button actually submits.

## [v1.0.2] - 2026-06-09

[Release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.2)

### Changed
- **Widget + Today rows** now lay out title-left, time-right — matches the kiosk schedule layout for visual continuity.
- **Widget large layout header** picks up the SK Luach logo.
- **Weather widget** medium/large layouts gain an hourly strip (next 4-5 hours with temp + icon).

## [v1.0.1] - 2026-06-09

[Release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.1)

### Added
- **Team chat** — `shul_<prefix>_chat` table with OS notifications via `ChatPollWorker`. New Chat tab in the admin nav.
- **Weather expansion** — hourly forecast, sunrise/sunset, UV, feels-like, cloud cover.

### Changed
- **UpdateChecker rewrite** — sealed `CheckResult` (Throttled / ApiFailure / ParseFailure / UpToDate / NoApkAsset / DownloadFailure / InstallTriggered) so the Settings snackbar can surface what actually happened. Switched from `/releases/latest` to `/releases?per_page=1` so pre-releases resolve too (the old endpoint silently 404s when only pre-releases exist, which is what stranded v0.0.7 → v1.0.0 for installed phones).
- **Widget redesign** — navy + gold "NEXT" card, hairline dividers, bigger fonts.
- **Bottom nav** shrinks fonts (and goes icon-only) when an admin is signed in, so the extra Admin/Chat tabs fit on narrow phones.

### Fixed
- `.gitignore` covers `_artifacts/`.
- Removed rogue `CZC.java` / `ZC.java` files committed by accident.

## [v1.0.0] - 2026-06-09

[Release page](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/tag/v1.0.0)

**First stable release.** Bundles everything from v0.0.1 through v0.0.7.

### Notes
- Promoted v0.0.7's binary from pre-release to stable so the in-app `/releases/latest` updater can resolve it. (GitHub's API silently skips pre-releases.)
- `BuildConfig.VERSION_NAME` inside the APK is still `0.0.7-debug`; v1.0.1 bumps it to `1.0.1` to break the spurious "newer version available" loop on installed v1.0.0 phones.

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
