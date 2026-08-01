# Google Play Store SQL Analysis

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1C0_RPDxFYskiXCx-uV0Y0Z9e9ViJNGeT)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)](https://sqlite.org/)
[![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

## Overview

SQL-based analysis of the Google Play Store dataset using SQLite3 within Python. Combines structured querying with Pandas and visualization to surface insights on app ratings, installs, categories, and pricing across 10,841 apps.

## Dataset

- **Source:** Kaggle: Google Play Store Apps
- **Size:** 10,841 apps, 34 categories
- **Features:** App, Category, Rating, Reviews, Size, Installs, Type, Price, Content Rating, Genres, Last Updated, Current Ver, Android Ver

## Objectives

- Load Play Store data into a SQLite3 database for structured querying
- Identify top-rated and most-installed app categories
- Compare free vs. paid app distribution and pricing
- Analyze content rating distribution and update frequency

## Approach

1. Load CSV into a Pandas DataFrame and inspect structure
2. Data cleaning: handle missing ratings, format Installs and Size columns
3. Ingest DataFrame into SQLite3 in-memory database
4. SQL queries for category-level aggregations (avg rating, total installs)
5. Free vs. paid breakdown by category and price range
6. Content rating and Android version distribution via SQL
7. Visualization of query results using Matplotlib and Seaborn

## Key Findings

- Dataset spans 34 categories with significant variation in app volume and rating quality
- Free apps dominate across all categories; paid apps cluster in Education and Productivity
- Top-installed categories include Communication, Social, and Video Players
- Data quality issues in Rating and Installs columns require preprocessing before aggregation

## Tools

`Python` `SQLite3` `Pandas` `Matplotlib` `Seaborn` `Google Colab`

## Files

| File | Description |
|------|-------------|
| `GooglePlayStore_SQL.ipynb` | Full SQL + EDA notebook |
| `google_play_store.csv` | Source dataset (10,841 apps) |
