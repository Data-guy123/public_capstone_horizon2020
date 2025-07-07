# What Are We Funding?  
## A Machine Learning Analysis of Research Outcomes in Horizon 2020 Projects

This repository contains the full code, Jupyter notebooks, and documentation for my data analytics capstone project, which explores which characteristics of Horizon 2020 research projects are most associated with research impact (publications and citations).  
The project uses open data from CORDIS and OpenAlex, advanced data cleaning, and interpretable machine learning.

---

## Project Overview

- **Goal:** Predict research outcomes (publications, citations) of Horizon 2020 projects using project metadata available at funding decision.
- **Approach:** Data wrangling, feature engineering, exploratory analysis, and model development with Random Forest (using GridSearchCV), plus interpretability via SHAP.
- **Data Sources:** 
  - [CORDIS](https://research-and-innovation.ec.europa.eu/funding/funding-opportunities/funding-programmes-and-open-calls/horizon-2020_en)
  - [OpenAlex](https://docs.openalex.org/)
- **Code Author:** Joseph A. Wright

---

## Notebooks

- `cordis_data_exploration.ipynb` – Initial data exploration and variable selection
- `capstone_data_cleaning_and_feature_table.ipynb` – Data cleaning, filtering, and feature engineering
- `data_plots.ipynb` – Descriptive statistics and visualization
- `Alexapifinalflow.ipynb` – **Main OpenAlex API extraction and bibliometrics matching** (this is the primary script for robust data collection)
- `alexcitations.ipynb` – *Test/early version of OpenAlex API extraction* (included for transparency; not used in the final workflow)
- `model_and_analysis.ipynb` – Model building, tuning (GridSearchCV), performance assessment
- `model_shap_pubs.ipynb` – SHAP interpretability analysis for publications

> **Note:** Some notebooks contain exploratory or test code and are included for transparency; follow the order above for the workflow used in the final analysis.

---

## Data

- CORDIS CSVs: Downloaded from the [EU Open Data Portal](https://data.europa.eu/data/datasets/cordis-h2020projects?locale=en)
- OpenAlex data was accessed via the [OpenAlex API](https://docs.openalex.org/).
- No raw data is distributed here due to size/licensing, but scripts are included for data extraction and cleaning.

---

## How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Data-guy123/public_capstone_horizon2020.git
   cd public_capstone_horizon2020
