## Predicting Gold Recovery Rates in Industrial Mining
## Project Overview
This project tackles the challenge of predicting the recovery rate of gold from ore at various stages of a real-world industrial mining process. The mining company wants to maximize gold recovery efficiency, minimize waste, and improve decision-making in the production pipeline. This analysis helps evaluate the effectiveness of the process and builds predictive models using real production data.

## Features & Functionality
Data Preprocessing:

Handled significant missing values using forward and backward fill.

Identified and analyzed duplicate records.

Calculated target recovery metrics using the given formula.

Data Validation:

Compared provided recovery rates with calculated ones using MAE (Mean Absolute Error).

Confirmed high accuracy between reported and derived values.

Exploratory Data Analysis:

Visualized feature distributions with boxplots and correlation analysis.

Modeling:

Built multiple regression models including:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Used custom metrics and cross-validation for model evaluation.

## Key Insights
The calculated recovery metric closely matched the reported one with very low MAE, validating the quality of the data.

After filling missing values using forward and backward fill, model performance significantly improved.

Random Forest Regression performed the best in terms of predictive accuracy and robustness.

## Tools & Libraries
Python 3.9+

pandas — data wrangling

NumPy — numerical operations

scikit-learn — modeling and evaluation

seaborn / matplotlib — data visualization

## System Requirements
Python 3.9+

pandas >= 1.3.0

numpy >= 1.21.0

matplotlib >= 3.4.0

seaborn >= 0.11.0

scikit-learn >= 0.24.0

Jupyter Notebook or JupyterLab

## Roadmap
Ideas to improve the project:

Fix potential data leakage using better train-test split based on timestamps to simulate real-time predictions.

Use feature selection techniques like PCA or SHAP to reduce dimensionality and highlight most impactful features.

Add rolling average features using time windows to capture trends and smooth out noise.

Deploy model using FastAPI or Streamlit so plant operators can upload batch data and receive predictions in real time.

Visualize model predictions vs. actual recovery in real time for QA/QC teams to monitor accuracy.

## Documentation
Data Sources

gold_recovery_train.csv: Training dataset with full production process features and target values.

gold_recovery_test.csv: Test set used for model evaluation.

gold_recovery_full.csv: Combined data for EDA and metrics calculation.

👤 Author
Created by Gabe Goodwin

Completed as part of the TripleTen Data Science Program
