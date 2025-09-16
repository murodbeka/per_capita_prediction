# 🇨🇦 Forecasting Canada's Per Capita Income (2024–2028)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains a complete time series forecasting project to predict **Canada’s per capita income from 2024 to 2028** using historical data (1970–2016). We apply **linear regression**, **autoregressive (AR)**, and **ARIMA models** to generate statistically sound forecasts with confidence intervals.

> 🔮 *Prediction is very difficult, especially about the future.* – Niels Bohr

---

## 📌 Overview

Accurate economic forecasting helps governments, businesses, and individuals make informed decisions. In this project, we:
- Explore Canada’s income trends over 50+ years
- Model growth using statistical time series methods
- Forecast the next 5 years with uncertainty bounds
- Evaluate model assumptions and residuals

All models are implemented in Python using `pandas`, `statsmodels`, and `matplotlib`.

---

## 📂 Files

- `per_capita_income.ipynb` – Jupyter notebook with full analysis
- `canada_per_capita_income.csv` – Historical dataset (1970–2016)
- `README.md` – This file

---

## 🔍 Key Steps Covered

### 1. Exploratory Data Analysis (EDA)
- Line plot of income over time
- Scatter plot with linear fit
- Log returns and volatility analysis

### 2. Trend Modeling
- Simple linear regression: `Income ~ Year`
- Forecast extension (2024–2028)

### 3. Time Series Modeling
- Stationarity test (ADF)
- ACF/PACF analysis
- AR(1) model on differenced log-income
- ARIMA(1,1,1) model

### 4. Forecasting
- Generate point forecasts for 2024–2028
- Calculate 95% confidence intervals
- Visualize predictions with historical context

### 5. Diagnostics
- Residual analysis
- Q-Q plot for normality
- ACF of residuals

---

## 📊 Results Summary

| Model | 2024 Forecast | 2028 Forecast | Notes |
|------|---------------|---------------|-------|
| Linear Regression | ~$52,000 | ~$58,000 | Assumes constant linear growth |
| ARIMA(1,1,1) | ~$51,500 | ~$57,200 | Accounts for volatility and mean reversion |

> 💡 **Key Insight**: Growth has slowed in recent decades. Forecasts suggest continued moderate growth (~2–3% annually), with increasing uncertainty over time.
