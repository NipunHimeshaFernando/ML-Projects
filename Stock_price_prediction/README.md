# Stock Price Prediction App (Machine Learning)

A machine learning project that predicts future stock prices using historical financial data.  
This application uses **Random Forest Regression** to forecast Apple (AAPL) stock closing prices 10 days ahead based on historical trends.

---

## Project Overview

This project demonstrates how supervised machine learning can be applied to financial time-series data for predictive analysis.

- Stock data collected from **Yahoo Finance**
- Historical period: **2010 – 2019**
- Target stock: **Apple Inc. (AAPL)**
- Forecast horizon: **10 days ahead**
- Model used: **Random Forest Regressor**
- Evaluation metric: **Root Mean Squared Error (RMSE)**

---

## Features

- Historical stock data extraction using financial APIs
- Data preprocessing and feature engineering
- 10-day future price forecasting
- Ensemble learning using Random Forest
- Model performance evaluation using RMSE
- Visualization of predicted vs actual stock prices
- Clean and structured implementation

---

## Technologies Used

- **Python**
- **Scikit-learn**
- **NumPy**
- **Matplotlib**
- **yFinance**

---

## How the Model Works

### 1️ Data Collection

Historical stock price data is downloaded for Apple (AAPL).

### 2️ Data Preparation

- Only the **closing price** is selected as the main feature.
- A shifted target column is created to represent the closing price 10 days in the future.
- Rows with missing values are removed.

### 3️ Model Training

- Dataset split into training and testing sets (80/20).
- Random Forest Regressor trained using 500 decision trees.
- Model learns patterns between current and future stock prices.

### 4️ Model Evaluation

- Predictions generated on test data.
- Performance measured using **RMSE**.

### 5️ Visualization

- Last 10 predictions compared with actual values.
- Results plotted using Matplotlib.
