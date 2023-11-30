# Seoul Bike Sharing Demand Prediction


## Introduction

This notebook focuses on predicting bike-sharing demand in Seoul using various machine learning models. The dataset contains information such as date, hour, weather conditions, and the count of rented bikes. The ultimate goal is to develop a model that accurately predicts bike rental counts based on the given features.

## Data Preprocessing

    The initial dataset consists of 14 columns with various data types, including datetime, numerical, and categorical.
    Converted 'Functioning Day' and 'Holiday' columns to binary (1 for 'Yes' and 0 for 'No').
    Converted the 'Date' column to the datetime format.
    Checked and found no missing values in the dataset.
    Removed rows where the bike count is zero and 'Functioning Day' is zero.
    Created additional features such as day of the week, day, month, and season indicators.
    Utilized one-hot encoding for the 'Seasons' column and dropped the original column.
    Mapped weekdays to numerical values.

## Exploratory Data Analysis (EDA)

    Explored the distribution of bike rentals based on different factors, such as day of the week, month, hour, and season.
    Visualized the bike rental count per day of the week and season.

## Feature Engineering

    Created categorical temperature and rainfall features to group them into intervals.
    Visualized the correlation matrix to identify highly correlated features and dropped 'Dew point temperature(°C)'.

## Model Building

Implemented several machine learning models for prediction:

    Linear Regression
    K-Nearest Neighbors Regressor
    Polynomial Regression
    Random Forest Regressor
    Stacking Regressor
    Bagging Regressor
    Neural Network

## Model Evaluation

    Evaluated models using metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared (R2).
    Normalized the metrics to compare their relative performance.

## Radar Chart

    Visualized the normalized metrics using a radar chart to compare the models.

## Conclusion

    The neural network and stacking regressor models performed well in predicting bike rental counts.
    Further fine-tuning and hyperparameter optimization could enhance model performance.
    The choice of the best model depends on the specific requirements and constraints of the application.

