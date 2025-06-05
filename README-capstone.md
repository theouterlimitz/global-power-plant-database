# Capstone Project: Analyzing Water Risk Exposure of Global Power Plant Infrastructure

## Project Overview

This repository hosts the work for my Data Science Capstone project. The primary goal of this project is to analyze the exposure of global power plant infrastructure to current and future water-related risks. This involves integrating detailed data on power plants worldwide with comprehensive water risk indicators to identify potential vulnerabilities and highlight areas of concern at the intersection of energy production and water scarcity.

This repository is a fork of the World Resources Institute's (WRI) [Global Power Plant Database](https://github.com/wri/global-power-plant-database).

## Purpose of this Fork

This fork serves as the central workspace for:
* Data curation and preprocessing scripts.
* Exploratory data analysis (EDA) notebooks.
* Project documentation and deliverables.
* Storing any developed models or dashboards (or links to them).

## Key Research Questions (Tentative)

* What is the current level of water stress and other water risks faced by different types of power plants globally and in specific regions?
* How might these water risks change for existing power infrastructure under various future climate and socioeconomic scenarios (e.g., 2030, 2050, 2080)?
* Are there particular types of power plants or geographical regions that are disproportionately vulnerable to water scarcity?
* What are the potential implications of these water risks for energy security and sustainable development?

## Datasets Used

1.  **WRI Global Power Plant Database:** This comprehensive database provides locations, capacities, fuel types, commissioning years, and other information for tens of thousands of power plants worldwide. (Forked from [wri/global-power-plant-database](https://github.com/wri/global-power-plant-database))
2.  **WRI Aqueduct 4.0 Water Risk Atlas:** This dataset provides detailed global water risk indicators, including:
    * Baseline water stress, water depletion, inter-annual variability, and seasonal variability (both monthly and annualized).
    * Future projections of these water risks under different climate scenarios (e.g., SSPs/RCPs) and for various time horizons (e.g., 2030, 2050, 2080).

## Methodology & Tools

The project will involve the following general steps:

1.  **Data Acquisition and Preprocessing:**
    * Cleaning and preparing the Global Power Plant Database.
    * Processing and understanding the Aqueduct 4.0 water risk data (baseline and future projections).
    * Geospatially linking power plant locations (latitude/longitude) to the relevant water basin identifiers (`pfaf_id`) from the Aqueduct dataset. This will likely involve using Pfafstetter basin shapefiles.
    * Merging the power plant data with the water risk indicators.
2.  **Exploratory Data Analysis (EDA):**
