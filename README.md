# Stock Price Forecasting on Indonesian IDX30

## Overview
A comparative data mining framework for predicting the next-day closing prices of highly liquid Indonesian stocks (IDX30). The project evaluates five different model families to analyze the trade-offs between predictive accuracy and model interpretability.

## Models Evaluated
- **Statistical**: SARIMAX (Linear patterns and autocorrelation).
- **Machine Learning**: XGBoost and LightGBM (Nonlinear tabular data and ensemble learning).
- **Deep Learning**: LSTM (Temporal dependencies and sequence learning).
- **Hybrid**: NeuralProphet (Combines deep learning with interpretable trend/seasonality components).

## Methodology
- **Data Source**: Historical OHLCV (Open, High, Low, Close, Volume) daily stock data for IDX30 equities.
- **Preprocessing**: Chronological sorting, numeric conversion, and MinMax scaling (for LSTM).
- **Evaluation Metrics**: Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE).

## Results
- **Best Performer**: **NeuralProphet** achieved the most reliable performance with the lowest error scores (RMSE: 244.73, MAE: 187.32).
- **Machine Learning**: XGBoost also showed high accuracy, significantly outperforming traditional statistical models like SARIMAX.
- **Deep Learning**: LSTM captured long-term dependencies effectively but acted as a "black box" regarding transparency.
