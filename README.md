# portfolio-risk-assessment
Monte Carlo Portfolio Risk Analysis 


***

# Portfolio Risk Assessment with Monte Carlo Simulation

**Author:** Muhsin KP
**Date:** November 2025

***

## Overview

This project analyzes and quantifies the risk characteristics of a multi-asset investment portfolio (AAPL, MSFT, SPY, TLT, VNQ) using real financial market data from [Yahoo Finance]. The workflow covers data extraction, cleaning, exploratory analysis, and Monte Carlo risk simulation. All code and data steps are fully reproducible for further learning and extension.

***

## Project Structure

- **data/raw/** — Original CSV files downloaded for each asset
- **data/processed/** — Cleaned and transformed close price and return DataFrames
- **notebooks/** — Step-by-step Jupyter notebooks for each stage:
    - `01_extracting_data.ipynb` — Download and save raw asset data
    - `02_cleaning_data.ipynb` — Clean and format data for analysis
    - `03_EDA.ipynb` — Exploratory Data Analysis: summary statistics, visuals, outlier review
    - `04_monte_carlo_simulation.ipynb` — Portfolio risk simulation, VaR/CVaR, distribution plots

***

## Key Steps and Methods

1. **Data Acquisition & Cleaning:**
    - Pulled historical prices for each asset.
    - Cleaned for consistent dates and selected only closing prices.

2. **Exploratory Data Analysis:**
    - Calculated basic statistics and visualized price/return trends.
    - Investigated return outliers, asset correlations, and volatility.

3. **Monte Carlo Simulation:**
    - Simulated thousands of future portfolio scenarios using historical mean/covariance.
    - Estimated Value at Risk (VaR), Conditional VaR (CVaR), and portfolio volatility.
    - Visualized return distributions and downside risk.

***

## How to Run

1. Clone or download this repository.
2. Open each notebook in sequence, or run the entire workflow in VS Code/Jupyter.
3. Change `data/raw/` source files or assets for further experiments or extension.

***

## Main Findings

- Portfolio risk is driven by asset correlations and extreme stock moves (outliers).
- Value at Risk (VaR) and CVaR highlight possible worst-case losses over a 1-month horizon.
- Diversification reduces most risks, but tail events and volatility remain key drivers.

***

## Possible Extensions

- Test different asset weights or additional securities.
- Add stress scenario analysis or rolling risk.
- Build an interactive dashboard with Streamlit/Plotly.

***

## License

This project is open for educational and research use. Please credit original data sources (Yahoo Finance).

***


