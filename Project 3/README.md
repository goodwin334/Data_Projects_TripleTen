## Megaline Mobile Plan Revenue Analysis
## Project Overview
Megaline, a telecom operator, offers two prepaid mobile plans: Surf and Ultimate. The commercial team wants to determine which plan generates more revenue to inform future advertising and customer acquisition strategies.

This project performs a preliminary analysis on 500 customers using various datasets including call records, internet usage, text messaging behavior, and plan specifications. The goal is to assess customer usage behavior and statistically evaluate which plan is more profitable.

## Features & Functionality
Data Cleaning & Transformation: Unified separate datasets for calls, messages, internet, and users into a consistent format. Rounded up usage data to reflect billable units (minutes, MB, messages).

Revenue Calculation: Computed monthly revenue for each user based on their usage and plan terms, including overage charges.

Exploratory Data Analysis: Identified trends in usage patterns across the Surf and Ultimate plans.

Statistical Testing: Performed hypothesis testing (two-sample t-test) to determine whether the difference in revenue between plans is statistically significant.

Visualization: Created histograms and bar charts to visualize usage behavior and revenue distribution.

## Key Insights
The Ultimate plan has a higher base cost but includes generous allowances that most users don’t exceed.

The Surf plan users often go over their monthly limits, resulting in frequent overage charges that boost revenue.

Hypothesis testing confirmed that the revenue from Surf users is significantly different (and slightly higher on average) than that from Ultimate users.

## Tools & Libraries
Python 3.9+

pandas for data manipulation

NumPy for numerical operations

matplotlib for data visualization

SciPy for statistical tests

Jupyter Notebook for documentation and interactivity

## Requirements
bash
Copy
Edit
Python >= 3.9
pandas >= 1.3.0
matplotlib >= 3.4.0
scipy >= 1.7.0
jupyterlab or notebook


## Roadmap
Planned improvements include:

Fix plan matching using billing date normalization to ensure consistent monthly revenue grouping.

Enhance revenue modeling using time-based plan churn assumptions to reflect real user behavior.

Build an interactive dashboard using Streamlit to dynamically explore customer usage by plan or region.

Automate monthly report generation using Jupyter nbconvert and scheduling tools for production-ready analytics.

## Documentation
Each dataset used in this project includes:

megaline_users.csv: User profiles with assigned plans and regions.

megaline_calls.csv: Outgoing call logs with duration and user mapping.

megaline_messages.csv: Sent SMS message logs.

megaline_internet.csv: Internet data usage per session in MB.

megaline_plans.csv: Plan definitions with cost and included service thresholds.

## Author
Created by Gabe Goodwin
Completed as part of the TripleTen Data Science Program

