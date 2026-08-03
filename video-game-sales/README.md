# Video Game Sales EDA

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1AhcZBVLpEJqTICYZ3-O_HDF88WXjRyk0)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/gregorut/videogamesales)

## Overview

End-to-end EDA on a global video game sales dataset covering North America, Europe, Japan, and other markets. The analysis walks through the full data preparation workflow including cleaning, outlier handling, and visual exploration.

## Dataset

- **Source:** Kaggle: Video Game Sales
- **Size:** 16,598 raw rows; 11,675 titles after cleaning (null Year removal and IQR outlier removal)
- **Features:** Genre, Year, NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales

## Objectives

- Profile global video game sales by region and genre
- Remove irrelevant columns, duplicates, and null values
- Detect and handle outliers across all regional sales fields
- Visualize sales distributions, correlations, and regional comparisons

## Approach

1. Load dataset and inspect column types
2. Drop non-analytical columns (Name, Platform)
3. Rename columns for readability
4. Duplicate check — 0 exact duplicate rows found
5. Null value detection and removal
6. IQR-based outlier removal across all sales columns
7. Histogram of NA_Sales distribution
8. Heatmap of sales correlations across regions
9. Scatter plot of Global Sales vs. North America Sales

## Key Findings

- Strong positive correlation between NA_Sales and Global_Sales
- Japan sales show weaker correlation with Western markets, reflecting distinct consumer preferences
- Outlier removal via IQR flagged approximately 4,600 rows; combined with 271 null Year records, final dataset is 11,675 titles
- Histogram reveals a right-skewed distribution in North American sales

## Tools

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `Videogamesales.ipynb` | Full EDA notebook |
| `vgsales.csv` | Source dataset |
