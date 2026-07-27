# Conversion Rate EDA

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QPWmAWBShi0KYpqqMaq5m__a7kRUZQdM)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)

## Overview

Exploratory data analysis on a multi-channel marketing campaign dataset to understand how clicks, impressions, and engagement translate to conversions. Examines campaign-level performance across different types, audiences, and channels.

## Dataset

- **Source:** Marketing campaign dataset
- **Features:** Campaign_ID, Campaign_Type, Target_Audience, Channel_Used, Clicks, Impressions, Engagement_Score, Conversion_Rate, Acquisition_Cost, ROI, Customer_Segment, Date

## Objectives

- Assess data quality and distribution of key campaign metrics
- Identify outliers in clicks, impressions, and engagement
- Analyze conversion rates by campaign type and channel
- Surface patterns in ROI and acquisition cost

## Approach

1. Load dataset and perform null checks and type validation
2. Descriptive statistics on numerical campaign metrics
3. Duplicate row removal and data cleaning
4. Outlier detection using box plots for Clicks, Engagement_Score, and Impressions
5. EDA on conversion rates, ROI, and channel distribution

## Key Findings

- Campaign dataset is complete with no missing values
- Outliers identified in click volume and impression counts
- Engagement score distribution varies significantly across campaign types
- Conversion and ROI patterns differ by channel and audience segment

## Tools

`Python` `Pandas` `NumPy` `Seaborn` `Matplotlib` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `Conversion.EDA.ipynb` | Full EDA notebook |
| `marketing_campaign_dataset.csv` | Source dataset |
