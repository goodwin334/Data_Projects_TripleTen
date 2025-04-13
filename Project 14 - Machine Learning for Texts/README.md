# Movie Review Classification: Negative Review Detection
## Project Overview
This project involves building a model to classify movie reviews as positive or negative. The dataset used comes from IMDB, with polarity labels indicating whether a review is positive or negative. The goal is to develop a model that can automatically detect negative reviews, with an objective of achieving an F1 score of at least 0.85.
The project follows these key steps:
Data Preprocessing: Load and clean the dataset to make it suitable for modeling.
Exploratory Data Analysis (EDA): Analyze the dataset, including the distribution of labels and key features.
Model Building: Use machine learning models to classify the reviews and compute the F1 score.
Model Evaluation: Evaluate model performance using metrics like F1 score, precision, recall, and accuracy.

Tools used:
Python for data processing and model building.
pandas and NumPy for data manipulation.
Matplotlib and Seaborn for data visualization.
scikit-learn for machine learning models and evaluation.


## System Requirements
Python version: 3.9+

Recommended Libraries:

pandas>=1.3

numpy>=1.21

matplotlib>=3.4

scikit-learn>=1.0

statsmodels>=0.13

## Roadmap for Improvement
Increase model performance:

Experiment with advanced models such as Random Forest, XGBoost, or BERT for text classification.

Implement hyperparameter tuning using GridSearchCV or RandomizedSearchCV to optimize the models for better performance.

Data Augmentation:

Implement text augmentation techniques like paraphrasing or back-translation to increase the dataset size.

Deep Learning:

Train a deep learning model (such as an LSTM or Transformer-based model) for more accurate text classification.

Model Deployment:

Create a simple API using Flask or FastAPI to deploy the model for real-time predictions.

## Contributors
Project Author: Gabe Goodwin
