# 🧠 RSI + Bollinger Bands Trading Strategy (Python)

## 📄 Overview
This project builds and backtests a quantitative trading strategy that combines **Relative Strength Index (RSI)** momentum and **Bollinger Band** volatility signals to identify high-confluence trade opportunities.  

The goal was to test whether using both indicators together could improve trading performance compared to the **SPY benchmark (S&P 500 ETF)** from 1993–2025.

---

## 🎯 Objectives
- Combine RSI and Bollinger Bands to form a **confluence-based trading system**
- Backtest performance over multiple decades of SPY price data  
- Compare cumulative returns to the SPY benchmark  
- Explore how **1.5× leverage** affects both risk and return  

---

## ⚙️ Features
- Fetches SPY data using the `yfinance` API  
- Computes RSI and Bollinger Bands using **Pandas** and **NumPy**  
- Generates buy/sell signals based on overbought/oversold and volatility thresholds  
- Implements leverage testing and cumulative return visualization  
- Visualizes results using **Matplotlib**

---

## 🧩 Strategy Logic
**RSI Rules:**
- RSI < 35 → potential **long**  
- RSI > 75 → potential **short**

**Bollinger Band Rules:**
- BB Length = 10
- BB Standard Deviations = 1
- Close < Lower Band → long bias  
- Close > Upper Band → short bias  

A trade is **confirmed** only when both signals agree.

---

## 📈 Results
- **Backtest Period:** 1993–2025  
- **Unleveraged Strategy:** ~8–9× growth  
- **SPY Benchmark:** ~25× growth  
- **Leveraged Strategy (1.5×):** matched SPY performance (~25×)  
- **Key Insight:** leverage amplifies returns **and** risk (margin calls, liquidation potential)

---

## 🧰 Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **yfinance**

---

## 🧠 Lessons Learned
- Combining simple indicators like RSI and Bollinger Bands can provide meaningful insights when tested rigorously.
- Leverage enhances returns but significantly increases risk exposure.
- Python makes it possible to move from *intuition* to *data-driven validation* through backtesting.

---

## 🚀 Future Improvements
- Add stop-loss and take-profit logic  
- Optimize parameters (RSI length, BB deviations)  
- Incorporate portfolio allocation and transaction costs  
- Compare to more complex models (e.g., MACD, SMA crossover)

---

## 📎 Author
**Nathan Chelladurai**  
📍 Toronto Metropolitan University – Economics & Management Science  
💼 Interested in Finance · Data Analytics · Quantitative Research  
📫 Connect on [LinkedIn] (https://www.linkedin.com/in/nathan-chelladurai-779406221/)
