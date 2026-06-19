# Investment Risk Analysis in Sub-Saharan Africa

## Overview

This project evaluates investment risk across Sub-Saharan Africa using World Bank data and panel-data econometric techniques in R.

The analysis investigates whether macroeconomic instability, particularly exchange-rate volatility and inflation volatility, influences foreign direct investment (FDI) inflows. The objective is to identify economic conditions associated with stronger or weaker investment performance and demonstrate how quantitative analysis can support investment decision-making.

## Business Problem

Foreign direct investment plays a critical role in economic growth, job creation, and capital formation across developing economies. However, investors face uncertainty when evaluating markets with unstable macroeconomic conditions.

This project examines whether macroeconomic instability reduces investment attractiveness across Sub-Saharan Africa and identifies the factors most strongly associated with FDI inflows.

## Data

Source: World Bank World Development Indicators (WDI)

Period: 1980–2022

Region: Sub-Saharan Africa

Key variables include:

* Foreign Direct Investment (FDI)
* Population
* Exchange Rates
* Inflation
* GDP per Capita
* Trade Openness

## Methodology

The analysis was conducted in R and includes:

* Data cleaning and transformation
* Reshaping panel datasets
* Construction of FDI per capita measures
* Log transformations
* Exchange-rate volatility measures
* Inflation volatility measures
* Fixed-effects panel regression models
* Robustness checks using alternative volatility measures
* Data visualisation

## Main Model

The preferred specification estimates the relationship between:

## Dependent Variable

* Log FDI per capita

## Explanatory Variables

* Exchange-rate volatility
* Inflation volatility
* Trade openness
* GDP per capita

Country and year fixed effects are included to control for unobserved heterogeneity.

## Key Findings

* Higher exchange-rate volatility is associated with lower FDI inflows.
* Inflation instability generally reduces investment attractiveness.
* GDP per capita is positively associated with investment inflows.
* Results remain broadly consistent across alternative volatility measures.

## Project Files

* investment_risk_analysis_clean.R – analysis workflow and model estimation
* ssa_fdi_dataset.csv – processed dataset
* baseline_model_results.html – preferred regression results
* robustness_volatility_results.html – robustness checks
* graph_exrate_final.png – exchange-rate volatility analysis
* graph_inflation_final.png – inflation volatility analysis

## Tools Used

* R
* tidyverse
* fixest
* modelsummary
* ggplot2
* ggrepel
* World Bank WDI API

## Reproducing the Analysis

1. Download the dataset and R script.
2. Open the project in RStudio.
3. Install the required packages:
    * tidyverse
    * WDI
    * slider
    * fixest
    * modelsummary
    * ggplot2
    * ggrepel
4. Run the script from top to bottom.
5. Regression outputs and visualisations will be generated automatically.

## Future Improvements

Potential extensions include:

* Interactive investment-risk dashboard
* Python implementation
* Country-level investment risk scoring
* Additional macroeconomic indicators
* Real-time data integration

