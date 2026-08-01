# Superstore Sales EDA

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cOGEsH4gTjZXt9baUsf7VYhPTCu-sGxW)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

## Overview

Business analytics and EDA on a global sales dataset spanning multiple countries and product lines. The analysis explores revenue totals, geographic performance, product category breakdown, deal size impact, and the relationship between discounts and margins.

## Dataset

- **Source:** Kaggle: Sample Superstore / Sales Dataset
- **Scope:** Global orders across multiple territories
- **Features:** QUANTITYORDERED, SALES, PRICEEACH, STATE, COUNTRY, PRODUCTLINE, DEALSIZE, ORDERDATE, and additional order-level fields

## Objectives

- Compute actual total sales and revenue figures from the dataset
- Identify top-performing countries and territories by sales volume
- Break down revenue by product line and deal size
- Explore monthly sales trends over time
- Detect and handle outliers in sales and quantity data

## Approach

1. Load dataset and inspect structure, types, and null values
2. Remove duplicate rows and validate final shape
3. Outlier detection on QUANTITYORDERED and SALES via box plots
4. IQR-based outlier removal (99th percentile threshold)
5. Aggregate total revenue and unit totals
6. Geographic breakdown: top 10 territories by sales and quantity
7. Product line revenue and unit comparison
8. Deal size distribution and average order value
9. Monthly sales trend over time
10. Correlation heatmap across financial variables

## Key Findings

- Dataset includes international orders spanning the US, Europe, and Asia-Pacific. This is a global sales dataset
- Top revenue territories are consistent across both sales volume and units ordered
- Large deals generate significantly higher average revenue per order compared to medium or small
- Higher discounts increase order volume but reduce per-unit revenue, confirming the discount-margin tradeoff
- Strong positive correlation between quantity ordered and total sales

## Tools

`Python` `Pandas` `NumPy` `Seaborn` `Matplotlib` `Plotly` `GeoPandas` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `Superstore.dataset_EDA.ipynb` | Full EDA notebook |
| `sales_data_sample.csv` | Source dataset |
