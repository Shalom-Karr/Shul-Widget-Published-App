# Shul Widget

Android app + home-screen widget for any Luach-powered shul. Multi-tenant — one app, three shuls so far (CMH, Khal Yereim, Torah Life Kollel), more easy to add.

**Latest: v1.2.1** — Hide/show bottom-nav tabs (Settings → Visible tabs) + fix for the "Pick a shul before signing in with Google" false negative. v1.1.0 added **Sign in with Google** for admins.

## Install

1. Download the APK for your phone from the [latest release](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/latest).
   - Most modern phones: `shul-widget-vX.Y.Z-arm64-v8a.apk`
   - Older budget phones (TracFone, Moto E): `shul-widget-vX.Y.Z-armeabi-v7a.apk`
   - Emulator / unsure: `shul-widget-vX.Y.Z.apk` (universal)
2. Open it on your phone. Allow "Install from unknown sources" if asked.
3. Long-press your home screen → **Widgets** → drag **Shul Widget** out.
4. Pick your shul. Done.

Supports **Android 7.1.1 (API 25) and up**.

## What's in the app

### Seven tabs

| Tab | What |
| --- | --- |
| **Today** | Chronological list of today's minyanim, shiurim, and events. Date picker scrubs to any day, past or future. |
| **Schedule** | Weekly recurring view per tefilla (Shacharis / Mincha / Maariv). |
| **Zmanim** | 20 zmanim available (Alos, Misheyakir, sunrise, Sof Zman Shma / Tfila MGA + GRA, Chatzos, mincha gedola / ketana, plag MGA + plag, candle lighting, sunset, bain hashmashos, tzais 60 / 72 / RT, chatzos halayla). Customize which appear in Settings. |
| **Weather** | Open-Meteo (free, no API key) — current conditions, 5-day outlook, hourly breakdown when you tap a day. |
| **Admin** | **Sign in with Google** *(v1.1.0)* or email/password. Once signed in, manage minyanim, shiurim, events, exceptions, and settings for your shul. |
| **Chat** *(admins only)* | Per-shul team chat with OS notifications. |
| **Settings** | Switch shul, refresh schedule, check for updates, customize zmanim, **pick which tabs are visible in the bottom nav** (v1.2.0+), item-type icons toggle, kiosk preview, open full web admin, contact developer, report a bug. |

### Two widgets

- **Schedule widget** — three responsive sizes; large layout scrolls the full chronological day via Glance LazyColumn. Light cream surface, navy + gold text, item-type icons.
- **Weather widget** — current conditions + 5-day forecast in the same visual language.

### Under the hood

- **Stale-while-revalidate caching** — tabs paint cached data instantly, refresh in the background.
- **Zmanim computed on-device** via KosherJava — no network round-trip after the first load.
- **ABI-aware self-updater** — picks the APK slice matching your phone's CPU so you don't download more than you need.
- **Auto-updates** from this repo's Releases — install once, get every future version automatically.
- **Light theme widgets** regardless of system dark mode (home screens have unpredictable wallpapers).
- **Stable signing** — APK upgrades happen in place, no uninstall + reinstall.

## Sign in with Google

v1.1.0 added a "Sign in with Google" button on the Admin tab.

1. Tap **Admin** at the bottom of the app.
2. Tap **Sign in with Google**.
3. A browser tab opens; pick your Google account.
4. You're returned to the app automatically. If your account is listed as an admin for the selected shul, you'll land in the management screen.

Email/password sign-in is still available below the Google button.

## Latest changes

See [CHANGELOG.md](CHANGELOG.md) for the full release history. The landing page at <https://shalom-karr.github.io/Shul-Widget-Published-App/> renders the changelog inline.

## Contact + support

- **Contact developer**: shalomkarr+luach.app@gmail.com
- **Report a bug**: Settings tab → Report a bug — opens a GitHub issue prefilled with app/Android/shul diagnostics.

## License

© 2026 Shalom Karr. All rights reserved.

You may **install and use** this app on personal devices for personal, non-commercial purposes. You may **not** modify, distribute, mirror, re-upload, sell, or create derivative works without **explicit written permission** from Shalom Karr. See [LICENSE](LICENSE) for the full terms.

## Source

Source code is in a separate private repository. Distribution and releases live here.
