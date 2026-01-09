# Stock-Price-Volatility-Forecasting-ARIMA-GARCH-

📌 Project Overview

This project applies time-series forecasting and volatility modeling to Apple Inc. (AAPL) stock data using a hybrid ARIMA–GARCH framework.

ARIMA is used to forecast future stock prices

GARCH is used to model and forecast time-varying volatility

Forecasts are evaluated using actual market data

Confidence intervals and error metrics are included

This project demonstrates quantitative finance, econometrics, and risk modeling skills.

🎯 Objectives

Forecast short-term stock prices using ARIMA

Model volatility clustering using GARCH

Generate confidence intervals around forecasts

Compare forecasts with actual realized prices

Evaluate volatility forecasts using Mean Squared Error (MSE)

🛠 Tech Stack

Python

NumPy

Pandas

yFinance

Matplotlib

Statsmodels (ARIMA)

ARCH package (GARCH)

Scikit-learn (Evaluation)

📊 Data Details

Asset: Apple Inc. (AAPL)

Data Source: Yahoo Finance

Price Type: Adjusted Close

Period Used: 2010 – 2024

Frequency: Daily (Trading Days)

📐 Modeling Approach
1️⃣ Data Preparation

Convert prices to log prices

Compute log returns

Remove missing values

Log transformation ensures stationarity and stability

2️⃣ ARIMA Model (Price Forecasting)

ARIMA models the conditional mean of log prices

Manual ARIMA(1,1,1) and auto-ARIMA selection used

Forecasts future log prices, converted back to real prices

ARIMA(p,d,q)

3️⃣ GARCH Model (Volatility Forecasting)

GARCH(1,1) models conditional variance

Captures volatility clustering common in financial returns

Forecasts 10-day ahead volatility

𝜎^2=ω+αϵt−12​+βσt−12​

4️⃣ ARIMA + GARCH Combined

ARIMA forecasts expected prices

GARCH forecasts volatility

Confidence intervals constructed using:


PRICE = ey^​t​±σt​​

