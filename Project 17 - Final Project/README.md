# Customer Churn Prediction
## Project Name
Customer Churn Prediction for Telecom Service

## Project Description
This project involves analyzing customer data to predict churn in a telecom company. The goal is to use demographic and service usage data to identify patterns that help predict whether a customer is likely to churn. The model will help the company proactively address customer retention strategies by identifying at-risk clients.

The business requirement is to accurately predict customer churn and provide insights into the factors contributing to churn.

# Features & Functionality
## Data Analysis

Analyzed customer data for null values and adjusted data types.

Created new features like customer tenure and churn status to help predict churn.

Visualized distributions of categorical variables to understand customer preferences and identify imbalances.

## Modeling Techniques

Preprocessed data by encoding categorical features using One-Hot Encoding and binary features using Ordinal Encoding.

Scaled numerical features to improve model performance.

Trained several machine learning models (Logistic Regression, Random Forest, etc.) and evaluated them based on the AUC-ROC score.

Tuned the best model to improve its predictive power.

## Evaluation Metrics

AUC-ROC score was used as the key metric to evaluate the performance of models.

The best model achieved a strong performance, which will be further improved with hyperparameter tuning.

## System Requirements
Make sure your environment meets the following requirements:

Python >= 3.6
pandas >= 1.2.3
numpy >= 1.19.5
matplotlib >= 3.4.2
scikit-learn >= 0.24.2

## Roadmap for Improvement

Fix model performance by tuning hyperparameters using GridSearchCV to improve the AUC-ROC score.

Investigate and apply techniques like SMOTE to handle class imbalance in the target variable (churn).

Improve model explainability by implementing SHAP (SHapley Additive exPlanations) to interpret feature importance.

Deploy the final model as a web service using Streamlit or FastAPI.

## Contributors
Author: Gabe Goodwin
Program: TripleTen Data Science Bootcamp
