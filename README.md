# Stock Price Prediction with XGBoost

## Overview
This project explores short-term stock return prediction using machine learning techniques. The goal is to evaluate whether engineered time-series features can provide predictive power for equity returns and be applied in a simple trading strategy.

## Methodology
- **Data**: Historical stock price and volume data  
- **Feature Engineering (Alpha Factors)**:  
  - Lagged returns  
  - Rolling volatility measures  
  - Momentum indicators (e.g., moving averages, Bollinger Bands)  
- **Model**: Gradient Boosted Regression Trees (XGBoost)  
  - Trained using expanding-window cross-validation to avoid look-ahead bias  
  - Objective: predict next-day stock returns  

## Trading Strategy and Backtesting
- Model outputs were converted into trading signals:  
  - Positive predicted return → long position  
  - Negative predicted return → short position  
- Backtested on historical data with evaluation metrics:  
  - **Cumulative return**  
  - **Maximum drawdown**  
  - **Sharpe ratio**  

## Results
- The model demonstrated predictive ability relative to naive benchmarks (e.g., buy-and-hold, simple moving average crossover).  
- Backtest results showed that engineered features provided meaningful signals for short-term return forecasting, with improved risk-adjusted performance compared to baseline strategies.  

## Future Work
- Incorporate transaction costs and slippage into the backtest framework  
- Extend feature set with macroeconomic and alternative data  
- Compare against traditional statistical methods (ARIMA, GARCH)  
