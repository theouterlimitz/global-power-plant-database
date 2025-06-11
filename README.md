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

## Installation

To set up the project, clone the repository and install the required dependencies:

```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
pip install -r requirements.txt
```

## Project Structure

- `build_databases/`: Scripts to build the power plant databases from raw source files.
- `output_database/`: The final global power plant database CSV and summary files.
- `raw_source_files/`: Raw data files from various sources.
- `resources/`: Supporting CSV files, thesauri, and concordance lists.
- `utils/`: Utility scripts for various tasks like coordinate assembly, country checking, etc.
- `*.ipynb`: Jupyter notebooks for data curation and exploratory data analysis.

## Usage

Detailed usage instructions and examples will be provided for specific scripts and notebooks.

## Contributing

Contributions are welcome! Please see our [Contributing Guidelines](.github/CONTRIBUTING.md) for more details on how to submit pull requests, report issues, and suggest improvements.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details (if one exists, otherwise we can create a standard MIT License text).

## Acknowledgments

This project utilizes the Global Power Plant Database, a product of the World Resources Institute (WRI). We are grateful for their efforts in compiling and sharing this valuable dataset.

## Contact and Citation

For questions about this project, please contact [Your Name/Email or Project Email].

If you use this work in your research, please cite it as follows:
[Placeholder for citation format]
