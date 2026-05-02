# efficient-frontier-optimization
Portfolio optimization using Modern Portfolio Theory (MPT) and Monte Carlo simulations in Python.
# Efficient Frontier & Portfolio Optimization

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Quant](https://img.shields.io/badge/Focus-Quantitative%20Finance-gold.svg)

## 📌 Project Overview
This project focuses on the implementation of **Modern Portfolio Theory (MPT)** to construct optimal asset allocations. It automates the process of fetching historical market data, calculating risk-return profiles, and solving for the **Efficient Frontier** using quadratic optimization.

The tool allows users to identify the **Maximum Sharpe Ratio (MSR)** portfolio and the **Global Minimum Variance (GMV)** portfolio, providing a mathematical foundation for asset selection and risk management.

## 🛠️ Core Features
*   **Automated Data Ingestion:** Integrated with `yfinance` to pull real-time historical data for any list of tickers.
*   **Monte Carlo Simulation:** Simulates 10,000+ portfolio iterations to visualize the risk-return scatter plot.
*   **Numerical Optimization:** Uses `SciPy.optimize` to find the exact tangency portfolio on the Capital Market Line.
*   **Interactive Visualizations:** Built-in support for `Plotly` to generate interactive Efficient Frontier charts.

## 📁 Repository Structure
```text
efficient-frontier-optimization/
├── notebooks/
│   └── portfolio_optimization_research.ipynb  # Step-by-step math and EDA
├── src/
│   ├── data_engine.py          # Clean modular code for data fetching
│   ├── optimization_engine.py  # MPT and Sharpe Ratio logic
│   └── plotting_utils.py       # Reusable visualization functions
├── tests/
│   └── test_math_logic.py      # Unit tests for weight constraints
├── requirements.txt            # Project dependencies
└── README.md                   # Project documentation
