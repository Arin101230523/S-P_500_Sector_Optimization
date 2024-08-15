# S&P 500 Portfolio Optimization

## Overview

This project performs portfolio optimization using historical data of S&P 500 companies. The goal is to create an optimized portfolio that maximizes the Sharpe ratio while minimizing volatility. The optimization process involves:

1. Fetching historical price data for S&P 500 companies.
2. Calculating sector-wise average closing prices.
3. Generating random portfolios and calculating their metrics.
4. Running Monte Carlo simulations to evaluate potential portfolios.
5. Applying Random Forest Regression for further portfolio optimization.

## Prerequisites

Ensure you have the following libraries installed:
- `openpyxl`
- `pandas`
- `yfinance`
- `matplotlib`
- `scipy`
- `scikit-learn`
- `PyPortfolioOpt`
- `cvxpy`

You can install these libraries using pip:

`bash
pip install openpyxl pandas yfinance matplotlib scipy scikit-learn PyPortfolioOpt cvxpy`


## Instructions

1. **Setup and Data Fetching:**

   - Fetch the list of S&P 500 companies and their sectors from Wikipedia.
   - Replace ticker symbols for consistency and handle missing data.
   - Fetch historical adjusted closing prices for each sector.

2. **Data Processing:**

   - Calculate the average closing prices for each sector.
   - Compute the logarithmic returns and remove negative returns.
   - Generate random portfolio weights and normalize them.

3. **Optimization Metrics:**

   - Calculate expected returns, volatility, and Sharpe ratio for the portfolios.
   - Save the results to Excel files for further analysis.

4. **Monte Carlo Simulation:**

   - Run simulations to generate various portfolios and their metrics.
   - Analyze the results to identify the portfolio with the maximum Sharpe ratio and minimum volatility.

5. **Machine Learning Enhancement:**

   - Use Random Forest Regression to predict portfolio weights based on portfolio metrics.
   - Evaluate the model performance using Mean Squared Error.



The code is organized into sections as follows:

1. **Library Installation** - Install necessary libraries.
2. **Data Fetching** - Retrieve and preprocess data from the web.
3. **Data Processing** - Calculate averages and log returns.
4. **Optimization Metrics** - Compute portfolio metrics.
5. **Monte Carlo Simulation** - Simulate and analyze portfolios.
6. **Machine Learning** - Train and evaluate a Random Forest model for portfolio weight prediction.


## Results

The final output includes:
- Portfolio weights with the highest Sharpe ratio.
- Portfolio weights with the lowest volatility.
- Predicted weights from the Random Forest model.

