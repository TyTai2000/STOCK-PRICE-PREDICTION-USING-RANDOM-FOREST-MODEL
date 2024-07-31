# Stock Price Prediction Using Machine Learning

## Introduction
This project aims to predict the closing price of Johnson & Johnson (JNJ) stock using machine learning techniques.

## Data Collection
Historical stock price data for JNJ was collected from Yahoo Finance.

## Data Preprocessing
- Converted 'Date' column to datetime format.
- Filled missing values using forward fill.
- Created additional features like moving averages and returns.

## Feature Engineering
- Created 10-day and 50-day moving averages.
- Calculated daily returns.

## Model Training and Evaluation
- Used Random Forest Regressor for prediction.
- Achieved a Mean Absolute Error (MAE) of 0.0113.

## Model Deployment
- Saved the trained model using `joblib`.
- Created an API using Flask for making predictions.

## Conclusion
The model provides reasonably accurate predictions of the stock's closing price. Future improvements could include hyperparameter tuning and testing other machine learning models.

## How to Use
1. Clone the repository.
2. Install required packages using `pip install -r requirements.txt`.
3. Run the Flask API using `python app.py`.
4. Make POST requests to the API endpoint `/predict` with JSON input for predictions.

