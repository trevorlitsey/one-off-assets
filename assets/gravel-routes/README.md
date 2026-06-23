# twin cities gravel route finder

static github pages prototype for browsing public gravel / mixed-surface routes near minneapolis.

## data

- current source: public gravelmap city pages + public `/gpx/<route id>` endpoint
- drive time: OSRM estimate from an approximate pleasant ave / minneapolis home area
- surface percentage: source-estimated in this first pass; next step is OSM segment matching against route geometry using `surface`, `highway`, and `tracktype` tags

refresh data:

```bash
python3 assets/gravel-routes/scripts/scrape_gravelmap.py
```
