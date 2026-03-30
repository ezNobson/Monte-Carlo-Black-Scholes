# Monte Carlo Option Pricing (Black-Scholes)

A simple Python implementation of the Monte Carlo method to price European Call options using real-market data.

## 📊 How it works
1. Fetches historical stock data (NVDA) via `yfinance`.
2. Calculates annual volatility ($\sigma$) from log returns.
3. Simulates 100,000 price paths using **Geometric Brownian Motion**.
4. Validates the result against the analytical **Black-Scholes** formula.

## 🚀 How to run
1. Open the `.ipynb` file in **Google Colab**.
2. Run all cells to see the pricing results and the "Fan Chart" visualization.

## 👤 Author
**Michał Dyrek** Data Engineering & Analysis student @ AGH University of Krakow
