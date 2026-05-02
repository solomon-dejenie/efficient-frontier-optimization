
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

 Mathematical FoundationThe optimization engine solves for weights ($w$) that minimize portfolio variance ($\sigma_p^2$) for a target return ($E[R_p]$):$$ \min \sigma_p^2 = w^T \Sigma w $$Subject to:$\sum w_i = 1$ (Full investment)$w_i \ge 0$ (No short-selling constraint)$w^T \mu = E[R_p]$ (Target return constraint)🚀 How to RunClone the Repo:Bashgit clone [https://github.com/your-username/efficient-frontier-optimization.git](https://github.com/your-username/efficient-frontier-optimization.git)
Install Requirements:Bashpip install -r requirements.txt
Execute Analysis:Open notebooks/portfolio_optimization_research.ipynb in your preferred editor to view the full analysis.📈 Key InsightsDemonstrated how diversification shifts the frontier to the left, reducing idiosyncratic risk.Identified the "Tangency Portfolio" which provides the highest return per unit of risk based on current risk-free rates.Contact: [Your Name] - [Your LinkedIn Link]
---

### Why this works:
1.  **Badges:** The blue and gold badges at the top make the project look like a professional library.
2.  **Visual Hierarchy:** Recruiters can scan the "Core Features" in 5 seconds to see your tech stack.
3.  **LaTeX Equations:** Including the optimization formula proves you actually understand the math behind the code, which is a huge green flag for FinTech roles.
4.  **Modular Folder Structure:** Mentioning the `src/` and `tests/` folders shows you have "Clean Code" habits, not just "Notebook habits."

**Ready for Project 2 (Financial Asset Return Analys
