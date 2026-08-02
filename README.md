# Macroeconomic Indicators and the FTSE 100

Code from my MSc dissertation at the University of Greenwich: analysing how macroeconomic indicators affect the FTSE 100, and comparing classical time-series models with an LSTM for forecasting.

The core question: when interest rates, inflation, GDP growth, the GBP/USD rate or market volatility move, what happens to the index — and which modelling approach captures it better?

## Data

Monthly series, 2007–2024:

- FTSE 100 closing prices (Yahoo Finance)
- Bank Rate (Bank of England)
- CPIH inflation and GDP growth (UK government data)
- GBP/USD exchange rate
- VIX index

## Method

1. Preprocessing — interpolation for missing values, log transformation, differencing to reach stationarity (checked with the ADF test).
2. Exploratory analysis — series plots, correlation heatmaps.
3. Granger causality tests to identify which indicators lead the index.
4. VAR model with lag order selected by AIC/BIC; impulse response functions to trace how shocks in one variable ripple through the others.
5. Forecast comparison against an LSTM baseline.

## Stack

Python — pandas, numpy, yfinance, statsmodels, scipy, scikit-learn, matplotlib, seaborn.
