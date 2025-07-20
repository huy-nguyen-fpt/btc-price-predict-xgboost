# Bitcoin Price Prediction using XGBoost (1-Hour Interval)
This project builds a time-series regression model to predict the **next-hour Bitcoin price** using historical market data and technical indicators.

## 📊 Data Sources
- **Binance API**: Historical OHLCV (Open, High, Low, Close, Volume) data for BTC/USDT at 1-hour intervals since February 2018.
- **Fear & Greed Index** from [alternative.me](https://alternative.me/): Market sentiment mapped to numerical scores (0–100).

## 🔧 Features
- Technical indicators: SMA (Simple Moving Average), EMA (Exponential Moving Average), RSI (Relative Strength Index), log(volume)
- Time-based features: Hour, Day of Week, Month, Quarter
- Lagged values: Close price at t-1, t-6, t-24

## 🧠 Model
- Algorithm: **XGBoost Regressor**
- Target: Predict next-hour `close` price
- Evaluation metric: RMSE (Root Mean Squared Error)

## 📈 Results
- The model captures short-term patterns using engineered features.
- Further improvements possible using deep learning models like LSTM or Transformer.

## 🚀 How to Run
Open the Colab notebook or clone the repo to run locally:
```bash
pip install pandas xgboost matplotlib scikit-learn
