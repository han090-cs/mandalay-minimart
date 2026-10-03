# CoCo Mandalay Finder

Mobile-first static website for finding CoCo Convenience Store branches in Mandalay.

## Run
No Python package or Node.js is required.

Linux/macOS:
    python3 -m http.server 8080

Then open:
    http://localhost:8080

Or deploy the whole folder to any static hosting service.

## Data
`data/shops.json` contains records collected from public online listings on 2026-10-03.

Confidence:
- verified: address/phone supported by a business directory; some also cross-checked with Foodpanda.
- online-listed: Foodpanda branch listing exists, but exact street/township/phone was not independently verified here.
- directory-listed: public directory listing exists but branch identity may need cross-checking.

IMPORTANT: This is a working initial dataset, not a claim that it contains every CoCo branch in Mandalay. Do not present the count as exhaustive until every township/branch has been cross-checked.

## Features
- Myanmar-friendly mobile UI
- Search by shop name, street, branch code, township, phone
- Township filter
- Google Maps search link
- Detail modal
- Foodpanda link when available
- No API key required
- No backend required

## v2 additions
- Brand chips: CoCo / G&G / Lar Lar / City Mart / Ocean / Capital / Minimart
- Street search accepts Burmese or English digits (e.g. "၈၄" = "84", "30x77")
- "My nearest" button uses phone GPS; Google Maps live-search buttons find every real branch near you
- Call (tel:), Foodpanda order link, share, favourites (saved on device)
- Add-your-own shops (GPS pin, saved on device) + JSON export
- Dark mode, system Myanmar font stack (no font file needed)

NOTE: shops.json has 23 CoCo + 9 G&G records (3 with confirmed addresses, 6 Foodpanda-listed only). Lar Lar / other chains are found through the live Google Maps buttons until their branches are added to shops.json (use brand_name, lat, lng fields; lat/lng enables distance sorting).
