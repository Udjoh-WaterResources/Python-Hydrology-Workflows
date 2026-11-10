# Python for Hydrology & Water Resources
Automated hydrological analysis and spatial data processing using Python. Features SMHI API integration, watershed delineation with Pysheds, and geospatial data visualization

## 📌 Project Overview
This repository contains a collection of Python workflows designed to automate hydrological data analysis, spatial mapping, and climate data extraction. These scripts demonstrate the transition from traditional GUI-based GIS software (like QGIS) to programmatic, reproducible data science.

## 🛠️ Technical Stack
*   **Data Analysis:** `pandas`, `numpy`
*   **Data Visualization:** `matplotlib`
*   **API & Web Requests:** `requests`
*   **Geospatial Analysis:** `geopandas`, `rasterio`, `shapely`
*   **Hydrological Modeling:** `pysheds`, `elevation`

## 🚀 Key Workflows Demonstrated

### 1. Climate Data Processing (Pandas)
*   Loaded and filtered 70+ years of daily weather data.
*   Calculated rolling averages, max/min statistics, and filtered specific timeframes (e.g., seasonal temperature curves).

### 2. Automated API Integration (SMHI)
*   Connected directly to the Swedish Meteorological and Hydrological Institute (SMHI) Open Data API.
*   Parsed complex JSON responses into clean Pandas DataFrames.
*   Plotted precipitation bar charts for Stockholm automatically, removing the need for manual CSV downloads.

### 3. Spatial Hydrology & DEM Processing (GeoPandas & Pysheds)
*   Downloaded Digital Elevation Models (DEMs) for specific regions (Gothenburg, Sweden; Ajah, Nigeria).
*   Calculated catchment areas in metric units (km²) using coordinate reprojection (UTM).
*   Executed a full hydrological terrain analysis workflow in Python:
    *   **Fill Sinks:** Handled artificial pits in raw satellite data.
    *   **Flow Direction:** Calculated D8 flow paths.
    *   **Flow Accumulation:** Generated stream networks automatically.
    *   **Watershed Delineation:** Extracted specific catchment boundaries based on outlet points.

## 💻 How to Use
All notebooks are designed to run in **Google Colab**. You do not need to install any software locally. Simply open the `.ipynb` file in Colab and run the cells sequentially. 

## 🔮 Future Additions
*   **Phase 4:** Extreme Value Analysis (Flood Frequency curves using `scipy.stats`).
*   **Phase 5:** Capstone Project (Automated flood risk assessment tool).
