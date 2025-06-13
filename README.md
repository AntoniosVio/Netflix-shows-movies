# 📺 Netflix Shows and Movies Data Analysis

This project is a Python-based exploratory data analysis (EDA) of Netflix's catalogue of shows and movies. It uses Jupyter Notebooks to visualize trends, distributions, and insights within the dataset.

## 📊 Project Features

- Cleaned and explored Netflix data
- Analyzed the distribution of content by type, genre, release year, and country
- Visualized patterns in content ratings and durations
- Identified trends in Netflix’s content catalogue growth

## 📁 Project Structure

# Netflix Shows ETL Project

## Overview

This project extracts, transforms, and loads (ETL) the Netflix shows dataset from Kaggle.  
The process cleans the data, validates quality, and saves a cleaned CSV file for analysis.

## Data Source

- Dataset from [Kaggle Netflix Shows](https://www.kaggle.com/shivamb/netflix-shows)

## ETL Steps

1. **Extract:** Load raw CSV data.
2. **Transform:** Clean missing values, convert dates, split genres.
3. **Validate:** Check for missing values, duplicates, and reasonable release years.
4. **Load:** Save cleaned data to CSV.
5. **Automate:** ETL script `etl_netflix.py` for easy reuse.
6. **Logging:** Logs progress and errors to `etl_netflix.log`.

## How to Run

```bash
python etl_netflix.py


