# Need For Print

Personal app to save and organize 3D models you want to print. Built for **Android** as a PWA (Progressive Web App).

## Features

- Paste a link from **Printables**, **Thingiverse**, **MakerWorld**, **Thangs**, **Creality Cloud**, **Cults3D**, **MyMiniFactory**, **Yeggi**, or **Sketchfab**
- Set a custom **title** for each model
- Pick a **color** per project (colored border on each card)
- **Light / dark theme** with a header switch (preference saved on device)
- Source platform logo on each card
- Quick share from every card
- **Receive links** from other apps (Share → Need For Print): opens “New model” with the URL prefilled (installed PWA on Android)
- Custom tags with suggestions from tags you already use
- Mark **printed** or **to print**
- Filters by status, tag, and **color family** (AND), plus text search
- Data stored on device (localStorage)
- Export/import backup as JSON
- Works offline after the first load
- **noindex**: not intended for search engine indexing (`robots.txt` + meta robots)

## Install on Android

### Option A — GitHub Pages (recommended)

1. Open **Settings → Pages** on the repository
2. Set **Source** to branch `main`, folder `/ (root)`
3. Wait for deploy (1–2 minutes)
4. Open the generated URL (e.g. `https://yourname.github.io/print-queue/`) in Chrome
5. Menu ⋮ → **Add to Home screen** / **Install app**

To appear in Android’s **Share** sheet, install the app this way. After an update, if Need For Print is missing from Share: remove the home icon and install the PWA again.

### Option B — Local files

1. Download the project (Download workspace)
2. Serve files over HTTP (ES modules won’t work from `file://`)
3. Open from your phone on the same network, or use static hosting

## Usage

1. Tap **+** to add a link
2. Paste the URL, enter a **title**, pick a **color**, and optional tags
3. The model appears under **To print**
4. After printing, tap **○ To print** to mark it printed
5. Use filters and tags to find what you need
6. Tap a card to open the model in the browser
7. Tap the share icon on a card to share the link

## Backup

- **↓** Export a JSON file with all models
- **↑** Import a backup (replaces the current list)

## Technical notes

- Each card shows the source site icon (works offline)
- Data stays on your phone only — no account or cloud sync

---

Built with [BrainDaemon](https://braindaemon.com)