# Crypto Trade Prediction

This analysis aims to investigate whether it is possible to predict the direction of the next trade as `Buy` or `Sell` by applying machine learning techniques on historical cryptocurrency trading data. The study focuses on engineered features derived from two datasets: `fills_data`, which records the details of executed trades, including trade price, quantity, and side (Buy/Sell), and `market_data`, which provides bid and ask prices over time, offering insight into the market conditions surrounding each trade. The engineered features are used to train a Gradient Boosting model, and the results are evaluated.

The results demonstrate that trade direction is moderately predictable using well-engineered features. Among the most predictive signals are:

- Changes in deviation from mean inventory (`dev_from_mean_balance_lag1_diff`)
- Market price movement relative to its long-term mean
- Lagged trade profitability and volatility
