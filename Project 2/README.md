## Instacart Customer Behavior Analysis
## Project Overview
This project explores shopping habits of customers on Instacart, an online grocery delivery platform. By cleaning and analyzing transaction and product data, the goal was to uncover patterns in customer behavior — such as popular purchase times, frequently ordered products, and shopping trends by aisle and department.

This analysis can help business stakeholders improve marketing, optimize product placement, and better understand user engagement across various product categories.

## Features & Functionality
Data Cleaning: Removed duplicate orders and products, validated schema integrity.

Multi-Table Merging: Connected multiple CSV files (orders, order_products, products, aisles, departments) into a cohesive dataset.

Temporal Analysis: Identified peak shopping hours and days of the week.

Product Trends: Investigated which products, aisles, and departments are most popular.

Visualization: Generated charts to illustrate user behavior and support conclusions.

## Key Insights
A noticeable spike in order activity during specific hours (e.g. Wednesday at 2:00 AM).

Certain aisles (like fresh fruits, baby items) consistently outperform others in volume.

A high frequency of repeat purchases for staple items, suggesting the potential for recommendation algorithms.

## Tools & Libraries
Python 3.9+

pandas for data manipulation

matplotlib / seaborn for visualizations

Jupyter Notebook for exploration and presentation


## Requirements
Python >= 3.9
pandas >= 1.3.0
matplotlib >= 3.4.0
seaborn >= 0.11.0
jupyterlab or notebook


## Roadmap
Here are future improvements you could work on:

Fix user retention analysis using reorder ratios to understand repeat behavior and loyalty.

Enhance time series analysis using datetime conversion to explore seasonality and long-term shopping trends.

Deploy interactive dashboard using Streamlit to allow dynamic filtering by aisle, product, or time.

Integrate external data (e.g., weather, holidays) to detect external factors influencing shopping behavior.

Automate data pipeline using Airflow or Prefect for real-time analysis in production environments.

## Documentation
Each data file in the project maps to the following:

orders.csv: Contains customer order logs with timestamps.

order_products.csv: Contains product items per order.

products.csv: Lists all products with product IDs.

aisles.csv: Maps product IDs to aisle categories.

departments.csv: Maps product IDs to top-level departments.

## Author
Created by Gabe Goodwin
As part of the TripleTen Data Science Program

