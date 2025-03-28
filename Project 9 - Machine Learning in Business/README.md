## Oil Field Profitability Prediction
## Project Overview
This project uses machine learning to identify the most profitable oil wells to drill in one of three regions. The primary objective is to help a petroleum company make data-driven decisions about where to invest a $100 million drilling budget. Each well costs $500,000 to develop and generates $4.50 per barrel of oil. The challenge is to determine which region and which 200 wells will yield the highest profit based on predicted reserves.

## Features & Functionality
Data Loading & Cleaning:

Imported datasets from three regions.

Checked and removed duplicate entries.

Exploratory Data Analysis:

Box plots and KDE plots to visualize feature distributions and reserve values.

Modeling & Predictions:

Linear regression models trained on 500 wells per region.

Prediction of oil reserves (target variable: product).

Evaluated RMSE for each region’s model.

Revenue Simulation:

Selected top 200 wells per region based on predicted reserves.

Calculated expected revenue and profit margins.

Region Recommendation:

Compared all three regions to identify the best place to drill based on projected return on investment and model confidence.

## Key Insights
Region 0 and Region 2 have similar reserve distributions, but Region 2 showed slightly more consistent returns.

Region 1 had higher variability and slightly weaker prediction performance based on RMSE.

Region 2 was selected as the best region due to its stable distribution and high return among top wells.

## Tools & Libraries
Python 3.9+

pandas

NumPy

seaborn

matplotlib

scikit-learn

## Requirements
Python >= 3.9

pandas >= 1.3.0

numpy >= 1.21.0

matplotlib >= 3.4.0

seaborn >= 0.11.0

scikit-learn >= 0.24.0

## Roadmap
Here’s how this project could be improved further:

Fix model limitations using ensemble methods (like Random Forest) to account for nonlinear relationships in reserves.

Use cross-validation with multiple samples to improve robustness of well selection.

Add confidence interval visualizations to quantify risk in revenue forecasts.

Build a Streamlit app for region/well selection to allow dynamic user inputs and interactive predictions.

Use geospatial analysis (with GeoPandas or Folium) to visualize well locations and optimize logistics.

## Documentation
Datasets
File	Description
geo_data_0.csv	Oil well feature and reserve data for Region 0
geo_data_1.csv	Data for Region 1
geo_data_2.csv	Data for Region 2
All datasets include 3 feature columns (f0, f1, f2) and a product column (barrels of oil expected per well).

## Author
Created by Gabe Goodwin
Completed as part of the TripleTen Data Science Program
