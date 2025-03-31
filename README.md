# Gold Price Forecasting Using XGBoost and LSTM

![screenshot-localhost_8888-2025 03 31-13_14_37](https://github.com/user-attachments/assets/88983030-1bc3-476b-bd8a-6d0aa2ed8dda)

### Project Overview

This project aims to predict gold prices using machine learning models. Two models were implemented:

- XGBoost – A powerful tree-based ensemble learning algorithm.
- LSTM (Long Short-Term Memory) – A deep learning model designed for sequential data.

The models were trained on historical gold price data with various technical indicators (e.g., moving averages, volatility, and price lags) to improve forecasting accuracy.

### Dataset

The dataset used in this project consists of historical daily gold prices, along with calculated features such as:

- Moving averages (7-day, 30-day, 90-day)
- Volatility (7-day, 30-day, 90-day)
- Lagged price values (lag-1, lag-2, lag-3, lag-5, lag-7)
- Daily returns and log returns

### Model Training & Evaluation

1. Feature Engineering
- Moving averages and volatility indicators were calculated.
- Lagged price features were added to capture historical trends.
- Data was scaled using MinMaxScaler for better model performance.

2. Train-Test Split
- The dataset was split into 80% training and 20% testing.
- Features and target values were separately scaled.

### Model Performance Metrics

- LSTM outperformed XGBoost in RMSE but had a higher MAE, indicating better trend prediction but slightly worse absolute error performance.

- Both models captured trends in gold prices, but further improvements can be made through hyperparameter tuning and feature engineering.

### Results & Visualization

The model predictions were compared to actual gold prices using plots:

- XGBoost Predictions vs. Actual Prices
- LSTM Predictions vs. Actual Prices
- Model Error Distribution

### Future Improvements

1. Experiment with additional features like macroeconomic indicators.
2. Tune hyperparameters further using Bayesian optimization.
3. Implement alternative deep learning models such as Transformer-based architectures.

### Source

![Gold Price 1979 to Present from Kaggle](https://www.kaggle.com/datasets/jishnukoliyadan/gold-price-1979-present)
