# Shul Widget

Android app + home-screen widget for any Luach-powered shul. Multi-tenant — one app, three shuls so far (CMH, Khal Yereim, Torah Life Kollel), more easy to add.

## Install

1. Download the APK from [Releases](https://github.com/Shalom-Karr/Shul-Widget-Published-App/releases/latest).
2. Open it on your phone. Allow "Install from unknown sources" if asked.
3. Long-press your home screen → **Widgets** → drag **Shul Widget** out.
4. Pick your shul. Done.

Supports **Android 7.1.1 (API 25) and up**.

## What's in the app

### Five tabs (six when signed in as admin)

- **Today** — chronological list of today's minyanim, shiurim, and events with a date picker so you can scrub to any day, past or future
- **Schedule** — weekly recurring view per tefilla (Shacharis / Mincha / Maariv)
- **Zmanim** — 20 zmanim available (Alos, Misheyakir, Sunrise, Sof Zman Shma MGA + GRA, Sof Zman Tfila MGA + GRA, Chatzos, Mincha Gedola, Mincha Ketana, Plag, Plag MGA, Candle Lighting, Sunset, Bain Hashmashos, Tzais, Tzais 60, Tzais 72, Tzais RT, Chatzos Halayla). Customize which appear in Settings.
- **Weather** — Open-Meteo (free, no API key), current conditions + 5-day forecast
- **Settings** — switch shul, admin login, customize zmanim, item-type icons toggle, kiosk preview, open full web admin, report a bug, check for updates
- **Admin** (appears only when signed in) — minyanim / shiurim / events / exceptions / settings CRUD against your shul's Supabase

### Two widgets

- **Schedule widget** — three responsive sizes; large layout scrolls the full chronological day via Glance LazyColumn. Light cream surface, navy + gold text, item-type icons.
- **Weather widget** — current conditions + 5-day forecast in the same visual language.

### Other

- Zmanim computed on-device via KosherJava — no network round-trip after the first load
- Auto-updates from this repo's Releases — install once, get every future version automatically
- Self-updater shows verbose snackbar diagnostics (v1.0.1+) so you can see exactly what happened
- Light theme for the widgets regardless of system dark mode (home screens have unpredictable wallpapers)
- Stable debug keystore so APK upgrades happen in place, no uninstall + reinstall

## Latest changes

See [CHANGELOG.md](CHANGELOG.md) for the full release history. The landing page at <https://shalom-karr.github.io/Shul-Widget-Published-App/> renders the changelog inline.

## License

© 2026 Shalom Karr. All rights reserved.

You may **install and use** this app on personal devices for personal, non-commercial purposes. You may **not** modify, distribute, mirror, re-upload, sell, or create derivative works without **explicit written permission** from Shalom Karr. See [LICENSE](LICENSE) for the full terms.

## Source

Source code is in a separate private repository. Distribution and releases live here.
