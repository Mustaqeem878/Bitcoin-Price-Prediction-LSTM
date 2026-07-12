# 📈 Bitcoin Price Prediction Using LSTM

A deep learning project that predicts the next **30 days of Bitcoin closing prices** using an **LSTM (Long Short-Term Memory)** neural network trained on historical daily Bitcoin market data.

This project demonstrates the complete machine learning workflow, including data preprocessing, feature engineering, model training, evaluation, and prediction.

---

## 🚀 Project Overview

The objective of this project is to forecast future Bitcoin prices by learning patterns from historical market data.

The model uses:

- Historical OHLCV (Open, High, Low, Close, Volume) data
- Technical indicators
- LSTM Neural Network
- Multi-step forecasting (Next 30 Days)

---

## 📊 Dataset

- **Source:** Binance Historical Bitcoin Dataset
- **Timeframe:** Daily (1D)
- **Period:** 2018 – 2025
- **Rows:** ~3,000

---

## 🧠 Features Used

### Market Data

- Open
- High
- Low
- Close
- Volume
- Quote Asset Volume
- Number of Trades
- Taker Buy Base Asset Volume
- Taker Buy Quote Asset Volume

### Technical Indicators

- 7-Day Moving Average (MA7)
- 30-Day Moving Average (MA30)
- 20-Day Exponential Moving Average (EMA20)
- 50-Day Exponential Moving Average (EMA50)
- Relative Strength Index (RSI)
- MACD
- MACD Signal
- MACD Histogram
- Bollinger Bands
- Average True Range (ATR)
- Daily Return
- Rolling Volatility

---

## 🏗️ Model Architecture

```
Input (90 Days × 23 Features)
            │
            ▼
      LSTM (128)
            │
         Dropout
            │
            ▼
       LSTM (64)
            │
         Dropout
            │
            ▼
      Dense (32)
            │
            ▼
Output (Next 30 Closing Prices)
```

---

## ⚙️ Technologies Used

- Python
- TensorFlow / Keras
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- TA (Technical Analysis Library)

---

## 📈 Model Performance

| Metric | Score |
|---------|-------|
| MAE | 7281 |
| RMSE | 9317 |
| MAPE | 7.87% |

> These results were obtained using only historical daily market data and technical indicators.

---

## 📜 Disclaimer

This project is intended for educational and research purposes only.

It is **not financial advice** and should not be used as the sole basis for investment decisions.
