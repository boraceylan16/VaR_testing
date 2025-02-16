# 🚀 Value-at-Risk (VaR) Analysis of Crude Oil Prices Using Python

## 📌 Overview
This project focuses on **Value-at-Risk (VaR)** analysis of crude oil futures (**CL=F**) using Python. It fetches real-time market data via `yfinance`, computes daily returns, and applies different VaR estimation techniques to assess market risk.

## 🛠️ Key Features

### 📈 Financial Data Retrieval
- Uses `yfinance` to obtain crude oil futures data.
- Extracts key financial metrics (bid/ask price, daily high/low, 52-week range, and opening price).

### 🔍 Data Preprocessing & Analysis
- Computes daily percentage changes in crude oil prices.
- Cleans the data by handling missing values.

### 📉 Value-at-Risk (VaR) Calculation
- **Historical VaR:** Uses past return distributions to estimate risk.
- **Parametric VaR (Variance-Covariance Method):** Assumes normal distribution and calculates risk using mean and standard deviation.
- **Monte Carlo Simulation:** Generates random returns based on observed data to estimate risk exposure.

### 📊 Visualization
- Plots the probability density of daily returns using `seaborn`.
- Displays VaR thresholds to indicate potential losses at a given confidence level.

## 📷 Sample Code for VaR Calculation
```python
var_95 = np.percentile(gold_data_daily_returns, 5)  # 95% Confidence Interval
print(f"95% VaR: {var_95:.4f}")
```

## 📌 Why This Matters?
VaR is a crucial risk management tool used by financial institutions and traders to quantify potential losses. This project provides a comprehensive approach to risk assessment using multiple VaR techniques.





