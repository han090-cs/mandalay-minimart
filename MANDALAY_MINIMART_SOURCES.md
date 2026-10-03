# Mandalay Mini-Market Dataset

Updated: 2026-10-03

This project is intentionally scoped to **Mandalay** and to businesses listed as **mini market / minimart / convenience store**.

## Dataset size

101 distinct active records are included after merging duplicate listings.

## Sources searched

- Google Maps indexed business listings
- Food Industry Directory
- Mandalay Directory
- OpenStreetMap / OpenAlfa
- BizSouthAsia
- Hearty Heart directory
- Supermyan directory
- AEON MFI agent directory
- MyanmarYP
- DENKO official location directory

## Filtering rules

- `city_mm` must be Mandalay.
- Category is `mini_market`.
- Clearly closed listings are excluded.
- Supermarkets, department stores, wholesalers, hotel-supply stores, and other non-mini-market uses are excluded when the indexed source clearly categorized them that way.
- Some directory-only entries have township-level addresses because the indexed directory result did not expose a reliable street-level address; these are marked `medium` or `low` confidence and should be field-verified before treating them as exact locations.

## Important limitation

No public index can guarantee every tiny neighborhood shop, newly opened shop, or unlisted shop. This is therefore a broad, source-merged **Mandalay mini-market dataset**, not a mathematically exhaustive census.
