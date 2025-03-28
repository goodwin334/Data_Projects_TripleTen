## Customer Plan Recommendation with Classification Models
## Project Overview
This project analyzes user behavior data from a mobile phone carrier to predict which plan a customer should switch to: Smart or Ultra. The company has data on users who transitioned from legacy plans to these new ones, and this project builds machine learning models to automate future recommendations.

Using logistic regression, decision trees, and random forests, the analysis evaluates the accuracy of each model and tunes hyperparameters to find the most effective predictor.

## Features & Functionality
Data Preprocessing:

Imported and split the dataset into features and a binary target variable (is_ultra).

Divided the data into training, validation, and test sets (60%/20%/20%).

Model Training:

Trained three classifiers:

Logistic Regression

Decision Tree (with hyperparameter tuning)

Random Forest (with default settings)

Model Evaluation:

Assessed each model using accuracy scores and classification reports.

Optimized the decision tree using a grid search over max_depth and min_samples_split.

Goal:

Select the model that best predicts which plan is best for each user based on their past usage data.

## Key Insights
Decision Tree Classifier with tuned hyperparameters yielded the highest validation accuracy.

Logistic Regression performed well but slightly under the tree-based models.

Proper splitting into training, validation, and test sets helped ensure generalizable results.

## Tools & Libraries
Python 3.9+

pandas, NumPy

scikit-learn

Jupyter Notebook

## Requirements

Python >= 3.9
pandas >= 1.3.0
numpy >= 1.21.0
scikit-learn >= 0.24.0
jupyterlab or notebook

## Roadmap
Future improvements to the project:

Fix data imbalance using SMOTE to enhance performance for underrepresented classes and reduce false positives.

Improve accuracy by using a GridSearchCV across all models to tune multiple hyperparameters simultaneously.

Incorporate cross-validation scoring with stratified folds to further validate performance consistency.

Deploy the best model using Flask or FastAPI so users can receive real-time recommendations via a web interface.

Log feature importance from tree models to provide insight into which user behaviors influence plan selection.

## Documentation
users_behavior.csv: Dataset including customer usage patterns and current plan label.

Features include minutes, messages, and mb_used among others.

Target variable: is_ultra (binary: 1 for Ultra plan, 0 for Smart plan).

## Author
Created by Gabe Goodwin
Completed as part of the TripleTen Data Science Program
