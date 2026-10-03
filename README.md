# Myanmar Minimart Finder

A mobile-first static web app for finding convenience stores and minimarts across Myanmar, with an emphasis on CoCo, G&G, Lar Lar, City Mart, Ocean, and other local minimart brands.

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
- Search by shop name, address, township, phone number, city, or state
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

This project uses a working directory dataset stored in `shops.json`.

It is intended for local discovery and demo use, and the dataset should be treated as an evolving directory rather than a fully exhaustive national registry. The app is designed to make it easy to update and expand over time as more verified information becomes available.

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

- Verified: linked to a reliable directory and/or cross-checked with public sources
- Online-listed: appears in a Foodpanda or online branch listing but may need further verification
- Directory-listed: present in a directory listing, but exact branch details may still need confirmation

## Why this is useful

- Easy to browse on mobile devices
- Helpful for people looking for nearby minimart branches
- Good for a personal project, local community listing, or small-scale demo
- Lightweight and easy to deploy on GitHub Pages, Netlify, or a simple static web host

## License

This project is provided as-is for demo, local use, and community-focused development.
