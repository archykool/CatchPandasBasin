# Catch Basin Pandas
### Mapping the Drainage Breakdown Loop in East Harlem

**Winner — Best Incorporation of Risk Assessment + Projection**
Urban Futures Hackathon: Co-Creating Climate Resilience in NYC
American Museum of Natural History and Columbia University, New York | January 2026

---

The goal of this project was to leverage NYC Open Data to highlight a community-identified environmental justice issue in East Harlem. Community reporting (interviews with the project’s community partners, 311 Data, DSNY Litter Basket Data) indicates that public waste bins are sparse or have been removed, residential trash pickup is inconsistent, and street litter is a persistent issue. To estimate how likely litter is to enter storm drains, we measured the distance between catch basins and public trash bins. In East Harlem, the average distance was 46.7 meters, compared to 19.8 meters in the neighboring Upper East Side. We defined high clogging risk as catch basins with no trash bin within a 50-meter radius. Overlaying these high-risk basins with current and projected stormwater flood zones demonstrates that these areas also have conditions that make drainage failure due to clogging more likely. Compounding flood vulnerability in East Harlem demonstrates how inequitable city sanitation services are a climate risk.  

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
