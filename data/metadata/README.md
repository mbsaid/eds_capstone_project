# 📚 Metadata Documentation

## 📌 **Project**: **Climate–Livestock Dynamics in Somalia:**_Rainfall Trends and Shifts in Pastoral Livestock Stock Across Somalia (1981–2024)_
---

## 📖 Overview

This folder contains metadata documentation for all datasets used in this project. The goal is to ensure transparency, reproducibility, and clear understanding of the data.
---

## 📂 Datasets Included

| Dataset   | Description |
|----------|------------|
| CHIRPS   | Rainfall and climate data |
| FAOSTAT  | Livestock population data |
| GADM     | Administrative boundary data |

---

## 🎯 Purpose of Metadata

- Describe data sources
- Define variables and units
- Document processing steps
- Support reproducibility

---

## ⚠️ Note

All users should review metadata before using the datasets.

# ☀️ CHIRPS Rainfall Data Metadata

## 📌 Overview

Satellite-based rainfall estimates used to analyze climate variability and drought patterns in Somalia (1981–2024).
---

## 🌍 Source

| Field     | Details |
|----------|---------|
| Provider | Climate Hazards Center (UCSB) |
| Link     | [CHIRPS Data](https://www.chc.ucsb.edu/data/chirps) |

---

## 🗓 Temporal Coverage

| Start Year | End Year |
|-----------|---------|
| 1981      | 2024    |

---

## 🗺 Spatial Resolution

| Resolution | Approx. Size |
|------------|-------------|
| 0.05°      | ~5 km       |

---

## 📊 Variables

| Variable       | Description               | Unit |
|----------------|---------------------------|------|
| precipitation  | Total annual rainfall     | mm   |
| anomaly        | Deviation from long-term mean | mm |

---

## ⚙️ Processing Steps

1. Download CHIRPS raster data
2. Clip to Somalia boundary
3. Aggregate to yearly averages
4. Calculate rainfall anomalies

---

## ⚠️ Limitations

- Satellite-based estimates may contain uncertainty
- Aggregated data may mask local variability

---

## 📈 Usage in Project

- Analyze rainfall trends
- Identify drought periods
- Compare climate with livestock dynamics

# 🐄 FAOSTAT Livestock Data Metadata

## 📌 Overview

Livestock population statistics for Somalia, used to analyze long-term trends in livestock dynamics.
---

## 🌍 Source

| Field     | Details |
|----------|---------|
| Provider | Food and Agriculture Organization (FAO) |
| Link     | [FAOSTAT](https://www.fao.org/faostat/) |

---

## 🗓 Temporal Coverage

| Start Year | End Year |
|-----------|---------|
| 1981      | 2024    |

---

## 📄 Data Format

CSV (tabular data)
---

## 📊 Variables

| Variable | Description           | Unit     |
|----------|----------------------|---------|
| Year     | Observation year      | Year    |
| Species  | Livestock type        | Category|
| Value    | Number of animals     | Heads   |

---

## 🔄 Derived Variables

| Variable      | Description                |
|---------------|----------------------------|
| growth_rate   | Year-to-year change (%)    |
| log_livestock | Log-transformed livestock  |

---

## ⚙️ Processing Steps

1. Download data from FAOSTAT
2. Filter for Somalia
3. Clean and standardize dataset
4. Transform for time-series analysis

---

## ⚠️ Limitations

- National-level data only (no regional detail)
- Some values may be estimated

---

## 📈 Usage in Project

- Analyze livestock population trends
- Compare livestock with rainfall variability

# 🗺 GADM Administrative Boundaries Metadata

## 📌 Overview

Geographic boundaries for Somalia, used for spatial analysis and mapping.
---

## 🌍 Source

| Field     | Details |
|----------|---------|
| Provider | GADM    |
| Link     | [GADM](https://gadm.org/) |

---

## 📄 Data Format

Shapefile (.shp)
---

## 📊 Variables

| Variable | Description      |
|----------|-----------------|
| NAME_0   | Country name     |
| NAME_1   | Region name      |
| NAME_2   | District name    |

---

## 🌐 Coordinate System

| System | Code |
|--------|-----|
| WGS84  | EPSG:4326 |

---

## ⚙️ Usage in Project

- Clip rainfall data to Somalia
- Aggregate climate data by region
- Support GIS mapping

---

## ⚠️ Limitations

- Boundaries may not reflect recent administrative changes

# 📝 Data Dictionary

## 📊 Variables Overview

| Variable          | Description                    | Unit      |
|------------------|--------------------------------|----------|
| year             | Observation year               | Year     |
| rainfall_mm      | Annual rainfall                | mm       |
| rainfall_anomaly | Deviation from long-term mean  | mm       |
| species          | Livestock type                 | Category |
| livestock_count  | Number of animals              | Heads    |
| growth_rate      | Year-to-year livestock change  | %        |
| region           | Administrative region          | Text     |

---

## 📌 Notes

- Rainfall data is derived from CHIRPS
- Livestock data is sourced from FAOSTAT
- Spatial variables are based on GADM boundaries

