# False Color Visualization of the 2025 Los Angeles Wildfires

## About

This repository contains a Jupyter notebook that creates false color imagery to visualize fire scars from the Eaton and Palisades fires that burned in Los Angeles County in January 2025. The analysis uses Landsat 8 satellite data to highlight burn severity and vegetation impacts through infrared band composites.

**Key outputs:**
- True color composite of the fire area
- False color composite (SWIR/NIR/Red) highlighting fire scars
- Map overlaying fire perimeters on false color imagery

This project was completed as part of EDS 220: Working with Environmental Datasets at the Bren School of Environmental Science & Management, UC Santa Barbara.

## Repository Structure
```
eds220-hwk4/
│
├── README.md
├── hwk4-task2-false-color-[YOURLASTNAME].ipynb
└── .gitignore
```

## Data

**Landsat 8 Surface Reflectance Data:**
- File: `landsat8-2025-02-23-palisades-eaton.nc`
- Source: Microsoft Planetary Computer (Landsat Collection 2 Level-2)
- Access: Available via course shared Google Drive
- Bands included: Red, Green, Blue, Near-Infrared (NIR), Shortwave Infrared (SWIR)
- Date: February 23, 2025
- Note: Pre-clipped to fire perimeter area; for educational use only

**Fire Perimeter Data:**
- Files: `Eaton_Perimeter_20250121.shp`, `Palisades_Perimeter_20250121.shp`
- Source: ArcGIS Hub - Palisades and Eaton Dissolved Fire Perimeters
- Date: January 21, 2025
- Format: ESRI Shapefile
- Access: https://hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c

## References

Course materials from EDS 220: Working with Environmental Datasets, Bren School of Environmental Science & Management, UC Santa Barbara.

Landsat 8 data retrieved from Microsoft Planetary Computer. Original data from U.S. Geological Survey.

Palisades and Eaton Dissolved Fire Perimeters (2025). ArcGIS Hub. Retrieved from https://hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c
