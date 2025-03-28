## Chicago Cab Trip Analysis
## Project Overview
This project analyzes cab trip data from the Chicago metro area. The aim is to uncover which neighborhoods and companies are the most frequently used, how trip durations vary by weather conditions, and what factors influence travel demand across the city.

Using multiple SQL-generated datasets, we explore key patterns and apply statistical testing to understand the real-world effects of weather on trip times. This data is vital for transportation planning, fleet optimization, and understanding user behavior.

## Features & Functionality
Data Ingestion: Loaded multiple .csv datasets exported from SQL queries.

Data Cleaning: Checked for and removed duplicate rows.

Top Rankings:

Identified the top 10 cab companies based on trip volume.

Ranked neighborhoods by average number of trip drop-offs.

Visualization:

Created bar charts of top-performing cab companies and high-traffic neighborhoods.

Weather Impact Analysis:

Used hypothesis testing (scipy.stats.ttest_ind) to evaluate whether weather conditions affect trip duration.

Compared average trip durations during good vs. bad weather conditions.

## Key Insights
Flash Cab is the most frequently used cab company, significantly outpacing competitors.

The Loop, River North, Streeterville, and West Loop are the most common drop-off neighborhoods.

Trip durations are significantly longer during bad weather, with the t-test showing a statistically significant difference.

## Tools & Libraries
Python 3.9+

pandas

NumPy

Matplotlib

SciPy (for statistical testing)

Jupyter Notebook

## System Requirements

Python >= 3.9
pandas >= 1.3.0
matplotlib >= 3.4.0
scipy >= 1.7.0
jupyterlab or notebook

## Roadmap for Improvement
Fix inaccurate or generic weather labels using detailed weather APIs to improve the granularity of environmental analysis.

Integrate spatial analysis using geopandas to visualize trip patterns geographically across Chicago neighborhoods.

Create a time-series analysis module using hourly trip data to detect demand peaks and optimize fleet availability.

Build a Streamlit dashboard for interactive exploration of cab usage by time, company, and weather.

Automate data retrieval from Chicago's open data portal to keep insights up to date.

## Documentation
File	Description
project_sql_result_01.csv	Trip counts by company
project_sql_result_04.csv	Average trips by neighborhood
project_sql_result_07.csv	Trip durations with weather conditions
All datasets were generated using SQL queries and loaded into pandas DataFrames for further analysis and visualization.

## Author
Created by Gabe Goodwin
Completed as part of the TripleTen Data Science Program
