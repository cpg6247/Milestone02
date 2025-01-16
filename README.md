# README.md: Drug Overdose Death Rates Analysis
# Caroline Gore

## Binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cpg6247/Milestone02/main?labpath=milestone02_cpg6247.ipynb)
## Project Overview

This project aims to analyze drug overdose death rates across different U.S. states from 2015 to 2023. The analysis seeks to uncover patterns and trends in overdose deaths, both on a state-wise and year-wise basis, using a combination of data visualizations and statistical insights.

## Research Question

How have drug overdose death rates evolved across different U.S. states over the period from 2015 to 2023, and what patterns or trends can be observed with respect to state-wise and year-wise variations in overdose deaths?

## Data Sources

The analysis is based on two primary data sources:

1. **Primary Dataset**: `VSRR_Provisional_Drug_Overdose_Death_Counts.csv` 
   - This dataset contains provisional overdose death counts from 2015 to 2023 across different U.S. states. It includes columns for State, Year, and Data Value, representing the total number of drug overdose deaths reported.
2. **Geospatial Data**: GeoJSON file from Plotly for U.S. states
   - URL: [GeoJSON File](https://raw.githubusercontent.com/plotly/datasets/master/geojson-counties-fips.json)
   - This file is used for visualizing geographic distribution in the choropleth map.

## Data Cleaning and Processing

- **Data Cleaning**: The dataset was cleaned by selecting relevant columns (`State`, `Year`, `Data Value`) and converting `Data Value` to numeric, while removing any rows with missing values.
- **Data Transformation**: State names were mapped to their respective two-letter abbreviations to ensure consistency for visualizations.

## Visualizations Created

A series of visualizations were created to illustrate the trends in drug overdose deaths:

1. **Bar Plot**: Displays the total overdose deaths per year from 2015 to 2023. This visualization helps identify year-over-year trends in the overall number of overdose deaths.
2. **Line Plot**: Depicts the trend of total overdose deaths over time, providing an overview of the progression of overdose deaths from 2015 to 2023.
3. **Box Plot**: Shows the distribution of overdose deaths by state, illustrating state-wise variability and identifying states with consistently high or low numbers of deaths.
4. **Choropleth Map**: Displays overdose deaths across U.S. states by year, representing the geographic distribution and highlighting areas with the highest concentrations of overdose deaths.
5. **Top States Plot for 2022**: Highlights the top 10 states with the highest overdose deaths in 2022, providing a snapshot of the most affected states during that year.

All visualizations are saved in the `UNC/CHIP490/Milestone02/Visuals` directory for easy access.

## Running the Analysis

The analysis is conducted using a Jupyter notebook, which includes the following steps:

1. **Install Dependencies**: Ensure the required Python packages are installed:
   - `pandas`, `seaborn`, `matplotlib`, `plotly`, `numpy`, and `kaleido` for saving Plotly visualizations.
   
   You can install them using:
   ```sh
   pip install pandas seaborn matplotlib plotly numpy kaleido
   ```

2. **Load Data**: The dataset (`VSRR_Provisional_Drug_Overdose_Death_Counts.csv`) is loaded and cleaned to ensure consistency.

3. **Create Visualizations**: The notebook generates various plots, including bar plots, line plots, box plots, and a choropleth map. Each plot is saved to the `Visuals` directory.

4. **Save Visualizations**: The visualizations are saved as PNG files to the `UNC/CHIP490/Milestone02/Visuals` directory.

To run the analysis, simply open the Jupyter notebook and execute the cells in sequence. The visualizations will be generated and saved automatically.

## Summary of Key Insights

- **Yearly Trends**: The bar plot and line plot show that overdose deaths have generally increased from 2015 to 2023, highlighting the worsening opioid crisis in the U.S.
- **State-wise Distribution**: The box plot reveals significant variability in overdose deaths among states, with certain states consistently experiencing higher death counts.
- **Geographic Insights**: The choropleth map provides a clear visual representation of which states are most affected by overdose deaths, with noticeable clusters in certain regions.
- **Top States in 2022**: The bar plot for 2022 shows that a few states, such as [specific states], had significantly higher overdose deaths, pointing to regional hotspots for further investigation.

---
This README file documents the entire analysis process, providing an overview of the objectives, data sources, analysis steps, and key insights derived from the visualizations.
