# Superstore Sales EDA

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cOGEsH4gTjZXt9baUsf7VYhPTCu-sGxW)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

## Overview

Business analytics and EDA on a retail superstore sales dataset. The analysis explores sales volume, profitability by state, quantity-price relationships, and the impact of discounts on margins.

## Dataset

- **Source:** Kaggle — Sample Superstore Dataset
- **Features:** QUANTITYORDERED, SALES, PRICEEACH, STATE, and additional order-level fields

## Objectives

- Summarize total sales and profitability figures
- Identify top-performing states by sales and profit
- Explore the relationship between discounts, sales volume, and margins
- Detect and handle outliers in sales and quantity data

## Approach

1. Load dataset and inspect structure, types, and null values
2. Remove duplicate rows and validate final shape
3. Outlier detection on QUANTITYORDERED and SALES via box plots
4. IQR-based outlier removal (99th percentile threshold)
5. Aggregate total sales and profit figures
6. Bar charts for top 10 states by sales and profit
7. Scatter plot for interdependence of sales, quantity, and price
8. Pair plots and correlation heatmap for financial variables

## Key Findings

- **Top states by sales and profit:** CA, MA, NY, NSW, Victoria, PA, CT, BC, NH, Tokyo
- Higher discounts correlate with increased sales volume but reduced profit margins
- Technology category shows stronger profit performance due to lower average discount rates
- Positive correlation between sales and quantity ordered, weaker with price per item

## Tools

`Python` `Pandas` `NumPy` `Seaborn` `Matplotlib` `Plotly` `GeoPandas` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `Superstore.dataset_EDA.ipynb` | Full EDA notebook |
| `sales_data_sample.csv` | Source dataset |
