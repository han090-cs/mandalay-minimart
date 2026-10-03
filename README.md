# Mandalay Minimart Finder

Mobile-first static website for finding convenience stores and minimarts in Mandalay, with emphasis on CoCo, G&G, Lar Lar, City Mart, Ocean, Capital, and other local minimart brands.

## Live demo

To run locally:

```bash
python3 -m http.server 8080
```

Then open:

```text
http://localhost:8080
```

## Features

- Mobile-friendly Myanmar UI
- Search by shop name, address, township, phone number, or branch code
- Brand filters for CoCo, G&G, Lar Lar, City Mart, Ocean, Capital, and minimart brands
- Nearby shop lookup using browser GPS
- Quick Google Maps links
- Foodpanda links when available
- Share functionality
- Favorite-saving on the device
- Add-your-own shop entry with local storage
- Dark mode and responsive layout
- No backend or API key required

## Data note

This project uses a working directory dataset stored in `shops.json` for Mandalay only.

It is intended for local discovery and demo use. The dataset should be treated as an evolving directory rather than a fully exhaustive registry. The app is designed to make it easy to update and expand store information over time.

## Project structure

```text
.
├── index.html
├── shops.json
├── README.md
├── manifest.webmanifest
└── .gitignore
```

## Data quality notes

- Verified: address and phone supported by directory listings or other public references
- Online-listed: listing exists online but exact branch details were not independently verified here
- Directory-listed: public directory listing exists but branch identity may need further checking

## Share

You can share this project with friends using the repository link:

```text
https://github.com/han090-cs/mandalay-minimart
```

For a live hosted version, deploy the folder to GitHub Pages or any static web host.
