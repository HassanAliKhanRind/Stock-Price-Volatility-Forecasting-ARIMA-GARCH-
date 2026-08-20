# Stock Price Volatility Forecasting (ARIMA-GARCH)

Advanced time-series forecasting to predict mean returns (ARIMA) and volatility/risk (GARCH).

Overview

This project combines two complementary time-series models:

ARIMA (AutoRegressive Integrated Moving Average) — models and forecasts the mean/expected return of a stock's price series
GARCH (Generalized Autoregressive Conditional Heteroskedasticity) — models and forecasts the volatility of returns, capturing volatility clustering (periods of high volatility followed by more high volatility)

Together, ARIMA-GARCH gives both a return forecast and a risk (volatility) forecast, which plain ARIMA alone cannot capture.

Tools Used
Python
statsmodels (ARIMA)
arch (GARCH)
Pandas, Matplotlib
Jupyter Notebook

How to Run

Open the notebook in Jupyter and run all cells. Replace the stock ticker/price series with any asset you want to forecast.

Why This Matters

Volatility forecasting is central to options pricing, risk management (VaR), and portfolio construction — GARCH models are the industry standard for capturing time-varying volatility in financial returns.
