# Catch Basin Pandas
### Mapping the Drainage Breakdown Loop in East Harlem

**Winner — Best Incorporation of Risk Assessment + Projection**
Urban Futures Hackathon: Co-Creating Climate Resilience in NYC
American Museum of Natural History, New York | January 2026

---

East Harlem (MH11) sits at the intersection of two compounding crises: a chronic shortage of street-level trash infrastructure and a growing flood risk from clogged catch basins. This project traces the full cascade — from overflowing litter baskets to blocked sewers to neighborhood-scale flooding — using 2025 NYC 311 service request data, NYCDEP catch basin records, and DSNY litter basket locations. By overlaying 311 sanitation complaint hotspots with stormwater flood projections, we identify which catch basins are at highest clogging risk and give the community a tool to act before the next cloudburst.

---
## Interactive Map
please check our GIS Map here!  https://storymaps.arcgis.com/stories/b7f751120eee4a51a45a4ef2c210003b

---
![Problem Define](slides/BLUE_WHALE_Presentation%20%282%29.png)

![Data and Tools](slides/BLUE_WHALE_Presentation%20%283%29.png)

![Litter Basket Distribution](slides/BLUE_WHALE_Presentation%20%284%29.png)

![Trash Vulnerability](slides/BLUE_WHALE_Presentation%20%285%29.png)

![Catch Basin Identification](slides/BLUE_WHALE_Presentation%20%286%29.png)

![Clogged Basins Flood Risk](slides/BLUE_WHALE_Presentation%20%287%29.png)

![Actionable Insights](slides/BLUE_WHALE_Presentation%20%288%29.png)

---


## Repository Structure

| File | Description |
|------|-------------|
| `311_2025_sanitation_filtering.ipynb` | Filter 3.5M raw 311 records to ~730K sanitation complaints |
| `311_2025_sanitation_modeling.ipynb` | Seasonal analysis, sub-category bucketing, spatial join with NTAs and catch basins |
| `Convert_Format.ipynb` | Convert NTA CSV with WKT geometry to ESRI Shapefile |
| `slides/` | Presentation slides from Urban Futures final presentations |
| `Materials/` | Reference materials — 1865 Viele Map, East Harlem Resiliency Study, data links |

> Large data files (CSV, Parquet, Shapefile) are excluded via `.gitignore`. Only notebooks, slides, and materials are tracked.

## Team

Archy Guo · Charlotte Rhoads · Raheem Williams · Tracy Obirika

LEAP Blue Whales — January 2026
