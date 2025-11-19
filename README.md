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
├── hwk4-task2-false-color-MILLER.ipynb
└── .gitignore
```

## Data

### Data Sources

**Landsat 8 Surface Reflectance Data**
Atmospherically corrected surface reflectance data from the Landsat 8 satellite, collected on February 23, 2025. This simplified dataset contains five spectral bands (red, green, blue, near-infrared, and shortwave infrared) from the Landsat Collection 2 Level-2 product. The data was retrieved from the Microsoft Planetary Computer data catalogue and clipped to an area surrounding the Eaton and Palisades fire perimeters. This dataset is intended for visualization and educational purposes only.

**Eaton and Palisades Fire Perimeter Data**
Dissolved fire perimeter shapefiles for the Eaton Fire and Palisades Fire that burned in Los Angeles County in January 2025. These ESRI shapefiles delineate the spatial extent of the burned areas as of January 21, 2025, and are used to overlay fire boundaries on satellite imagery for impact assessment and visualization.

### Data Access

**Landsat 8 Imagery:**
The Landsat data (`landsat8-2025-02-23-palisades-eaton.nc`) is **not included** in this repository due to file size. The data is available through the EDS 220 course shared Google Drive folder. Download the file and place it in your working directory before running the analysis notebook.

**Fire Perimeter Shapefiles:**
The fire perimeter data is **not included** in this repository. Access the shapefiles from ArcGIS Hub:
- Palisades and Eaton Dissolved Fire Perimeters: https://hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c

Download the shapefiles and store them locally to run the analysis.

**Note:** Both datasets must be downloaded separately to reproduce the analysis.

## Requirements

This analysis requires Python 3.x with the following packages:
- `xarray` - Multi-dimensional array handling and NetCDF file operations
- `rioxarray` - Geospatial raster data operations and CRS management
- `geopandas` - Vector geospatial data handling (shapefiles)
- `matplotlib` - Data visualization and plotting
- `pandas` - Data manipulation and analysis
- `numpy` - Numerical operations

## References

Bennett, M. M., Chen, J. K., Alvarez León, L. F., & Gleason, C. J. (2022). The politics of pixels: A review and agenda for critical remote sensing. *Progress in Human Geography*, *46*(3), 729–752. https://doi.org/10.1177/03091325221074691

Galaz García, C., Cawse-Nicholson, K., Frew, A., & Fontenot, R. (2024). *EDS 220: Working with environmental datasets* [Course materials]. Master of Environmental Data Science, Bren School of Environmental Science & Management, University of California, Santa Barbara. https://meds-eds-220.github.io/MEDS-eds-220-course/

NASA Earth Observatory. (n.d.). *Why is that forest red and that cloud blue? How to interpret a false-color satellite image*. https://earthobservatory.nasa.gov/features/FalseColor

Palisades and Eaton Dissolved Fire Perimeters. (2025). *Fire perimeter shapefiles* [Geospatial dataset]. ArcGIS Hub. https://hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c

U.S. Geological Survey. (2025). *Landsat 8 Collection 2 Level-2 surface reflectance data* [Satellite imagery dataset]. Microsoft Planetary Computer. https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2

## License

This project is licensed under the terms included in the LICENSE file.

---

*This project is part of the curriculum for the Master of Environmental Data Science program at the Bren School of Environmental Science & Management, UC Santa Barbara.*