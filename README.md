# India Climate Analysis and Prediction Models

This notebook performs a comprehensive climate analysis for India using CHELSA climate data, focusing on spatial patterns, temporal trends, and predictive modeling.

## Overview

The analysis covers the following key areas:

1.  **Spatial Climate Analysis**: Visualizing temperature and precipitation patterns across India.
2.  **Climate Zone Classification**: Defining and mapping custom climate zones based on temperature and precipitation thresholds.
3.  **Temporal Trend Analysis**: Examining historical trends in temperature and precipitation from 2000 to 2023.
4.  **Time Series Prediction Modeling**: Building and comparing ARIMA, Random Forest, and a simplified Neural Network model to forecast future climate conditions.
5.  **Climate Change Impact Assessment**: Analyzing long-term trends and projecting future climate scenarios (2024-2030).

## Data

The analysis utilizes CHELSA (Climatologies at High Resolution for the Earth's Land Surface Areas) climate data, specifically BioClim variables 1 (Annual Mean Temperature) and 12 (Annual Precipitation). Elevation data from AWS Terrain Tiles is also used for 3D visualization.

## Methodology

The notebook follows a structured approach:

1.  **Setup**: Installing and loading necessary R packages.
2.  **CHELSA Data**: Downloading and processing CHELSA temperature and precipitation data.
3.  **Spatial Analysis**: Cropping and masking climate data to the extent of Asia and then India, followed by resampling to match the resolution of elevation data.
4.  **Bivariate Mapping**: Creating bivariate maps to visualize the relationship between temperature and precipitation across Asia and India.
5.  **Climate Zone Mapping**: Classifying and mapping custom climate zones for India based on defined temperature and precipitation ranges.
6.  **Time Series Preparation**: Generating synthetic time series data for India (for demonstration purposes) and preparing it for time series modeling.
7.  **Prediction Modeling**:
    *   **ARIMA**: Fitting and forecasting with ARIMA models for temperature and precipitation.
    *   **Random Forest**: Building and evaluating Random Forest models with lagged features and seasonal indicators.
    *   **Simplified Neural Network**: Implementing a basic feed-forward neural network as an alternative for sequence prediction.
8.  **Climate Change Assessment**: Analyzing decadal trends, calculating climate change indicators, and projecting future climate scenarios based on historical trends.
9.  **Model Comparison and Future Projections**: Comparing the performance of the implemented models and visualizing future climate projections under different scenarios.
10. **Summary and Insights**: Presenting key findings from the spatial analysis, temporal trends, model performance, and future projections.

## Key Findings

The analysis revealed several key findings:

*   **Spatial Patterns**: Identification of dominant climate zones across India based on temperature and precipitation.
*   **Temporal Trends**: Observed trends in annual mean temperature and precipitation in India from 2000 to 2023.
*   **Model Performance**: Comparison of ARIMA, Random Forest, and Neural Network models for climate prediction, indicating the relative performance of each approach for this specific dataset.
*   **Future Projections**: Projections for temperature and precipitation from 2024 to 2030 under different climate change scenarios, highlighting potential future climate conditions and variability.

## Output Files

The notebook generates the following output files:

*   `asia_bivariate_2d.png`: 2D bivariate map of temperature and precipitation for Asia.
     ![alt text](https://github.com/Stalinosmj/R_project-/blob/0e4dd5d25e023252c59ead5453ee0ad25773d854/asia__bivariate_2d.png "Asia bivariate")   
*   `india_climate_bivariate.png`: 2D bivariate map of temperature and precipitation for India.
     ![alt text](https://github.com/Stalinosmj/R_project-/blob/0e4dd5d25e023252c59ead5453ee0ad25773d854/india_climate_bivariate.png "India Climate bivariate")    
*   `india_climate_zones.png`: Map of custom climate zones for India.
     ![alt text](https://github.com/Stalinosmj/R_project-/blob/0e4dd5d25e023252c59ead5453ee0ad25773d854/india_climate_zones.png "India climate zones")   
*   `india_climate_trends.png`: Plots showing annual temperature, precipitation, extreme heat events, and drought events trends for India.
     ![alt text](https://github.com/Stalinosmj/R_project-/blob/0e4dd5d25e023252c59ead5453ee0ad25773d854/india_climate_trends.png "Indai climate trends")   
*   `india_climate_projections.png`: Plots showing future temperature and precipitation projections for India under different climate change scenarios.
     ![alt text](https://github.com/Stalinosmj/R_project-/blob/0e4dd5d25e023252c59ead5453ee0ad25773d854/india_climate_projections.png "india climate projection")   
*   `india_climate_timeseries.csv`: CSV file containing the synthetic time series data for India.
*   `india_climate_projections_2024_2030.csv`: CSV file containing the detailed future climate projections.
*   `india_climate_analysis_results.RData`: RData file containing summary statistics and key findings from the analysis.

## Usage

To run this analysis, execute the code cells sequentially in a Google Colab environment. Ensure you have the necessary R packages installed (the notebook includes installation steps). The CHELSA data will be downloaded automatically.

## Dependencies

The analysis relies on the following R packages:

*   `knitr`
*   `remotes`
*   `rchelsa`
*   `pacman`
*   `geodata`
*   `tidyverse`
*   `sf`
*   `terra`
*   `biscale`
*   `elevatr`
*   `cowplot`
*   `gridGraphics`
*   `rayshader`
*   `rnaturalearth`
*   `forecast`
*   `tseries`
*   `caret`
*   `randomForest`
*   `neuralnet`
*   `keras`
*   `tensorflow`
*   `lubridate`
*   `dplyr`
*   `ggplot2`
*   `plotly`
*   `corrplot`
