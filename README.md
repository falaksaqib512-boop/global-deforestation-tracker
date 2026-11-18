
# Global Deforestation Tracker: GEE + Python

## Project Overview
This project uses Google Earth Engine and Python to detect and map canopy loss worldwide from satellite imagery. It compares vegetation cover across time periods and highlights areas of change on an interactive global map.

## Key Findings
- Mapped canopy loss at a global scale using satellite imagery from 2020 to present.
- Loss clusters appear across Southeast Asia, eastern China, India, and other regions visible on the map.
- Results varied by region and land-cover type.

## Tools & Technologies
- **Google Earth Engine (GEE) API:** cloud-based satellite data processing
- **Python:** geemap for interactive mapping, pandas for data handling, rasterio for raster data
- **Data:** Sentinel-2 and Landsat 8/9 surface reflectance imagery

## Analysis

### Data Collection
Sentinel-2 and Landsat 8/9 surface reflectance imagery was filtered by date and cloud cover, then combined into composites for each period.

### Canopy Change Detection
Vegetation indices ([NDVI]) were calculated for each period. The difference between periods was thresholded to flag areas of canopy loss, shown in red on the map. The map is visualized at [X] m scale.

## Visualizations

### Global Deforestation Map
![Global Deforestation Map](images/map.png)

## Project Workflow
```
Satellite Imagery (Sentinel-2, Landsat 8/9)
        ↓
Google Earth Engine (Filtering & Composites)
        ↓
Vegetation Index Calculation
        ↓
Change Detection (Thresholding)
        ↓
geemap (Interactive Map Rendering)
        ↓
Insights & Visualization
```

## Skills Demonstrated
- Google Earth Engine and cloud-based geospatial analysis
- Remote sensing and satellite image processing
- Vegetation change detection
- Python programming (geemap, pandas, rasterio)
- Geospatial data visualization
- Environmental and forestry monitoring

## Limitations
- Change detection based on vegetation indices can also flag cropland, urban change, and seasonal variation, not only forest loss.
- Results are intended for visual exploration, not as validated deforestation statistics.

## Conclusion
This project shows how Google Earth Engine and Python can turn global satellite imagery into practical insights on vegetation and canopy change.

## Author
Syeda Falak Saqib
[LinkedIn](https://www.linkedin.com/in/syeda-falak-saqib-01b67a2a5)
