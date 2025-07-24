# Stock Price Prediction with XGBoost 📈

This project implements a machine learning pipeline to predict future stock prices using XGBoost regression. It includes feature engineering from technical indicators and time series cross-validation.

## 🔍 Features

- Technical indicator generation with `ta`
- Time series cross-validation with `TimeSeriesSplit`
- XGBoost regression model
- Evaluation using RMSE
- Cumulative return backtest

## 🛠️ Installation

```bash
pip install -r requirements.txt
```

## 🧪 Usage

All code is in `notebooks/StockPredictionwithXGboost_clean.ipynb`. You can run it cell-by-cell.

## 📁 Directory Structure

```
notebooks/              # Contains the Jupyter Notebook
data/                   # (Optional) Raw or processed stock data
outputs/                # (Optional) Figures or saved models
```

## 📌 To-Do

- Add LSTM or other model comparisons
- Use more advanced factor engineering (e.g. industry-neutral factors)
- Add more evaluation metrics (Sharpe Ratio, Max Drawdown)

## 👤 Author

Jinghan He
