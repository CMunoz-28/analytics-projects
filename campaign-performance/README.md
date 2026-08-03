# Campaign Performance Analysis

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VHaK21AB4U6sY31ncwfosff9mi3Qxm86)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/jackdaoud/marketing-data)

## Overview

Exploratory data analysis on a real-world marketing dataset to understand customer behavior, product preferences, and campaign effectiveness across different channels.

## Dataset

- **Source:** Kaggle: iFood Marketing Data
- **Size:** 2,240 customers
- **Features:** Customer profiles, product spend by category, campaign response flags, channel engagement

## Objectives

- Profile customers by age, income, and spending behavior
- Identify which product categories generate the most revenue
- Evaluate campaign success rates across all 5 campaigns
- Assess channel performance (web, store, catalog, deals)

## Approach

1. Load and inspect the dataset for null values and data types
2. Descriptive statistics across demographic and purchase features
3. Age distribution analysis using histogram and box plot
4. Food category distribution across customer base
5. Campaign success/failure comparison
6. Channel performance breakdown

## Key Findings

- Most customers fall between ages 47 and 65 (IQR); mean age is 55; a maximum of 131 was noted as a likely data entry error
- Significant spread in food spend across product categories
- Campaign performance varies by customer segment and channel
- Web and store channels drive the majority of transactions

## Tools

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `Campaign Performance.ipynb` | Full EDA notebook |
| `ifood_df.csv` | Source dataset (2,240 customers) |
