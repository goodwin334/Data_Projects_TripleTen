## Car Price Prediction for Rusty Bargain
### Project Overview
This project was developed for Rusty Bargain, a used car sales service launching a new app that allows users to estimate the market value of their vehicles. Using historical sales data—including technical specifications, model details, and registration information—the goal is to build a predictive model that delivers accurate, fast, and efficient price estimates.

Rusty Bargain specifically cares about:

Prediction accuracy

Speed of predictions

Training efficiency

## Features & Functionality
Data Cleaning:

Standardized column names using regex formatting.

Removed unrealistic registration_year values (<1950 or >2017).

Filtered out extreme outliers in engine power.

Handled missing data in features like vehicle_type, fuel_type, gearbox, and not_repaired.

Feature Engineering:

One-hot encoding for categorical features.

Numeric scaling and validation for regression.

Model Training:

Baseline sanity check with LinearRegression.

Hyperparameter-tuned DecisionTreeRegressor and RandomForestRegressor.

Advanced modeling with GradientBoostingRegressor.

Evaluation Metrics:

Used RMSE (Root Mean Squared Error) for model performance.

Compared training time, prediction speed, and accuracy across models.

## Key Insights
Random Forest offered the best trade-off between speed and accuracy.

Gradient Boosting delivered the best predictive performance but at a higher computational cost.

Cleaning extreme values in registration_year and power significantly improved model stability.

## Tools & Libraries
Python 3.9+

pandas

NumPy

scikit-learn

matplotlib / seaborn

re (for column name normalization)

## System Requirements
Python >= 3.9
pandas >= 1.3.0
numpy >= 1.21.0
scikit-learn >= 0.24.0
matplotlib >= 3.4.0
seaborn >= 0.11.0


## Roadmap for Improvement
Fix feature correlation issues using PCA or feature selection to reduce model complexity without accuracy loss.

Improve categorical encoding using Target or Frequency Encoding for high-cardinality features like model.

Use cross-validation with stratified folds to improve model generalization.

Deploy as a Streamlit app where users can input car features and get instant price estimates.

Integrate real-time model logging to track prediction confidence and drift over time.

## Project Documentation
car_data.csv: Historical car listings with features like model, registration year, power, mileage, fuel type, and price.

Notebook walks through full analysis: cleaning, EDA, modeling, evaluation.

## Author
Created by Gabe Goodwin

Completed as part of the TripleTen Data Science Program
