# CatchPandasBasin

**NYC Sanitation & Catch Basin Analysis — 2025 311 Data**

This project analyzes New York City's 311 service request data (2025) to identify patterns in sanitation complaints — illegal dumping, missed collections, sewer issues, rodent activity, and more — and spatially correlates them with the city's catch basin infrastructure.

The pipeline filters 3.5 million raw 311 records down to ~730K sanitation-related complaints, enriches them with neighborhood (NTA) boundaries, and produces geospatial outputs (Shapefiles, GeoDataFrames) ready for GIS analysis.

## Project Structure

| File | Description |
|------|-------------|
| `311_2025_sanitation_filtering.ipynb` | Load raw 311 parquet, filter to sanitation complaint types, export `311_2025_sanitation.csv` |
| `311_2025_sanitation_modeling.ipynb` | Seasonal analysis, sub-category bucketing, spatial join with NTAs and catch basins |
| `Convert_Format.ipynb` | Convert NTA CSV with WKT geometry to a clean ESRI Shapefile |
| `Materials/` | Reference materials — 1865 Viele Map, East Harlem Resiliency Study, data source links |

## Data Sources

- [NYC 311 Service Requests (Open Data)](https://data.cityofnewyork.us/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9)
- [NYCDEP Citywide Catch Basins](https://data.cityofnewyork.us/)
- [2020 Neighborhood Tabulation Areas (NTAs)](https://data.cityofnewyork.us/)
- [DSNY Litter Basket Inventory](https://data.cityofnewyork.us/)

## Displaying the GIS Map

GitHub natively renders `.geojson` files as interactive Leaflet maps. To add a live map to this repo:

1. Export a GeoJSON of your points or polygons (e.g. from GeoPandas):
   ```python
   gdf.to_file("map_preview.geojson", driver="GeoJSON")
   ```
2. Commit and push `map_preview.geojson` to the repo.
3. Clicking it on GitHub will show an interactive map automatically.

For a static map preview embedded in this README, export a PNG from your notebook and add it here:

```markdown
![NYC Sanitation Complaints 2025](assets/map_preview.png)
```

> **Note:** Large datasets (3.5M rows) are excluded from this repo via `.gitignore`. Only notebooks, materials, and lightweight exports are tracked.

## Team

LEAP Blue Whales — NYU, Jan 2026
