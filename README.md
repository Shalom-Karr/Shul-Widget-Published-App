# Shul Widget

Android app + home-screen widget for any Luach-powered shul. Multi-tenant — one app, three shuls so far (CMH, Khal Yereim, Torah Life Kollel), more easy to add.

**Latest: v3.1.0 — Zmanim & Weather by your location** — pick **“No Shul — Zmanim & Weather only”** in the shul list and the app becomes a clean **zmanim + weather** app for **your device location or a ZIP code** (Today and Schedule tabs hide themselves, and reminders become zmanim-only). The Zmanim header shows your city, ZIP, and coordinates. v3.0.0 added **Flip Phone Support** — a separate **flip-phone APK** with full **D-pad navigation** (Left/Right switch tabs, Up/Down/OK select), a scaled-down UI, and non-touch install support; regular phones grab the normal APK as before. v2.5.1 added **swipe between tabs**, the **Next Zman** widget's tomorrow rollover (+Chatzos), and weather-widget 2×2 details. v2.5.0 added reminders **full-screen alarm** (snooze/dismiss) + "fires in X", the weather widget **2×1 / 2×2 (with H/L)**, and a **Shabbos widget** (4×6). v2.4.0 introduced the redesigned **widget lineup** of purpose-built widgets, each with a real preview in the picker, plus first-launch home-screen setup. v2.3.0 added **Nearby shuls**, **all zmanim by default**, and a device-location **weather header**. v2.2.1 added **instant shul switching** and hid the **admin tab** by default. v2.2.0 added **per-widget shul** (every widget can show a different shul), the **Custom widget** that really customizes (pick + reorder sections), better widget sizing, and a **See Shabbos** view (Friday-Mincha-onward + Shabbos, with the parsha). v2.1.x added **device location for weather** and a wider Next Up widget; v2.0.x brought the full **widget family** (seven widgets) plus **reminders** with customizable alarm sound. v1.1.0 added **Sign in with Google** for admins.

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
| **Settings** | Switch shul, refresh schedule, check for updates, customize zmanim, **pick which tabs are visible in the bottom nav** (v1.2.0+), **reminders** (v1.3.0+), item-type icons toggle, kiosk preview, open full web admin, contact developer, report a bug. |

### Zmanim & Weather by your location — no shul needed *(v3.1.0)*

Not affiliated with a shul in the list, or just want zmanim and weather for wherever you are? In the shul picker, choose **“No Shul — Zmanim & Weather only.”** The app then:

- **Hides the Today and Schedule tabs** — there's no shul schedule, so it becomes a focused **Zmanim + Weather** app.
- Computes **zmanim on-device** (KosherJava) for **your location**, and shows **local weather** for the same spot.
- Lets you set that location in **Settings → Location** — either your **device GPS** or a **US ZIP code**. The Zmanim header shows your **city, ZIP, and coordinates**.
- Keeps **reminders** working — in this mode they're **zmanim-only** (e.g. "20 minutes before sunset").

### Reminders *(v1.3.0+)*

Settings → **Reminders**. Pick a minyan or a zman and how many minutes before it you want to know — the phone fires an **alarm-style notification (vibration + alarm sound)** at that moment, repeating every day the time occurs. Built on exact alarms so "10 minutes before Mincha" lands on the minute, and re-armed automatically after a reboot.

### Seven widgets *(expanded in v2.0.0)*

Long-press the home screen → **Widgets** → **Shul Widget** to find them all. Every widget keeps a light cream surface with navy + gold text so it reads on any wallpaper, and any widget showing zmanim honors your Settings → Zmanim selection.

- **Schedule widget** — three responsive sizes; large layout scrolls the full chronological day. Now shows a live **"NEXT · in 25 min" countdown**.
- **Next Up** *(v2.0.0)* — small, just the next minyan/shiur with its time and a live countdown.
- **Zmanim** *(v2.0.0)* — today's zmanim (the set you chose in Settings).
- **Full Day** *(v2.0.0)* — the whole day's schedule plus a zmanim strip, sized larger than the 3×2 schedule widget.
- **Full Screen** *(v2.0.0)* — a big "next" hero + the full schedule + zmanim, sized to fill a maximized home-screen page.
- **Custom** *(v2.0.0)* — configure on placement which sections show (Next / Schedule / Zmanim) and resize it however you like; each copy is independent.
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
