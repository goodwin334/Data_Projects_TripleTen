## Machine Learning Solutions for Insurance Analytics
### Project Overview
This project was developed for Sure Tomorrow, an insurance company exploring how machine learning can optimize business processes. The dataset contains anonymized customer information including age, income, family members, and insurance benefits.

The project is divided into four tasks, each solving a specific business problem using different machine learning techniques:

Customer Similarity Search for targeted marketing

Binary Classification to predict benefit eligibility

Regression to estimate number of benefits a customer may receive

Data Obfuscation to secure personal information while preserving model performance

## Features & Functionality
### Task 1: Similarity Search (KNN)
Used K-Nearest Neighbors algorithm to find customers similar to a given profile.

Enables personalized marketing outreach and recommendations.

### Task 2: Benefit Eligibility Prediction (Classification)
Implemented and evaluated a Logistic Regression model.

Compared results with a dummy baseline model.

Achieved higher accuracy, precision, and recall, confirming model usefulness.

### Task 3: Predicting Number of Benefits (Regression)
Built a Linear Regression model to predict insurance_benefits.

Evaluated with MAE and R² scores.

Used real-world interpretation to validate predictions.

### Task 4: Data Masking & Privacy
Developed a matrix transformation algorithm to obfuscate personal data.

Demonstrated that the model still performs equally well after obfuscation.

Proved the viability of secure ML pipelines in privacy-sensitive industries.

## Key Insights
Logistic regression performed well in predicting whether a customer is likely to receive benefits.

Income and age were the most impactful features in both classification and regression models.

Data obfuscation using matrix operations preserved predictive performance, proving that sensitive information can be masked without compromising model accuracy.

## Tools & Libraries
Python 3.9+

pandas

NumPy

matplotlib / seaborn

scikit-learn

## System Requirements
Python >= 3.9
pandas >= 1.3.0
numpy >= 1.21.0
matplotlib >= 3.4.0
seaborn >= 0.11.0
scikit-learn >= 0.24.0

## Roadmap for Improvement
Fix overfitting using regularization in logistic regression to improve generalization.

Use PCA or feature selection techniques to simplify similarity search.

Add cross-validation for model evaluation to improve metric reliability.

Integrate an interactive Streamlit UI for agents to explore customer clusters and predictions securely.

Implement adversarial testing on obfuscated data to validate privacy robustness.

## Credits
Created by: Gabe Goodwin

Program: TripleTen Data Science Bootcamp
