# ESG-Constrained-Portfolio-Optimization

This project explores the creation of optimized portfolios under varying environmental, social, and governance (ESG) constraints. By integrating historical financial data, advanced risk models, and visualizations, this project demonstrates a comparison of portfolio performance across three scenarios:

- No ESG Constraints
- Mild ESG Constraints (e.g., minimum ESG score ≥ 0.6)
- Aggressive ESG Constraints (e.g., minimum ESG score ≥ 0.8)

The goal is to analyze how ESG constraints impact portfolio performance metrics such as Expected Return, Volatility, and Sharpe Ratio.


**Libraries:**
- pandas: Data manipulation and analysis
- numpy: Numerical computing
- yfinance: To fetch historical financial data
- matplotlib: For data visualization
- seaborn: Advanced visualizations
- pypfopt: Portfolio optimization and financial modeling

**Key Functionalities:**

_1. Data Fetching and Processing_
- Market Data: Historical price data is fetched using yfinance for a universe of tickers.
- Market Cap Selection: The top 10 stocks by market capitalization are dynamically selected for analysis.
- Data Cleaning: Missing values are handled using forward fill and interpolation to ensure a continuous price series.

_2. Portfolio Optimization_
- Risk Models: Both sample covariance and Ledoit-Wolf shrinkage models are computed to estimate the covariance matrix.
- Expected Returns: CAPM (Capital Asset Pricing Model) is used to estimate returns for the tickers.

_3. Performance Comparison and Visualization_
- Historical Prices: Line charts to illustrate price trends over the past 5 years.
- Bar Chart: Visualizes performance metrics (Expected Return, Volatility, Sharpe Ratio) across the three scenarios.
- Heatmap: Displays portfolio performance (in percentages) across metrics and scenarios for a condensed view.
- Covariance/Correlation Matrix: Highlights relationships and dependencies among the selected stocks.


