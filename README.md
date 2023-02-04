# Time-Series-Forecasting-with-XGBoost
This repository contains code to perform time series forecasting using XGBoost on the "American Energy Consumption AEP_hourly.csv" dataset.

# Dependencies
The code in this repository requires the following libraries:

pandas
numpy
xgboost
scikit-learn
# Pre-processing
The first step is to pre-process the data. This involves handling missing values and transforming the data into a suitable format for machine learning. In this code, missing values are dropped and the Datetime column is converted to a datetime format and set as the index.

#Feature Engineering
Next, lagged variables are added as predictors. This involves shifting the target variable by a number of time steps to create new variables that can be used as input to the XGBoost model.

#Model Training and Evaluation
The pre-processed and feature-engineered data is then split into a training set and a test set. The XGBoost model is trained on the training set and its performance is evaluated on the test set by computing the Root Mean Squared Error (RMSE).

#Forecasting
Finally, the trained XGBoost model is used for forecasting by making predictions on new, unseen data.

#Usage
To run the code, simply clone this repository and run the time_series_forecasting_xgboost.py file in a Python environment with the necessary dependencies installed. The code will output the RMSE of the XGBoost model and perform forecasting on the test set.

#Conclusion
This repository provides a simple example of how to perform time series forecasting using XGBoost on the "American Energy Consumption AEP_hourly.csv" dataset. This code can be used as a starting point for further experimentation and optimization.
