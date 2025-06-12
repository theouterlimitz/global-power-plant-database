# Capstone Project: Analyzing Water Risk Exposure of Global Power Plant Infrastructure

## Project Overview

This repository hosts the work for my Data Science Capstone project. The primary goal of this project is to analyze the exposure of global power plant infrastructure to current and future water-related risks. This involves integrating detailed data on power plants worldwide with comprehensive water risk indicators to identify potential vulnerabilities and highlight areas of concern at the intersection of energy production and water scarcity.

This repository is a fork of the World Resources Institute's (WRI) [Global Power Plant Database](https://github.com/wri/global-power-plant-database).

## Project Status (As of June 2025)

* [x] **Project Description & Scoping:** Complete & Submitted
* [x] **Data Curation:** Complete & Submitted
* [ ] **Exploratory Data Analysis (EDA) Deliverable:** In Progress
* [ ] **Datafolio & Dashboard:** In Progress
* [ ] **Final Report:** Not Started

## Key Findings from Exploratory Data Analysis

Our analysis has uncovered several key insights into the water risk faced by the global power fleet:

1.  **Risk Varies by Fuel Type:** Thermal fossil fuels (Coal, Gas, Oil) and Solar power plants have the highest average baseline water stress scores. Wind power has the lowest risk profile, while Hydropower's risk is more moderately distributed.
2.  **Risk is Geographically Concentrated:** The highest-risk power plants are not evenly distributed but are concentrated in major global hotspots, including India, Northern China, the Middle East, and North Africa.
3.  **Future Risk is Scenario-Dependent:** The future risk profile changes dramatically based on the climate and socioeconomic pathway. A "Pessimistic" 2050 scenario shows a significant increase in the total power capacity under "Extremely High" stress, while an "Optimistic" scenario shows a tangible reduction in risk.

## Datasets Used

1.  **WRI Global Power Plant Database (GPPD):** This database provides locations, capacities, fuel types, and other attributes for ~35,000 power plants worldwide.
2.  **WRI Aqueduct 4.0 Water Risk Atlas:** This dataset provides detailed global water risk indicators at the hydrological basin level, including baseline historical trends and future projections under three different climate scenarios.
3.  **HydroBASINS Level 6:** Geospatial data used to link power plant locations to their corresponding water basins.

## Methodology & Tools

The project followed a structured data analysis workflow within a Python environment.

1.  **Data Curation:** Raw data from all sources was loaded, cleaned, and merged. Key steps included handling special numeric codes, remediating data anomalies, performing a geospatial join using `GeoPandas`, and performing attribute joins. The final, cleaned, and merged dataset was saved to `analytical_data.pkl` to streamline all subsequent analysis.

2.  **Exploratory Data Analysis (EDA):** Insights were generated using `pandas`, `matplotlib`, and `seaborn`. This involved creating visualizations to understand risk distribution by fuel type, geography, and across future scenarios.

3.  **Dashboarding:** An interactive dashboard was built using [Looker Studio](https://lookerstudio.google.com/reporting/db75b288-9c6b-4b15-8dd8-f35e03fd3b10) to present the key findings. This involved connecting a prepared CSV file and building several charts, maps, KPIs, and filters.

## Repository Contents

* **/deliverables/**: Contains the `.ipynb` notebook files for the Data Curation and EDA deliverables.
* **Final Interactive Dashboard:** [View the Dashboard on Looker Studio](https://lookerstudio.google.com/reporting/db75b288-9c6b-4b15-8dd8-f35e03fd3b10)
