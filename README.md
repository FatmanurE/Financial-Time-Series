# Time Series Analysis of Macroeconomic Indicators on London Stock Exchange (FTSE 100)
This project analyzes the impact of macroeconomic indicators on the FTSE 100 Index using time series modeling techniques, specifically Vector Autoregression (VAR). The project focuses on exploring relationships between interest rates, inflation, GDP, exchange rates, and market volatility.

📌 Project Overview
Objective: To forecast FTSE 100 movements and understand how macroeconomic variables influence stock market trends.

Data Sources:
-Yahoo Finance: FTSE 100 closing prices.
-Bank of England: Bank Rate (interest rates).
-UK Government Economic Data: CPIH Rate (inflation), GDP Growth Rate.
-GBP/USD Exchange Rate: Obtained from financial data providers.
-VIX Index: Market volatility data.
-Time Frame: 2007 - 2024
-Models Used: VAR, ADF Test, Granger Causality, Impulse Response Function (IRF)

🛠️ Technologies & Libraries
This project is implemented in Python and uses the following libraries:

📊 Data Processing: pandas, numpy, yfinance

📈 Time Series Analysis: statsmodels, scipy, matplotlib, seaborn

📉 Machine Learning: sklearn.preprocessing, sklearn.metrics

📂 Dataset & Preprocessing
Economic Indicators:

--Bank Rate (Bank of England)
--CPIH Rate (Inflation Data)
--GDP Growth Rate
--GBP/USD Exchange Rate
--FTSE 100 Closing Prices
--VIX Index (Market Volatility)

--Preprocessing:
Handling missing values via interpolation
Transforming non-stationary series via ADF test & differencing
Log transformation to stabilize variance

🔬 Methodology
Data Cleaning & Transformation
Convert time series to monthly frequency
Log transformation & differencing to ensure stationarity
Exploratory Data Analysis
Time series visualization
Correlation heatmaps & pairplots
Statistical Tests
Augmented Dickey-Fuller (ADF): Check stationarity
Granger Causality Test: Identify causal relationships
Model Training & Forecasting
Vector Autoregression (VAR) Model
Optimal lag selection via AIC/BIC criteria
Impulse Response Functions (IRF) to analyze variable impact

--Evaluation & Results
Forecasting FTSE 100 price movements
Analyzing economic shock responses
