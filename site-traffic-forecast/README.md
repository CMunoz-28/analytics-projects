# Site Traffic Forecast

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pMf2GuvU6lKha3wHSQiVlIXL9kyaT1L1)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)

## Overview

Time series forecasting of website traffic using Facebook Prophet. Analyzes historical click patterns and generates a 365-day forward forecast with confidence intervals, including seasonal trend decomposition.

## Dataset

- **Source:** Internal web analytics export
- **Files:** `Clicks.csv` (date, traffic volume), `art_daily_small_noise.csv` (Numenta benchmark series)
- **Frequency:** Daily

## Objectives

- Visualize historical web traffic trends
- Build a forecasting model using Facebook Prophet
- Generate a 365-day traffic projection with upper and lower bounds
- Decompose trend, weekly, and yearly seasonality components

## Approach

1. Load and prep time series data with `ds` (date) and `y` (traffic) columns
2. Fit Prophet model to historical data
3. Build future dataframe extending 365 periods
4. Generate forecast with `yhat`, `yhat_lower`, and `yhat_upper`
5. Visualize raw traffic over time and forecasted trend
6. Plot seasonal decomposition (trend, weekly, yearly components)
7. Build interactive Plotly forecast visualization

## Key Findings

- Traffic shows a consistent trajectory through the observed period
- Forecast reveals potential plateau or decline in future periods without campaign intervention
- Weekly and yearly seasonality components are identifiable in the decomposition
- Confidence intervals widen progressively, reflecting growing uncertainty over the forecast horizon

## Tools

`Python` `Pandas` `Prophet` `Matplotlib` `Seaborn` `Plotly` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `Site-Traffic-Forecast.ipynb` | Full forecasting notebook |
| `Clicks.csv` | Historical web traffic data |
| `art_daily_small_noise.csv` | Benchmark time series for model testing |
