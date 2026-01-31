# A-model-to-predict-stock-market-performance-using-LSTM

---

# Stock Market Prediction using LSTM

This project demonstrates predicting stock market prices using a Long Short-Term Memory (LSTM) neural network in Python. I am useing Apple Inc. (AAPL) stock data fetched from Tiingo API and trained an LSTM model to predict future stock prices. I have used this stock as a proxy to prediction stock market

---

# Table of Contents

* Project Overview
* Technologies
* Data
* Project Structure
* Usage
* Results

---

# Project Overview

* Stock prices are time-series data, where each price depends on previous prices.
* LSTM is a type of Recurrent Neural Network (RNN) that is ideal for time-series prediction.
* This project:
  * Fetches historical stock data for AAPL using Tiingo API
  * Preprocesses the data (scaling and shaping for LSTM)
  * Builds a **stacked LSTM model**
  * Predicts future stock prices and evaluates performance with **RMSE**
  * Visualizes both historical and predicted prices

---

# Technologies

* Jupyter notebook
* Python 3.x
* Libraries:
  * `pandas` – for data manipulation
  * `numpy` – for numerical operations
  * `matplotlib` – for plotting graphs
  * `scikit-learn` – for data preprocessing and RMSE calculation
  * `tensorflow` / `keras` – to build the LSTM model
  * `pandas_datareader` – to fetch stock data from Tiingo

---

# Data

* Source: Tiingo API
* Stock: Apple Inc. (AAPL)
* Columns in dataset:
  * `date` – trading date
  * `open`, `high`, `low`, `close` – stock prices
  * `volume` – number of shares traded
* Usage in project: I have used only the `close` column** for predictions.

---

# Project Structure

```
Stock-Market-LSTM/
│
├── README.md                # Project description
└── model.ipynb              # Main Jupyter Notebook
```

---

# Usage

1. Open `model.ipynb` in Jupyter Notebook or VS Code
2. Run cells in order:
   * Fetch data
   * Preprocess data
   * Train the LSTM model
   * Predict and visualize future stock prices
3. You will see:
   * Training and testing RMSE
   * Graphs of actual vs predicted prices
   * Future 30-day price predictions

---

# Results

* The model predicts the next 30 days stock price based on the last 100 days of historical data.
* Graphs generated:
  * Historical vs Predicted prices
  * Future 30-day forecast
* RMSE indicates prediction accuracy:
  * Training RMSE: 90.3%
  * Testing RMSE:  86.1%

---
