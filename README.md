# Time-series-Analysis
Time Series Analysis & Forecasting on Stock Market Data
🔍 Project Overview

This project demonstrates a comprehensive Time Series Analysis workflow using real-world stock market data (Apple and Tesla).
It covers everything from data collection and visualization to stationarity testing, decomposition, forecasting models, multivariate analysis, smoothing techniques, and missing value handling.

The goal is to analyze stock price behavior over time and apply classical statistical time series models for forecasting and evaluation.

🧠 Key Concepts Covered

This project includes practical implementation of:

Time Series visualization

Trend, seasonality, and residual analysis

Stationarity (weak & strict)

Statistical hypothesis testing

Forecasting models (univariate & multivariate)

Model evaluation metrics

Data preprocessing and missing value handling

📊 Dataset

Source: Yahoo Finance (yfinance)

Stocks Used:

Apple Inc. (AAPL)

Tesla Inc. (TSLA)

Frequency: Daily closing prices

Time Period:

From 2023–2024

🔧 Technologies & Libraries Used
Python
NumPy
Pandas
Matplotlib
yfinance
statsmodels
scikit-learn
SciPy

📈 Data Visualization

Line plots of stock closing prices

Trend visualization

Rolling statistics

Smoothing techniques:

Simple Moving Average (SMA)

Weighted Moving Average (WMA)

Exponential Moving Average (EMA)

🧩 Time Series Decomposition

Two decomposition techniques are applied:

1️⃣ Classical Decomposition

Additive model

Components:

Trend

Seasonal

Residual

Period = 30 days

2️⃣ STL Decomposition

Robust seasonal-trend decomposition using LOESS

Better handling of non-linear trends

📉 Stationarity Analysis
Weak Stationarity Tests

ADF (Augmented Dickey-Fuller Test)

KPSS Test

Interpretation of:

Test statistics

p-values

Critical values

Strict Stationarity

Simulated stationary vs non-stationary data

Kolmogorov–Smirnov (K-S) Test to compare distributions over time

🔄 Making Data Stationary

Multiple techniques applied:

Differencing

First-order

Second-order

Transformations

Log

Square root

Box-Cox

De-trending

Linear regression trend removal

Moving average detrending

Seasonal adjustment

Stationarity validated again using ADF & KPSS tests.

🔮 Time Series Forecasting Models
Univariate Models

AR (AutoRegressive)

MA (Moving Average)

ARMA

ARIMA

SARIMA

Each model includes:

Train-test split

Forecast visualization

RMSE calculation

🔁 Multivariate Time Series Models
Granger Causality Test

Examines whether TSLA prices help predict AAPL prices

Vector Models

VAR (Vector AutoRegression)

VMA (Vector Moving Average / VARMAX)

Used for:

Joint modeling of AAPL & TSLA stock prices

Forecasting Tesla prices using multivariate dependencies

📏 Model Evaluation Metrics

Implemented metrics include:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Mean Absolute Percentage Error (MAPE)

Akaike Information Criterion (AIC)

Bayesian Information Criterion (BIC)

🧹 Handling Missing Values in Time Series
Techniques Used

Imputation

Mean

Median

Mode

Forward fill

Backward fill

Interpolation

Linear

Polynomial

Spline

Predictive Modeling

Linear Regression to estimate missing values based on correlated features
