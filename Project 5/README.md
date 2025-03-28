## Project Overview
This project explores patterns and trends in the global video game market using a historical dataset of video game sales. The goal is to analyze which platforms dominated sales, how release trends evolved over time, and how data cleaning impacts analytical results.

The dataset includes information on game names, release years, platforms, publishers, user and critic scores, genres, and regional sales.

## Features & Functionality
Data Cleaning:

Converted inconsistent column headers to lowercase.

Replaced non-numeric values (e.g., TBD) in user scores with NaN.

Converted release years to integers and filtered out missing values.

Feature Engineering:

Added a total_sales column aggregating all regional sales.

Exploratory Data Analysis (EDA):

Visualized game release trends over time.

Analyzed sales patterns by platform, identifying top-performing consoles.

Data Aggregation:

Used groupby and pivot tables to summarize sales by platform and year.

Visualization:

Created clear, informative bar charts and line plots to reveal key trends.

## Key Insights
Game releases peaked in 2008–2009 with over 1,400 titles per year, followed by a decline through 2016.

The PS2, Xbox 360, and Wii emerged as the top-performing platforms based on total global sales.

Many missing scores are likely due to lower-profile games lacking widespread reviews.

## Tools & Libraries
Python 3.9+

pandas

NumPy

matplotlib

SciPy

## Requirements

Python >= 3.9
pandas >= 1.3.0
matplotlib >= 3.4.0
scipy >= 1.7.0

## Roadmap
Here are some potential improvements:

Fix inconsistent genre classification using fuzzy matching to consolidate similar categories and improve analysis accuracy.

Visualize sales by publisher using a sunburst chart to explore hierarchy between publishers, platforms, and genres.

Integrate more recent datasets from APIs or Kaggle to extend analysis beyond 2016.

Build a predictive model using linear regression or random forests to forecast game sales based on platform, genre, and ratings.

Deploy insights using a Streamlit dashboard so stakeholders can interactively filter by year, platform, or genre.

## Documentation
games.csv: Contains raw data on games, including names, platforms, genres, scores, and regional sales.

Additional processing includes total sales computation and filtering of missing or malformed data.

## Author
Created by Gabe Goodwin
Completed as part of the TripleTen Data Science Program
