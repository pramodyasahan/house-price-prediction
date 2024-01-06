# Housing Price Prediction Model

## Overview
This repository contains the code for a machine learning model aimed at predicting housing prices. The model is based on the RandomForestRegressor algorithm from the scikit-learn library and utilizes feature selection, preprocessing, and pipeline techniques for improved performance.

## Data
The model is trained and tested using two datasets:
- `train.csv`: Contains training data with features and sale prices.
- `test.csv`: Contains testing data with features.

## Features
The datasets include a mix of numerical and categorical features. The features are preprocessed using pipelines and transformed to suitable formats for the model.

## Preprocessing
Preprocessing steps include:
- Handling missing values:
  - Numerical features: Imputed with mean values.
  - Categorical features: Imputed with the most frequent values.
- Scaling numerical features using StandardScaler.
- Encoding categorical features using OneHotEncoder.

## Feature Selection
Feature selection is performed using Recursive Feature Elimination (RFE) with RandomForestRegressor to select the top 50 features. This helps in improving the model performance by focusing on the most relevant features.

## Model Training
The RandomForestRegressor model is trained on the preprocessed and selected features.

## Usage
To run the model:
1. Load the datasets: `train.csv` and `test.csv`.
2. Separate features (`X`) and target (`y`) in the training dataset.
3. Preprocess the features using the defined pipelines.
4. Perform feature selection to identify the top features.
5. Train the RandomForestRegressor model on the selected features.
6. Use the model to make predictions on the test dataset.

## Dependencies
- pandas
- numpy
- scikit-learn

## Note
This code is designed as a basic framework for housing price prediction and can be further optimized and tuned for better performance.
