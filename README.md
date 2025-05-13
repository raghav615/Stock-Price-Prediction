# 📊 Bitcoin Market Behavior: Forecasts Across Timeframes

## 🧠 Project Overview

This project analyzes Bitcoin's historical price behavior and builds predictive models across **short-term (3 months)**, **mid-term (1 year)**, and **long-term (5 years)** timeframes using both statistical and machine learning techniques.

### 🎯 Goals:
- Forecast Bitcoin closing prices across different timeframes.
- Compare performance of **LSTM** vs **XGBoost**.
- Evaluate the effectiveness of moving averages in trend detection.

## 👨‍💻 Team Members
- Raghav Upadhyay  
- Umesh Kumar Siyak

## 📅 Date
April 15, 2025

---

## 📂 Data

- **Source**: [Yahoo Finance](https://finance.yahoo.com)
- **Frequency**: Daily historical data
- **Format**: CSV files (for each timeframe: 3M, 1Y, 5Y)

---

## 🛠 Tools & Technologies

- **Language**: Python  
- **Environment**: Jupyter Notebook

### 🧹 Data Collection & Processing:
- `yfinance`, `pandas`, `numpy`, `requests`

### 📈 Visualization:
- `matplotlib`, `matplotlib.ticker`

### 🔍 Modeling:
- **LSTM**: Built using `tensorflow.keras` with layers like `LSTM`, `Dense`, `Dropout`
- **XGBoost**: Used for regression with lag features

### 🧪 Preprocessing:
- `MinMaxScaler` from `sklearn.preprocessing` for scaling data

---

## 🔎 Research Questions

1. **How effective is the moving average in trend analysis?**  
   → Smoothing with 7-day and 45-day MAs provided strong visual insights for local trend detection and reversal spotting.

2. **LSTM vs XGBoost: Which is better?**  
   - **LSTM** performed better on **long-term trends** (5 years), capturing seasonality and cycles.  
   - **XGBoost** excelled in **short- and mid-term** forecasting, leveraging recent lag features effectively.

---

## 📊 Visuals & Architecture

- Bitcoin price trends plotted across 3 timeframes
- LSTM & XGBoost predictions overlaid on actual price
- Moving average overlays for volatility reduction
- Architecture diagram of the full pipeline

---

## 🧠 Key Learnings

- LSTM requires careful tuning and performs best for long-range trend forecasting
- XGBoost is more robust for near-term predictions but flattens for long-term data
- A **hybrid approach (LSTM + XGBoost)** may yield the most balanced results
- Visual inspection is crucial—statistical metrics don't always reflect visual performance

---

## 📁 File Structure

