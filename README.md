# Time-Series Forecasting with ARIMA

## Project Overview

This project implements an end-to-end time-series forecasting pipeline for historical daily demand data.

The project analyzes trends, seasonality, stationarity, and historical demand patterns before building an ARIMA forecasting model.

## Objectives

- Analyze historical demand trends
- Decompose the time series into trend, seasonal, and residual components
- Test stationarity using the Augmented Dickey-Fuller (ADF) test
- Apply differencing when required
- Select suitable ARIMA hyperparameters
- Evaluate forecasting performance using RMSE and MAPE
- Generate a 30-day future demand forecast

## Dataset

The dataset contains historical daily demand observations along with additional event-related information.

## Methodology

### 1. Exploratory Data Analysis

The historical demand series was visualized to understand overall demand behavior and trends.

### 2. Time-Series Decomposition

The series was decomposed into:

- Observed
- Trend
- Seasonal
- Residual

A weekly seasonal period of 7 days was considered for daily demand data.

### 3. Stationarity Testing

The Augmented Dickey-Fuller (ADF) test was used to determine whether the demand series was stationary.

Differencing was applied when necessary.

### 4. ARIMA Model

Multiple ARIMA configurations were evaluated by varying:

- p
- d
- q

The best configuration was selected based on test-set forecasting performance.

### 5. Model Evaluation

The model was evaluated using:

- RMSE (Root Mean Squared Error)
- MAPE (Mean Absolute Percentage Error)

### 6. Forecasting

The final model was trained using the complete historical dataset and used to generate a 30-day future demand forecast.

## Output

The project produces:

- Time-series visualization
- Trend/seasonality/residual decomposition
- ADF stationarity analysis
- ARIMA model comparison
- RMSE and MAPE evaluation
- Actual vs predicted visualization
- 30-day future forecast
- Forecast confidence interval

## Files

- `time_series_forecasting.ipynb` — Complete analysis and forecasting notebook
- `daily-demand-series.csv` — Input dataset
- `30_day_demand_forecast.csv` — Generated 30-day forecast