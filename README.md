# 🌋 Global Earthquake Analysis (1900-2014)

![Earthquake Analysis Dashboard](Screenshot 2026-03-14 175300.png)

## 📖 Project Overview
This project provides a comprehensive exploration of global seismic activity over nearly a century (1900-2014). By leveraging a massive dataset of ~8,300 earthquake records, we analyze the relationship between earthquake magnitude, depth, and geographical frequency to identify high-risk zones across the globe.

---

## 🛠️ Tech Stack & Source
- **Visualization Tool**: Tableau Desktop / Packaged Workbook (`.twbx`)
- **Data Source**: [USGS Earthquake Database via Kaggle](https://www.kaggle.com/datasets/varunsaikanuri/earthquakes-from-1900-2013)
- **Data Format**: CSV (containing Latitude, Longitude, Mag, Depth, etc.)

---

## 🚀 Step-by-Step Implementation

### Phase 1: Data Acquisition
1.  **Download**: Visit the Kaggle dataset link and download the `database.csv` (or similar archive).
2.  **Refine**: Ensure the dataset includes columns for `Date`, `Time`, `Latitude`, `Longitude`, `Magnitude`, and `Depth`.
3.  **Prepare**: Rename the file to `Earthquakes.csv` for consistency with this project.

### Phase 2: Exploratory Data Analysis (EDA)
Before visualization, the data was analyzed to identify:
- **Spatial Clusters**: Identifying "The Ring of Fire" and other tectonic hotspots.
- **Magnitude Trends**: Understanding the distribution of earthquakes (e.g., frequency of 6.0+ vs. 8.0+ events).
- **Depth-Magnitude Correlation**: Investigating if deeper earthquakes tend to have higher or lower magnitudes.

### Phase 3: Interactive Tableau Dashboard
The final dashboard (`Earthquake Analysis.twbx`) is composed of four key analytical views:

1.  **🌍 Geological Visualization**: A global map using Mapbox integration to plot every earthquake. Markers are color-weighted to show intensity, highlighting the heavy concentration of events along tectonic boundaries.
2.  **📊 Regional Treemap**: A visualization of countries with the highest occurrence of earthquakes. High-frequency regions like **Indonesia**, **Papua New Guinea**, and **Japan** are dominant.
3.  **📈 Relation Plot (Depth vs. Magnitude)**: A scatter plot displaying the correlation between the depth of the seismic source and its magnitude. A magnitude filter allows users to isolate specific intensity levels.
4.  **🏙️ High-Impact Analysis**: A bar chart focusing on the "Top 6 Countries" with earthquakes greater than 7.0 on the Richter scale, binned by magnitude for clarity.

---

## 📁 Repository Structure
- `Earthquakes.csv`: The processed raw dataset.
- `Earthquake Analysis.twbx`: The interactive Tableau dashboard file.
- `dashboard_preview.png`: Preview image of the final analysis.

---

## 📝 Conclusion
This project demonstrates how raw seismic data can be transformed into actionable insights. The interactive nature of the Tableau dashboard allows researchers and curious minds alike to drill down into specific regions and historical events to better understand one of nature's most powerful forces.