Corporación Favorita Grocery Sales Forecasting

This project aims to forecast the unit sales of products sold at various Corporación Favorita grocery stores across Ecuador. The dataset includes historical sales data, information on holidays and events, and metadata about the stores and products.

Project Overview
Objective
The main objective is to build a predictive model that accurately forecasts the sales of thousands of items in Favorita stores, helping the retailer optimize inventory management and reduce waste.

Dataset Description
The dataset consists of several files:

train.csv: Historical sales data, with columns for date, store, item, and unit sales.
test.csv: Data for the prediction period without sales information.
items.csv: Metadata about items, including their category.
stores.csv: Metadata about stores, including city and type.
transactions.csv: Number of daily transactions at each store.
oil.csv: Daily oil price data.
holidays_events.csv: Information on holidays and special events.
Evaluation Metric
The performance of the model is evaluated using Root Mean Squared Logarithmic Error (RMSLE).

Key Challenges

Seasonality and Trends: Capturing different patterns in sales due to holidays, events, and other factors.
Data Volume: Efficiently managing and processing large volumes of data.
Feature Engineering: Creating meaningful features to improve model accuracy.

Solution Approach

Data Preprocessing
Handling Missing Values: Imputing or removing missing values in the dataset.
Feature Engineering: Creating new features to capture seasonality, trends, and external factors:
Lag features to capture past sales trends.
Rolling windows for moving averages.
Holiday and event indicators.
Price features from the oil data.

Modeling
Time Series Models: Implementing models specifically designed for time series forecasting (e.g., ARIMA).
Machine Learning Models: Using models like XGBoost.
Ensemble Methods: Combining multiple models to improve prediction accuracy.
Cross-Validation
Implementing appropriate cross-validation strategies to ensure model robustness and prevent overfitting.

Results
The final model’s performance is measured using RMSLE, RMSE, MSE, MAE and R2. The model is validated on a holdout set to estimate its generalization error.
