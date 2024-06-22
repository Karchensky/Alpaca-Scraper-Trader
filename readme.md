# Alpaca Trading Analysis and Prediction

## Overview

This project focuses on predicting stock movement (up or down by a target threshold percentage) using data scraped from the Alpaca API. The core of this project is encapsulated in the `alpaca.ipynb` notebook, which contains various modeling techniques and data transformations aimed at achieving this goal. The notebook leverages volume/trading data to create technical indicators, which serve as the foundation for predicting stock movement directions.

## Data Collection

Data is scraped from the Alpaca API and stored locally in a SQLite Database. The [`AlpacaDataScraper`](alpaca_algo_trading/alpaca.ipynb) class within the notebook is responsible for this process. It requires an `alpaca_keys.txt` file for API authentication and interacts with the Alpaca API to fetch stock data.

## Technical Indicators

The notebook employs a wide range of technical indicators as features for the models. These include, but are not limited to:

- Relative Strength Index (RSI)
- Moving Average Convergence Divergence (MACD)
- Commodity Channel Index (CCI)
- Average Directional Index (ADX)
- Bollinger Bands
- Ichimoku Clouds
- +++

These indicators are calculated for various lag periods, providing a comprehensive dataset for analysis.

## Modeling Techniques

Several modeling techniques are explored in the notebook to predict stock movements. These include:

- K-Nearest Neighbors
- Gradient Boosting
- Logistic Regression
- LSTM (Long Short-Term Memory networks)
- CNN (Convolutional Neural Networks)
- RNN (Recurrent Neural Network)
- XGBoost
- Random Forest
- Neural Network
- Support Vector Machine

Each model is trained and evaluated on the dataset, with parameters and model types defined within the notebook. The models are stored as `.keras` or `.pkl` files for future use.

## Prediction and Trading Bot (Future Work)

The ultimate goal of this project is not only to predict stock movements accurately but also to develop a trading bot that uses these predictions to make trades via the Alpaca API. This is planned if we ever get a good enough model and have completed sufficient backtesting & testing.

## Getting Started

To use this notebook:

1. Ensure you have an `alpaca_keys.txt` file with your Alpaca API key and secret.
2. Install the necessary Python packages, including `alpaca-trade-api`, `joblib`, and machine learning libraries such as `scikit-learn` and `tensorflow`.
3. Run the `alpaca.ipynb` notebook, adjusting parameters and models as needed for your analysis.
4. ???
5. Profit
