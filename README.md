# World_Happiness_Report

## Project Overview

**World_Hapiness_Report** is a data analysis project based on the **World Happiness Report (2015–2023)**.
It studies global happiness levels, their dispersion across countries, and the key economic, social, and institutional factors that drive well-being.

The project combines data preparation, exploratory data analysis, KPIs, and visualizations to support **data-driven insights and public policy recommendations**.

---

## Objectives

- Study happiness as an indicator of human development and social well-being
- Measure the level and dispersion of happiness scores across countries and years
- Identify the main determinants of happiness (economic, social, health, institutional)
- Build KPIs and visualizations highlighting disparities between the most and least happy countries
- Propose analytical directions for predictive and explanatory models
  (time series, regression, classification, machine learning)

---

## Data

- **Source**: World Happiness Report datasets (open data via Kaggle), a widely recognized international reference
- **Period covered**: 2015–2023
  - 9 annual datasets merged with consistent variables
- **Granularity**:
  - One observation per country and per year
  - Global coverage with annual frequency

### Main Variables

- `happiness_score` – Global happiness score (target variable)
- `country`, `region` – Country name and geographic region
- `year` – Year of observation (temporal analysis)
- `gdp_per_capita` – Proxy for wealth and economic living conditions
- `social_support` – Quality of social and family support
- `healthy_life_expectancy` – Expected years of healthy life
- `freedom_to_make_life_choices` – Perceived freedom in life decisions
- `perceptions_of_corruption` – Perceived corruption and institutional trust

---

## Repository Structure

```text
World_Hapiness_Report/
├─ raw_datasets/
│  ├─ WHR_2015.xls
│  ├─ WHR_2016.xls
│  ├─ WHR_2017.xls
│  ├─ WHR_2018.xls
│  ├─ WHR_2019.xls
│  ├─ WHR_2020.xls
│  ├─ WHR_2021.xls
│  ├─ WHR_2022.xls
│  └─ WHR_2023.xls
├─ data_merging.ipynb
├─ whr_2015_2023.xls
└─ world_hapiness_report_2015_2023.ipynb
```

---

# KPIs and Analysis

## KPI 1 – Dispersion of Happiness by Year
- Boxplots of happiness scores (2015–2023)
- High dispersion until 2019
- Greater homogeneity between 2020 and 2022
- Renewed widening of disparities in 2023

## KPI 2 – Country Rankings (Top 10 / Bottom 10)
- Horizontal bar charts of the 10 happiest and 10 least happy countries
- Top 10 scores are high and concentrated (≈ 6.2–7.5)
- Bottom 10 scores are very low (≈ 3.0–3.7)
- Persistent structural gaps in well-being

## KPI 3 – Evolution of Global Happiness
- Line chart of average happiness by year
- Stability in 2015–2016
- Slight dip in 2017
- Improvement from 2018
- Peak in 2022 and slight decrease in 2023 (still above earlier levels)

## KPI 4 – Key Drivers of Happiness
- Correlation heatmap between happiness and explanatory variables
- Strongest correlations:
  - GDP per capita (≈ 0.72)
  - Healthy life expectancy (≈ 0.68)
  - Social support (≈ 0.65)
- Perceptions of corruption show a weaker but meaningful effect (≈ 0.42)

## KPI 5 – Gap Between Top 10 and Bottom 10
- Bar charts and range plots comparing group averages
- The average score of the Top 10 is more than double that of the Bottom 10
- Clear visual separation highlights deep structural inequalities

---

# Recommendations and Future Work
- Automate monitoring of dispersion metrics (variance, standard deviation) and combine them with forecasting models (e.g., ARIMA)
- Develop supervised learning models (regression or classification) using GDP, health, social support, and freedom to detect vulnerable countries
- Apply multivariate time-series models to track happiness trajectories by country or region beyond 2023
- Build predictive and explanatory models (linear regression, machine learning) to quantify the influence of each factor and compare their importance over time

---

# Tools & Skills Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- Data cleaning & merging
- Exploratory Data Analysis (EDA)
- KPI design
- Data visualization
- Statistical correlation analysis

---

# License
This project is for academic and educational purposes using publicly available data.
