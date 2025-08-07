# shinymrp-data

[![CC0 1.0 Universal](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

A data repository for the R package shinymrp.

## Catalog

### Example Data

The files in the `example/data/` folder contain input examples for sample and poststratification data.

| Name                  | Description           |
|-----------------------|-----------------------|
| covid_binomial_raw.csv            | Raw sample data for COVID data module                                                     |
| covid_binomial_prep.csv           | Preprocessed sample data for COVID data module                                            |
| poll_binomial_raw.csv             | Raw sample data for polling data module                                                   |
| poll_binomial_prep.csv            | Preprocessed sample data for polling data module                                          |
| timevarying_binomial_raw.csv      | Raw sample data with binary outcome for general time-varying data module                  |
| timevarying_binomial_ prep.csv    | Preprocessed sample data with binary outcome for general time-varying data module         |
| timevarying_normal_raw.csv        | Raw sample data with continuous outcome for general time-varying data module              |
| timevarying_normal_prep.csv       | Preprocessed sample data with continuous outcome for general time-varying data module     |
| crosssectional_binomial_raw.csv   | Raw sample data with binary outcome for general cross-sectional data module               |
| crosssectional_binomial_prep.csv  | Preprocessed sample data with binary outcome for general cross-sectional data module      |
| crosssectional_normal_raw.csv     | Raw sample data with continuous outcome for general cross-sectional data module           |
| crosssectional_normal_prep.csv    | Preprocessed sample data with continuous outcome for general cross-sectional data module  |
| pstrat.csv                        | Poststratification data for general data module                                           |

### Example Estimation Results

The files in the `example/fit/` folder contain example estimation results for the Shiny app.

| Name                  | Description           |
|-----------------------|-----------------------|
| covid_binomial_fit.csv            | Estimation results for COVID data module                                          |
| poll_binomial_fit.csv             | Estimation results for polling data module                                        |
| timevarying_binomial_fit.csv      | Estimation results for general time-varying data module (binary outcome)          |
| timevarying_normal_fit.csv        | Estimation results for general time-varying data module (continuous outcome)      |
| crosssectional_binomial_fit.csv   | Estimation results for general cross-sectional data module (binary outcome)       |
| crosssectional_normal_fit.csv     | Estimation results for general cross-sectional data module (continuous outcome)   |

### Geography Data

The files in the `geo/` folder contain data used by the package for generating maps and converting between geographies.

| Name                  | Description           |
|-----------------------|-----------------------|
| geojson_county.qs     | GEOJSON for generating maps of US counties    |
| geojson_state.qs      | GEOJSON for generating maps of US states      |
| fips_county.csv       | County names to FIPS codes                    |
| fips_state.csv        | State names to FIPS codes                     |
| zip_county_state.csv  | ZIP codes to counties and states              |
| zip_tract.csv         | ZIP codes to Census tracts                    |

### Poststratification Data

The files in `acs/` folder contain data used by the package functions for constructing poststratification tables for the second stage of MRP.

| Name                  | Description           |
|-----------------------|-----------------------|
| acs_2015-2019.csv<br>acs_2016-2020.csv<br>acs_2017-2021.csv<br>acs_2018-2022.csv<br>acs_2019-2023.csv | Tract-level population counts by demographics (general modules) |
| pstrat_covid.csv  | ZIP-code-level population counts by demographics computed from tract-level counts in 2017-2021 ACS data (COVID module) |
| covar_covid.csv   | ZIP-code-level covariates computed from tract-level quantities in the 2017-2021 ACS data (COVID data module) |
| pstrat_poll.csv   | State-level population counts by demographics (plus education level) computed from the 2014-2018 ACS data (Polling data module) |


## License

All data in this repository are released into the public domain under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).  
“No Rights Reserved” — you can copy, modify, and redistribute for any purpose.
