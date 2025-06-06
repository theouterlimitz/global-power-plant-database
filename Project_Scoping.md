Capstone Project Scoping Document
This document clarifies the project's problem statement and outlines the proposed solution, considering its feasibility, impact, and usability within the project timeframe.

1. Business Problem
The global energy sector, a cornerstone of modern economic and social stability, has a critical and often underestimated vulnerability: its dependence on reliable water resources. This "water-energy nexus" presents a growing challenge as climate change and increasing demand intensify water stress globally. While this systemic risk is acknowledged, there is a significant gap in the granular, plant-level assessment of water risk exposure for existing energy infrastructure.

This project addresses the specific problem of quantifying the current and projected future water risks—including water stress, depletion, and variability—for a comprehensive portfolio of global power plants. The goal is to move beyond high-level national averages and provide specific insights into which types of power generation facilities, located in which specific hydrological basins, are most vulnerable to water challenges now and through the end of the century.

2. Business Impact
The primary benefit of this analysis will be the creation of a detailed, data-driven water risk assessment for global power infrastructure, enabling stakeholders to make more informed decisions. The specific impacts include:

Enhanced Energy Security: By identifying which power plants are in current or future water-risk hotspots, energy operators and grid planners can better anticipate potential disruptions, reduced operational efficiencies, or plant shutdowns, leading to more resilient energy systems.
Informed Investment and Policy: The analysis will provide valuable intelligence for investors assessing the long-term viability of energy assets and for policymakers developing water management and climate adaptation strategies for the energy sector.
Support for Sustainable Development: The project directly supports Sustainable Development Goals (SDGs) related to water (SDG 6), energy (SDG 7), and climate action (SDG 13).
Strategic De-risking: For energy companies, this analysis can inform strategic decisions about their portfolio of assets, including where to prioritize water-efficiency upgrades or where to site new, less water-intensive power generation facilities.
3. Data
The analysis will be based on publicly available datasets from the World Resources Institute (WRI), a reputable source for global environmental and development data. The core datasets we will be working with are:

WRI Global Power Plant Database (GPPD): This dataset provides detailed information for approximately 35,000 power plants worldwide, including their specific location (latitude, longitude), capacity, primary fuel type, and operational status.
WRI Aqueduct 4.0 Water Risk Atlas: We will utilize several basin-level (pfaf_id) outputs from this suite:
Baseline Monthly Data: Provides historical trend data (1979-2019) for key water risk indicators like water stress, depletion, and interannual variability on a monthly basis.
Future Annual Data: Provides future projections for water risk indicators under various climate and socioeconomic scenarios (optimistic, business-as-usual, pessimistic) for milestone periods centered around 2030, 2050, and 2080.
Baseline Annual Data: This comprehensive dataset, containing all 13 of Aqueduct's baseline annual indicators (including flood, drought, and water quality risks) and industry-specific weighting schemes (including one for "Electric Power"), will also be incorporated for a holistic risk assessment.
Supporting Geospatial Data: HydroBASIN Level 6 shapefiles will be required to perform the geospatial join between the power plant point data and the Aqueduct basin-level risk data.
These datasets represent the initial plan for this analysis, and additional contextual datasets may be considered if necessary. Initial reviews and data dictionary analyses have been completed for all core datasets.

4. Methods
The methodology for this project will follow a structured data analysis process, from data curation through to quantitative analysis and visualization.

Key Variables:

From the Global Power Plant Database: gppd_idnr, name, country, capacity_mw, latitude, longitude, primary_fuel, commissioning_year.
From the Aqueduct 4.0 Datasets: pfaf_id (basin ID), bws_score (baseline water stress score), bwd_score (baseline water depletion score), and future scenario scores such as ws_score (water stress score) for different scenarios and years. We will primarily use the standardized _score (0-5 scale) and _label (e.g., "High Risk") columns for comparison and analysis.
Analysis Plan:

Data Curation & Preprocessing: This initial phase will involve loading all datasets, addressing data quality issues identified during initial review (e.g., handling missing values, special numeric codes like -9999), and ensuring data types are correct.
Geospatial Linking: A critical step will be to perform a geospatial join. Each power plant's latitude and longitude from the GPPD will be used to identify the specific hydrological basin (pfaf_id) it resides in. This will allow us to assign the corresponding Aqueduct water risk indicators to each power plant.
Exploratory Data Analysis (EDA): Once the datasets are cleaned and merged, we will conduct an EDA to uncover initial patterns. This will include mapping the locations of power plants color-coded by their baseline water risk scores and analyzing the distribution of capacity across different risk categories.
Scenario Analysis: We will analyze the future projection data to assess how water risks for existing power plants are expected to change by 2030, 2050, and 2080 under optimistic, business-as-usual, and pessimistic scenarios.
Final Output: The insights will be compiled into a final report and presented in an interactive dashboard or datafolio, allowing users to explore the water risk exposure of power plants by region, fuel type, and future scenario.
5. Milestones
To ensure the project progresses in a structured manner, the work will be broken down into the following key milestones, which align with the major deliverables for the capstone project:

Project Plan Finalized: The Project Description and Project Scoping documents are completed, defining the project's goals, scope, datasets, and methods.
Analytical Dataset Created: All necessary data is acquired, cleaned, processed, and merged. The crucial geospatial join between the power plant locations and the water risk basins is completed.
Exploratory Data Analysis (EDA) Completed: Initial analysis is performed on the clean dataset to uncover key insights, generate summary statistics, and create preliminary visualizations and maps.
Interactive Dashboard Developed: An interactive dashboard or datafolio is created to effectively communicate the project's key findings.
Final Submission Completed: The final report is written, documenting the entire process from problem scoping to conclusion, and a final presentation of the project is prepared.
6. Timeline
The following timeline is based on the official due dates for the capstone project deliverables. The work will be paced to meet these deadlines.

Project Description & Project Scoping:
Due Date: Friday, June 6, 2025
Status: Drafts completed.
Data Curation:
Due Date: Friday, June 13, 2025
Focus for the week (June 7 - June 13):
Acquire necessary geospatial data (HydroBASIN Level 6 shapefiles).
Write and execute data cleaning scripts.
Perform the geospatial join.
Create and validate the final, merged analytical dataset.
Exploratory Data Analysis (EDA):
Due Date: Friday, June 20, 2025
Focus for the week (June 14 - June 20):
Conduct deep analysis of the merged dataset.
Generate key visualizations (maps, charts).
Document initial findings.
Datafolio & Dashboard:
Due Date: Friday, June 27, 2025
Focus for the week (June 21 - June 27):
Design and build all interactive components of the dashboard.
Final Report:
Due Date: Friday, July 4, 2025
Focus for the week (June 28 - July 4):
Write all sections of the final report.
Prepare the final presentation.
This Project Scope is meant to be a baseline and not a contract; the project direction may change as the analysis progresses.
