## Customer Churn Prediction Using Supervised Learning
## Project Overview
This project focuses on predicting customer churn for a retail bank using supervised machine learning models. Customer churn refers to clients leaving the bank, which can be costly. Since retaining existing customers is cheaper than acquiring new ones, predicting churn in advance enables the bank to take action and improve retention.

The dataset includes a variety of customer features (e.g., credit score, geography, gender, balance, tenure), and the target variable Exited indicates whether a customer left the bank.

## Features & Functionality
Data Preprocessing:

Filled missing values (e.g., Tenure) with mean values instead of deleting records.

Removed irrelevant columns such as Surname and CustomerId.

Encoded categorical variables using One-Hot Encoding.

Scaled numerical features using StandardScaler.

Dataset Splitting:

Train (60%), Validation (20%), Test (20%) split using train_test_split.

Model Training:

Trained and evaluated the following classifiers:

Logistic Regression

Decision Tree

Random Forest

Evaluation Metrics:

Accuracy

Precision

Recall

F1 Score (main metric)

ROC AUC Score

## Key Insights
Random Forest consistently produced the best F1 Score among tested models, making it the most effective at identifying potential churners.

Data imbalance and feature correlation played key roles in model behavior.

Tenure, Balance, and Geography were important predictors.

## Tools & Libraries
Python 3.9+

pandas

NumPy

scikit-learn

Jupyter Notebook

## Requirements

Python >= 3.9
pandas >= 1.3.0
numpy >= 1.21.0
scikit-learn >= 0.24.0

## Roadmap
To further improve the project:

Fix class imbalance using SMOTE or class weighting to improve recall on minority class (churners).

Use GridSearchCV with cross-validation to optimize model hyperparameters more systematically.

Build a pipeline using Pipeline and GridSearchCV to streamline model tuning and preprocessing.

Deploy the model using Flask or FastAPI to make real-time churn predictions from a web form.

Add feature importance visualization using SHAP to better understand what drives churn.

## Documentation
File	Description
Churn.csv	Bank customer dataset with features and churn labels
Sprint Project 8.ipynb	Full notebook including EDA, preprocessing, modeling, and evaluation
Target column: Exited (1 = churned, 0 = stayed)
Feature columns include CreditScore, Geography, Gender, Age, Balance, Tenure, and more.

## Author
Created by Gabe Goodwin
Completed as part of the TripleTen Data Science Program
