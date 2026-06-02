# Dubai Mortgage and Rental Prediction

A Python notebook for exploring Dubai real estate data and forecasting rental market supply and mortgage-rate trends using time-series models.

## Overview

This project analyzes Dubai real estate market data from 2020–2026, combining monthly community-level pricing data with property-level rental and sales records. It focuses on understanding how rental prices, rental listings, and mortgage rates evolve over time, and uses forecasting models to predict near-term market behavior.

## Dataset

The notebook uses the **Dubai Real Estate Sales and Rentals (2020–2026)** dataset, which includes:

- Monthly community-level market data.
- Rental property records.
- Secondary sales records.
- Metro station and location-related features.

### Main fields used

#### Monthly price data
- `yearmonth`
- `community`
- `zone`
- `isfreehold`
- `rentalpricepersqftannualusd`
- `nlistingsrental`
- `avgmortgageratepct`

#### Rental listings
- `id`
- `datelisted`
- `community`
- `zone`
- `propertycategory`
- `propertytype`
- `bedrooms`
- `areasqft`
- `contracttype`
- `annualrentusd`
- `rentpersqftusd`

#### Sales listings
- `id`
- `datelisted`
- `community`
- `zone`
- `propertycategory`
- `propertytype`
- `bedrooms`
- `priceusd`
- `pricepersqftusd`
- `mortgagerateatlisting`

## What the notebook does

- Loads and inspects the Dubai real estate datasets.
- Cleans and reshapes the data for analysis.
- Visualizes trends in rental prices, rental listing volume, and mortgage rates.
- Builds a **SARIMAX** model to forecast rental supply for a selected community.
- Builds an **ARIMA** model to forecast mortgage rates.

## Key insights explored

The notebook is designed to answer questions such as:

- How have Dubai rental prices changed over time?
- Which communities show stronger rental supply growth?
- How do mortgage rates move over time?
- Can past market behavior help forecast short-term rental supply?

## Models used

- **SARIMAX** for rental listing forecasting.
- **ARIMA** for mortgage-rate forecasting.

## Requirements

This notebook was built in Python 3 and uses common data science libraries such as:

- pandas
- numpy
- matplotlib
- seaborn
- statsmodels

## How to run

1. Open the notebook in Jupyter Notebook or JupyterLab.
2. Make sure the required libraries are installed.
3. Download or mount the Kaggle dataset used in the notebook.
4. Run the cells in order to reproduce the analysis and forecasts.

## Notes

- The notebook includes exploratory analysis and modeling, so results may vary depending on the selected community or date range.
- One of the dataframe cleanup steps appears to have a column-selection error during development, but the core analysis and forecasting workflow is still clear.

## Project status

This project is best described as an exploratory forecasting notebook for Dubai residential real estate trends, with a focus on rentals and mortgage indicators.
