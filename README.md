# Fork of WRI Global Power Plant Database

This repository contains a fork of the [World Resources Institute (WRI) Global Power Plant Database](https://github.com/wri/global-power-plant-database). The original database is a comprehensive, open source dataset of power plants around the world.

This fork was created as part of a capstone project to [briefly describe the capstone project's objective, e.g., "analyze power plant data for X purpose" or "demonstrate data processing techniques using the WRI dataset"]. The original README specific to the capstone project can be found in [README-capstone.md](README-capstone.md).

Below is the modified README from the original WRI Global Power Plant Database, with project-specific details removed and links updated to point to the WRI repository.

---

# Global Power Plant Database
The Global Power Plant Database is a comprehensive, open source database of power plants around the world. It centralizes power plant data to make it easier to navigate, compare and draw insights for policy-makers, analysts and the public. The database covers approximately 35,000 power plants in 167 countries and includes thermal plants (e.g. coal, gas, oil, nuclear, biomass, waste, geothermal) and renewables (e.g. hydro, wind, solar). Each power plant is geolocated and entries contain information on plant capacity, generation, ownership, and fuel type. It will be continuously updated as data becomes available.

**Suggested citation:** World Resources Institute. 2023. Global Power Plant Database. Published on Resource Watch and Google Earth Engine; WRI, Washington, DC. Available online at: [https://github.com/wri/global-power-plant-database](https://github.com/wri/global-power-plant-database)

**License:** Creative Commons Attribution 4.0 International ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).

**Version:** 1.3.0 (July 2021) - previous versions are available in the [releases section](https://github.com/wri/global-power-plant-database/releases)

## Data
The database is available as a CSV file:
* [global_power_plant_database.csv](https://github.com/wri/global-power-plant-database/raw/master/source_databases_csv/global_power_plant_database.csv)

A data dictionary (.xlsx) explaining the columns and sources is available here:
* [data_dictionary.xlsx](https://github.com/wri/global-power-plant-database/blob/master/source_databases_csv/data_dictionary.xlsx?raw=true)

## Database Attributes
The database includes the following information for each power plant:

| Field Name                     | Description                                                                                                | Data Type |
|--------------------------------|------------------------------------------------------------------------------------------------------------|-----------|
| `country`                      | 3-letter ISO country code                                                                                    | TEXT      |
| `country_long`                 | Full name of country                                                                                       | TEXT      |
| `name`                         | Name of power plant                                                                                        | TEXT      |
| `gppd_idnr`                    | Unique identifier for the power plant from the Global Power Plant Database                                   | TEXT      |
| `capacity_mw`                  | Electrical generating capacity in megawatts                                                                  | NUMBER    |
| `latitude`                     | Latitude of power plant                                                                                      | NUMBER    |
| `longitude`                    | Longitude of power plant                                                                                     | NUMBER    |
| `primary_fuel`                 | Primary sub-type of fuel, if applicable                                                                    | TEXT      |
| `other_fuel1`                  | Secondary sub-type of fuel, if applicable                                                                  | TEXT      |
| `other_fuel2`                  | Tertiary sub-type of fuel, if applicable                                                                   | TEXT      |
| `other_fuel3`                  | Quaternary sub-type of fuel, if applicable                                                                 | TEXT      |
| `commissioning_year`           | Year of plant commissioning; recorded as year only                                                         | NUMBER    |
| `owner`                        | Majority owner of the power plant                                                                          | TEXT      |
| `source`                       | Entity reporting the data; could be a government agency, research institute, or company                      | TEXT      |
| `url`                          | Web address for the source                                                                                 | TEXT      |
| `geolocation_source`           | Source of the plant's geolocation data                                                                     | TEXT      |
| `wepp_id`                      | Identifier for the power plant from the World Electric Power Plants Data Base (see note below)               | TEXT      |
| `year_of_capacity_data`        | Year the capacity information was reported                                                                 | NUMBER    |
| `generation_gwh_xxxx`          | Electricity generation in gigawatt-hours for xxxx year (available for various years)                         | NUMBER    |
| `generation_data_source`       | Source of the generation data                                                                              | TEXT      |
| `estimated_generation_gwh_xxxx`| Estimated electricity generation in gigawatt-hours for xxxx year (see methodology for details)             | NUMBER    |
| `estimated_generation_note_xxxx`| Notes on the estimation methodology for xxxx year                                                          | TEXT      |

**Note on `wepp_id`**: The `wepp_id` field corresponds to the WEPP dataset from S&P Global (formerly Platts). This dataset is proprietary and not included directly in the Global Power Plant Database. However, users with access to the WEPP dataset can use this identifier to cross-reference information.

## How the Database is Built
The Global Power Plant Database is built using a variety of publicly available data sources, including:
* National government energy statistics
* Utility company reports
* News articles and press releases
* Other publicly available datasets

Data is manually collected, cleaned, and harmonized. Where possible, information is cross-referenced with multiple sources to ensure accuracy. The database is continuously updated as new information becomes available. The full methodology is detailed in the documentation available in the original WRI repository.

## Contributing
We welcome contributions to improve and expand this database. If you have new data or find errors in existing entries, please refer to the contribution guidelines in the [original WRI repository](https://github.com/wri/global-power-plant-database).

## Contact
For questions or feedback, please open an issue in the [original WRI repository's issue tracker](https://github.com/wri/global-power-plant-database/issues).
