# Customer Shopping Trends Data Analysis

## Overview
This project involves performing data analysis on a customer shopping trends dataset using PySpark. The dataset contains information about customers, their purchases, and reviews. The analysis aims to derive insights from the data and create visualizations to present the findings.

## Prerequisites
- Python 3.x
- Apache Spark
- PySpark
- Matplotlib
- Jupyter Notebook (or your preferred Python development environment)

## Project Structure
The project is structured as follows:

- **shopping_trends_updated.csv**: The dataset containing customer shopping trends data.
- **data_analysis.py**: The Python script for performing data analysis and generating visualizations.
- **README.md**: This README file.

## Data Analysis

### 1. Data Ingestion
The project starts by setting up a Spark session and loading the dataset from a CSV file. The data is then cast to the appropriate data types.

### 2. Summary Statistics
Basic summary statistics (count, mean, std, min, max) are computed for numerical columns: 'Age', 'Purchase Amount (USD)', and 'Review Rating'.

### 3. Category Analysis
The script groups the data by 'Category' and calculates the average 'Purchase Amount (USD)' for each category. The results are stored in a PySpark DataFrame.

### 4. High Rating Purchases
The data is filtered to include only purchases with a 'Review Rating' greater than 4.0.

### 5. Location Analysis
The script groups the data by 'Location' and calculates the total purchase amount (in USD) for each location.

### 6. Gender Analysis
The data is grouped by 'Gender' to calculate the average 'Purchase Amount (USD)' for each gender.

### 7. Data Visualization
The results of the category and location analysis are converted to Pandas DataFrames and sorted in descending order. Bar charts are created to visualize the average purchase amount by category and the total purchase amount by location using Matplotlib.
