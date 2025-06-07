Capstone Project Scoping Document
This document clarifies the project's problem statement and outlines the proposed solution, considering its feasibility, impact, and usability within the project timeframe.

1. Business Problem
The global energy sector, a cornerstone of modern economic and social stability, has a critical and often underestimated vulnerability: its dependence on reliable water resources. This "water-energy nexus" presents a growing challenge as climate change and increasing demand intensify water stress globally. While this systemic risk is acknowledged, there is a significant gap in the granular, plant-level assessment of water risk exposure for existing energy infrastructure.
This project addresses the specific problem of quantifying the current and projected future water risks—including water stress, depletion, and variability—for a comprehensive portfolio of global power plants.

2. Business Impact
The primary benefit of this analysis will be the creation of a detailed, data-driven water risk assessment for global power infrastructure, enabling stakeholders to make more informed decisions333. The specific impacts include:

Enhanced Energy Security: By identifying which power plants are in current or future water-risk hotspots, energy operators and grid planners can better anticipate potential disruptions, reduced operational efficiencies, or plant shutdowns, leading to more resilient energy systems.
Informed Investment and Policy: The analysis will provide valuable intelligence for investors assessing the long-term viability of energy assets and for policymakers developing water management and climate adaptation strategies for the energy sector.
Support for Sustainable Development: The project directly supports Sustainable Development Goals (SDGs) related to water (SDG 6), energy (SDG 7), and climate action (SDG 13).
Strategic De-risking: For energy companies, this analysis can inform strategic decisions about their portfolio of assets, including where to prioritize water-efficiency upgrades or where to site new, less water-intensive power generation facilities.
3. Data
The analysis will be based on publicly available datasets from the World Resources Institute (WRI). The core datasets we are working with are:

WRI Global Power Plant Database (GPPD): Provides detailed information for approximately 35,000 power plants worldwide, including their specific location (latitude, longitude), capacity, primary fuel type, and operational status.
WRI Aqueduct 4.0 Water Risk Atlas: We are utilizing several basin-level (pfaf_id) outputs from this suite, including baseline monthly data, future annual projections under various scenarios, and the comprehensive baseline annual dataset.
Supporting Geospatial Data: HydroBASIN Level 6 shapefiles are used to perform the geospatial join between the power plant point data and the Aqueduct basin-level risk data.
These datasets represent the initial plan for this analysis, and additional contextual datasets may be considered if necessary.
4. Methods
The methodology for this project will follow a structured data analysis process, from data curation through to quantitative analysis and visualization.

Key Variables6:


From the Global Power Plant Database: gppd_idnr, name, country, capacity_mw, latitude, longitude, primary_fuel, commissioning_year.
From the Aqueduct 4.0 Datasets: pfaf_id (basin ID), bws_score (baseline water stress score), bwd_score (baseline water depletion score), and future scenario scores such as ws_score (water stress score). We will primarily use the standardized _score (0-5 scale) and _label (e.g., "High Risk") columns.
Analysis Plan:


Data Curation & Preprocessing: Load all datasets, address data quality issues (missing values, special numeric codes), and ensure data types are correct.
Geospatial Linking: Perform a geospatial join to assign Aqueduct water risk indicators to each power plant based on its location.
Exploratory Data Analysis (EDA): Analyze the merged dataset to uncover patterns, including mapping risk hotspots and analyzing risk profiles by fuel type.
Scenario Analysis: Analyze the future projection data to assess how water risks for existing power plants are expected to change by 2030, 2050, and 2080 under different scenarios.
Final Output: Compile insights into a final report and present them in an interactive dashboard or datafolio.
5. Milestones
The project work is broken down into the following key milestones, aligning with the major capstone deliverables:

Project Plan Finalized: The Project Description and Project Scoping documents are completed.
Analytical Dataset Created: All data is acquired, cleaned, processed, and merged.
Exploratory Data Analysis (EDA) Completed: Initial analysis is performed to generate key insights and visualizations.
Interactive Dashboard Developed: An interactive dashboard or datafolio is created to communicate key findings.
Final Submission Completed: The final report and project presentation are prepared and completed.
6. Timeline
The following timeline is based on the official due dates for the capstone project deliverables to ensure timely completion.

Project Description & Project Scoping: Due Date: Thursday, June 12, 2025
Data Curation: Due Date: Friday, June 13, 2025
Exploratory Data Analysis (EDA): Due Date: Friday, June 20, 2025
Datafolio & Dashboard: Due Date: Friday, June 27, 2025
Final Report: Due Date: Friday, July 4, 2025

This Project Scope is meant to be a baseline and not a contract; the project direction may change as the analysis progresses.

