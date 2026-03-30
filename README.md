# Monte Carlo Option Pricing (Black-Scholes)

A simple Python implementation of the Monte Carlo method to price European Call options using real-market data.

## 📊 How it works
1. Fetches historical stock data (NVDA) via `yfinance`.
2. Calculates annual volatility ($\sigma$) from log returns.
3. Simulates 100,000 price paths using **Geometric Brownian Motion**.
4. Validates the result against the analytical **Black-Scholes** formula.

## 📉 Risk Assessment (6-Month Horizon)
The model extends beyond basic pricing to provide a comprehensive risk analysis using **Value at Risk (VaR)** and **Conditional Value at Risk (CVaR)**.

| Confidence Level ($\alpha$) | VaR (USD) | CVaR (USD) |
|:---:|:---:|:---:|
| 95% | 64.33 | 75.43 |
| 99% | 82.78 | 90.22 |

**Key Insight:** While VaR provides a loss threshold, CVaR quantifies the "Expected Shortfall" in the worst-case scenarios. The ~17% gap between VaR and CVaR at the 95% level indicates the presence of significant tail risk in NVDA's simulated distribution.

## 🚀 How to run
1. Open the `.ipynb` file in **Google Colab**.
2. Run all cells to see the pricing results and the "Fan Chart" visualization.

## 👤 Author
**Michał Dyrek** Data Engineering & Analysis student @ AGH University of Krakow
