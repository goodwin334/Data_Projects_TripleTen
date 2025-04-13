# Age Prediction from Faces
Age Prediction for Alcohol Purchase Classification

## Project Description
The goal of this project is to predict the age of individuals buying alcohol based on images of their faces. The project leverages neural networks for image classification, with the objective of achieving the highest accuracy in predicting age. This task involves the use of ImageDataGenerator to load images efficiently, given the large size of the dataset.

# Features & Functionality
## Data Analysis & Preprocessing

Loaded the labels CSV file containing file_name and real_age columns.

Images are stored in the /datasets/faces/ folder, and the ImageDataGenerator is used to load images with specific configurations (e.g., validation split, rescaling).

## Modeling Techniques

Built neural networks using TensorFlow and Keras.

Tuned model layers to improve age prediction accuracy.

## Evaluation Metrics

The primary evaluation metric is prediction accuracy, focusing on minimizing prediction error for age classification.

## System Requirements
Make sure your environment meets the following requirements:

bash
Copy
Python >= 3.7
pandas >= 1.1.0
tensorflow >= 2.4.0
Install dependencies with:

bash
Copy
pip install pandas tensorflow

## Roadmap for Improvement

Improve Model Accuracy

Experiment with advanced models like ResNet, VGG, or EfficientNet to capture more intricate details in facial features.

Implement hyperparameter tuning using techniques such as GridSearchCV or RandomizedSearchCV to optimize the neural network layers for better accuracy.

Model Regularization

Implement dropout layers and L2 regularization to reduce overfitting and improve model generalization.

Data Augmentation

Increase the dataset size by implementing more robust data augmentation techniques (e.g., rotation, flipping, or zooming).

Model Deployment

Convert the trained model into a REST API using Flask or FastAPI for real-time age predictions.

## Contributors

Gabe Goodwin

Program: TripleTen Data Science Bootcamp
