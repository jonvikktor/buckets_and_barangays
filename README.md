# Buckets & Barangays

A scrollytelling story testing whether the Philippines really has the most basketball courts per capita in the world — built with live OpenStreetMap data for the Lede Program at Columbia University.

**[Read the story →](#)** *(add your GitHub Pages link once it's live)*

Finding: Metro Manila actually trails the national rate — 15.7 courts per 100,000 residents vs. 21.3 nationwide.

## Files

- `index.html` — the scrollytelling page (Mapbox GL JS + Scrollama.js)
- `basketball_courts.ipynb` — collects and analyzes the data live via the Overpass API
- `*.geojson`, `*.csv`, `NCR_1.xlsx` — data the page and notebook load
- `photos/`, `basketball_banner.mp4` — media used in the story, credited on the page

## Running locally

`index.html` fetches its data files, which browsers block over `file://`. Serve the folder instead:

```bash
python3 -m http.server 4176
```

Then open `http://localhost:4176/index.html`.

## Data sources

- Basketball courts: [OpenStreetMap](https://www.openstreetmap.org/copyright), via the Overpass API
- Population and land area: Philippine Statistics Authority, 2024 Census of Population

## Author

Jon Viktor D. Cabuenas
