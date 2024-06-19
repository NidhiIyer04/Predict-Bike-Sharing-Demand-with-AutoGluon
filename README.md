# Predict Bike Sharing Demand with AutoGluon

## Project Overview

This project focuses on predicting bike-sharing demand using the AutoGluon library. The main tasks included loading and preparing the dataset, creating features, training models, making predictions, and evaluating model performance. The project is divided into the following key sections:

1. **Loading the Dataset**
2. **Feature Creation and Data Analysis**
3. **Model Training with AutoGluon**
4. **Comparing Model Performance**
5. **Competition Report**

## Loading the Dataset

- **Downloaded the Bike Sharing Demand data from Kaggle.**
  - Used the Kaggle CLI with the Kaggle API token to download and unzip the dataset into SageMaker Studio or local development environment.
- **Loaded all datasets into Pandas.**
  - Used Panda’s `read_csv()` function to load the train, test, and sample submission files into DataFrames. Ensure you can view the DataFrames in a Jupyter notebook.

## Feature Creation and Data Analysis

- **Created a feature and add it to the train and test dataset.**
  - Extracted data from one feature column and use it in a new feature column.
- **Created a histogram of all features in the train dataset.**
  - Used matplotlib to create histograms of each feature column in the train DataFrame.
- **Changed the datatype of features in the train and test dataset.**
  - Assigned category data types to feature columns initially typed as numeric values.

## Model Training with AutoGluon

- **Trained a Tabular Prediction model on the training set.**
  - Used the `TabularPredictor` class from AutoGluon to create a predictor by calling `.fit()`.
- **Changed the hyperparameters when training a Tabular Prediction model.**
  - Provided additional arguments in the `TabularPredictor .fit()` function to adjust hyperparameters.
- **Made predictions with a trained model on a test dataset.**
  - Used the trained predictor to predict new values from the test dataset.

## Comparing Model Performance

- **Submited a prediction submission from a model to Kaggle for scoring.**
  - Used the Kaggle CLI to submit predictions from the trained AutoGluon Tabular Predictor to Kaggle.
- **Graphed changes in model evaluation metrics after each iteration.**
  - Used matplotlib or Google Sheets/Excel to chart model performance metrics (e.g., using `fit_summary()` or `leaderboard()`).
- **Graphed changes to the Kaggle competition score after each iteration.**
  - Charted changes in the competition score using matplotlib or Google Sheets/Excel.

## Competition Report

- **Identified the best performing model from AutoGluon.**
  - Used `fit_summary()` or `leaderboard()` to detail the results and identify the best model.
- **Showed how EDA impacted model performance.**
  - Discussed how additional features and hyperparameter changes improved the Kaggle score.
- **Explained why changes to hyperparameters affected the model’s performance.**
  - Included a table outlining each hyperparameter used along with the corresponding Kaggle score. Explain the impact of these changes on model performance.
