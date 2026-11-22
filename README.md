# Washington State Climate Data Analysis (2012–2024)

An INFO 201 team project examining reported greenhouse gas emissions and monthly average temperatures in Washington State, using public government datasets.

## Overview

We explored how reported greenhouse gas emissions changed between 2012 and 2024, how they differed by reporting sector, and how these patterns compared with Washington's monthly temperature data. The analysis is **descriptive** and does not establish a causal relationship between emissions and temperature.

## Tools and methods

- **R**, **tidyverse** (`dplyr`, `readr`, `ggplot2`)
- Data cleaning and transformation, aggregation by year, joining datasets by year
- Line plots, annual emissions comparisons, temperature boxplots, sector-level comparisons

## Key observations

- Reported emissions increased sharply in the dataset after 2021.
- The supplier reporting sector contributed a large share of reported emissions in recent years.
- Monthly temperatures fluctuated across years rather than increasing monotonically.

**Interpretation caveat:** The number of reporting records also rose after 2021, so trends in reported emissions should not automatically be interpreted as changes in emissions from a fixed set of facilities. Correlation or visual co-movement does not demonstrate causality.

## Repository contents

- [`analysis.Rmd`](analysis.Rmd): Original team analysis and narrative, with data file paths updated for this repository
- [`report.pdf`](report.pdf): Original course report
- [`data/GHG_Reporting_Program_Publication_20260510.csv`](data/GHG_Reporting_Program_Publication_20260510.csv): Washington GHG reporting dataset snapshot
- [`data/data.csv`](data/data.csv): Washington monthly temperature download (2012–2024)

## Running the analysis

1. Install R and RStudio, and install the `tidyverse` package if needed: `install.packages("tidyverse")`.
2. Open the project folder in RStudio so the working directory is the repository root.
3. Open `analysis.Rmd` and choose **Knit** to render the report.

The source file retains the team's original analysis approach; this repository is a course project archive, not a maintained production pipeline. Rendering has not been independently tested in this package.

## Data sources

- [Washington State Department of Ecology — GHG Reporting Program Publication](https://data.wa.gov/Natural-Resources-Environment/GHG-Reporting-Program-Publication/idhm-59de)
- [NOAA National Centers for Environmental Information — Climate at a Glance, Washington State](https://www.ncei.noaa.gov/access/monitoring/climate-at-a-glance/statewide/time-series/45/tavg/1/0/2012-2024)

Data were obtained from these public sources. Check their current terms and attribution requirements before redistributing the snapshots.

## Team and contributions

**Team:** Xiaoyu, Kai, Mike (INFO 201, Spring 2026).

The original report identifies Xiaoyu as the author of the Abstract, Results, and Discussion sections; Kai of the Introduction and Datasets; and Mike of Data, Method, and Summary. The code is presented as a **team project**; individual code ownership is not separately established in the report.

## Limitations

This analysis covers one state and the 2012–2024 period. Joining by year and visualizing trends cannot support causal claims about local emissions and temperature change. The report reflects a classroom analysis rather than peer-reviewed climate research.
