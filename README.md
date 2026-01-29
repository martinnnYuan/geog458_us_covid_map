# GEOG 458 Lab 03 - US COVID-19 Maps

These two maps are visualizing 2020 COVID-19 cases and case rates across U.S. counties. The project includes two Mapbox GL JS maps: a choropleth of case rates and a proportional symbol map of total cases.

## Live Maps
- Choropleth (case rate): `map1.html`
- Proportional symbols (total cases): `map2.html`

## Screenshots
- `img/map1.png`
- `img/map2.png`

## Primary Functions
- Load GeoJSON and DBF in parallel using `fetch()` + `Promise.all()`.
- Parse DBF records in the browser using `DataView` + `TextDecoder` and join them to geometries (not covered in lecture).
- Build a choropleth with Mapbox GL JS `step` expressions for case rate styling.
- Create a legend for both maps based on the symbol/color breaks.
- Add interaction: hover tooltip for the choropleth and click popups for the proportional symbols.
- Use an Albers projection for the choropleth map.

## Libraries and APIs
- Mapbox GL JS
- Web APIs: Fetch, Promise.all, DataView, TextDecoder

## Data Sources
- COVID-19 case counts and rates (2020) from The New York Times COVID-19 dataset (see map legend in `map2.html`).
- County geometries and attribute tables included in `assets/`.

## File Structure
- `map1.html`: Choropleth of county-level case rates (per 1,000 people).
- `map2.html`: Proportional-symbol map of county-level case counts.
- `assets/us-covid-2020-rates.json` and `assets/us-covid-2020-counts.json`: GeoJSON geometries.
- `assets/us-covid-2020-rates/` and `assets/us-covid-2020-counts/`: DBF attribute tables.

## Credits
- The New York Times COVID-19 data team.
- Mapbox for basemaps and WebGL rendering.
- GEOG 458 course materials and instructors.

## Acknowledgments
Thank you to the GEOG 458 teaching team and classmates for feedback and troubleshooting tips.
