### **Climate Livestock Dynamics in Somalia: Rainfall Trends and Shifts in Pastoral Livestock Stock Across Somalia \(1981–2024\)**

Author: Mohamed Said  
Date: March 2026  

---

### Environmental Research Question: 

How do long-term rainfall trends influence density changes of goats, sheep, and camels across Somalia?
**GitHub Repository:** [Link here](https://github.com/mbsaid/eds_capstone_project)

#### Summary

This project analyzes long-term rainfall variability and its relationship with livestock population dynamics in Somalia using climate and livestock datasets. The goal is to understand how rainfall trends influence pastoral systems and livestock density changes.

#### Rationale

Somalia’s economy and livelihoods are highly dependent on pastoralism. Climate variability, particularly rainfall fluctuations and droughts, directly affects livestock health and carrying capacity. Understanding these relationships is important for improving resilience, informing policy, and supporting sustainable resource management.

#### Data Sources

- Rainfall data preprocessing (clipping, aggregation)
- Rainfall anomaly calculation
- Exploratory data analysis (EDA)
- Livestock time-series analysis
- Climate–livestock modeling (GAM)

#### Study Scope

- **Period**: `1980- 2026`
- **Location**: `Somalia (national and regional levels)`
- **Frequency**:`Annual`

#### Methodology

- Rainfall data preprocessing (clipping, aggregation)
- Rainfall anomaly calculation
- Exploratory data analysis (EDA)
- Livestock time-series analysis
- Climate–livestock modeling (GAM)
    
#### Final Analysis and Visualizations

1. Annual Rainfall Anomalies
![Annual Rainfall Anomalies](outputs/annual_rainfall_anomalies.png)

2. Observed vs GAM-fitted Livestock Stocks
![Observed vs GAM-fitted Livestock Stocks](outputs/observed_vs_gam_livestock.png)

3. Mean Raster + Highlight
![Mean Raster + Highlight](outputs/mean_raster_highlight.png)

#### File Organization

- `data/raw_data/` - Original CHIRPS rainfall and FAOSTAT livestock data
- `data/processed_data/` - Processed and transformed datasets
- `data/clean_data/` - Analysis-ready datasets
- `data/gis_data/` - Spatial data (GADM shapefiles)
- `data/metadata/` - Data documentation and descriptions
- `data/archive/` - Legacy and unused data
- `scripts/` - R scripts for data processing and analysis
- `outputs/` - Mps, figures, tables, and results
- `reports/` - RMarkdown, PDF, and presentation report
- `references/` - reference

#### Requirements

| Tool           | Purpose                                |
|----------------|----------------------------------------|
| `R`            | Data analysis and modeling             |
|`Bash / Python` | File management and Git operations     |
| `CoCalc`       | Cloud-based development environment    |
|`Git & GitHub`  | Version control and project management |

#### Ethical

| **Aspect**  | **Description**                                    |
| :----------:| ---------------------------------------------------|
| Privacy     | No personal data is included                       |
| Governance  | Data is openly available and ethically sourced     |
| Bias        | Potential dataset and analytical biases considered |

#### Contact


Mohamed Said  
[Email](mbsaid@gmail.com) 
[Linkedin](https://www.linkedin.com/in/mohamed-said-613895156/)

#### License

MIT License

_Copyright © 2026 Mohamed Said. All rights reserved_


