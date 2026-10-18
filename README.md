# Predicting Optimal NDVI Levels for Safe NO2 Concentrations

## Overview
This project explores the relationship between the Normalized Difference Vegetation Index (NDVI) and nitrogen dioxide (NO2) concentrations using Google Earth Engine data for Delhi from 2019 to 2023.

A polynomial regression model is used to estimate the NDVI change associated with a defined NO2 target. The trained model is then applied to hypothetical scenarios for Kolkata to explore potential vegetation-related changes.

## Technologies
- Python
- Pandas and NumPy
- Matplotlib
- Polynomial Regression
- Google Earth Engine data

## Workflow
1. Load and preprocess NDVI and NO2 data.
2. Calculate changes across observations and derive a target variable.
3. Engineer polynomial features and train a regression model.
4. Evaluate predictions using R² scores and an actual-versus-predicted plot.
5. Explore hypothetical Kolkata scenarios using the trained model.

## Results
- Training R²: 0.9834
- Test R²: 0.9808

These scores reflect performance against the target variable constructed in this notebook. They do not establish causal effects or validate the estimated vegetation requirements.

## How to Run
1. Open the notebook in Google Colab.
2. Provide the required CSV dataset and update the file path.
3. Run the notebook cells in order.

## Limitations
The target variable and scenario calculations are exploratory and require further validation. The estimated tree counts are rough proxies derived from NDVI change, not scientifically validated planting requirements.
