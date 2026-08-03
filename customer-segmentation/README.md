# Customer Segmentation

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E2hXjK6Ebm6sBgajwvGzdF9tLiOBqTtB)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

## Overview

Applied K-Means clustering to segment mall customers by annual income and spending behavior. The goal was to identify distinct customer groups that can inform targeted marketing strategies.

## Dataset

- **Source:** Kaggle: Mall Customer Segmentation
- **Size:** 200 customers
- **Features:** CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100)

## Objectives

- Understand the distribution of customer demographics and spend
- Identify the optimal number of clusters using the elbow method
- Segment customers and profile each cluster
- Visualize clusters in 2D and 3D space

## Approach

1. Data inspection, null checks, and descriptive statistics
2. Outlier detection via box plots on Age, Income, and Spending Score
3. Univariate analysis: age distribution histogram
4. Bivariate analysis: income vs. spending score scatter
5. Multivariate analysis: income, spending, age, and gender breakdown
6. Log transformation and StandardScaler normalization
7. K-Means clustering with elbow method (k=1 to 10)
8. Final model with k=3 and 3D cluster visualization

## Key Findings

- Optimal cluster count: **3 segments**
- **Cluster 0:** Mid income (~$63k), mid spend (score 55): balanced, moderately engaged customers; median age 52
- **Cluster 1:** High income (~$81k), low spend (score 13): high earners who are not converting to high spenders; median age 30
- **Cluster 2:** Low income (~$23.5k), low-to-mid spend (score 39.5): budget-constrained segment; median age 27
- Age patterns differ by cluster: younger customers (Cluster 2) show the lowest income but do not have the lowest spend scores

## Tools

`Python` `Pandas` `NumPy` `Scikit-learn` `Matplotlib` `Seaborn` `Plotly` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `Customer Segmentation.ipynb` | Full EDA and clustering notebook |
| `Mall_Customers.csv` | Source dataset |
