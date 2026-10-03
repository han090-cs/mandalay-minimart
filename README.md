# Mandalay Minimart Finder

A mobile-first, static directory for **mini market / minimart / convenience-store listings inside Mandalay**.

## GitHub Pages deployment

This project has no build step and no API key. Put `index.html` and `shops.json` in the **root of the repository**.

On GitHub:

1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select your publishing branch (usually `main`) and the folder **`/(root)`**.
4. Click **Save**.

GitHub Pages uses the repository's top-level `index.html` as the site entry file when publishing from the repository root.

## Files

- `index.html` — the website
- `shops.json` — Mandalay-only mini-market dataset
- `MANDALAY_MINIMART_SOURCES.md` — data sources and filtering notes

## Features

- Mandalay-only filtering at data-load and UI-render layers
- Search by shop name, address, township, phone, or branch
- Brand and township filters generated from the dataset
- Nearby sorting using browser GPS
- Google Maps links
- Favorites saved in the browser
- Add a local mini-market entry on your device
- Share a listing
- Responsive mobile/desktop UI
- No framework, backend, or API key required

## Data scope

The bundled dataset contains **101 active records** from the source-merged dataset prepared for this project. It is not an official registry and cannot guarantee every unlisted/new shop.

The application only accepts records where:

- `city_mm` is `မန္တလေး`
- `category` is `mini_market`
- `status` is `active`

User-added records are stored only in the browser's local storage.

## Local test

Do not open `index.html` with `file://` when testing the JSON loader. Run a local static server instead:

```bash
python3 -m http.server 8080
```

Then open:

```text
http://localhost:8080
```
