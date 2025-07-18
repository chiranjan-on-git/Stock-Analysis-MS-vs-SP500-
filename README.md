# Stock Market Risk Analysis - Morgan Stanley

<img width="1092" height="577" alt="Screenshot 2025-07-18 174632" src="https://github.com/user-attachments/assets/ae394193-1072-4e9a-83d5-eb3b99fb6bb7" />

## Overview
This project performs a comprehensive risk analysis of **Morgan Stanley's (MS) stock performance** from **June 1, 2023, to January 1, 2024**, comparing it with the **S&P 500 index (^GSPC)**. The analysis uses historical stock data to compute various risk and return metrics.

## Key Features
-   **Historical Data Fetching**: Retrieves daily stock prices for MS and ^GSPC using `yfinance` for a specified period.
-   **Daily Returns Calculation**: Computes the daily percentage change in close prices for both assets.
-   **Rolling Volatility**: Calculates the 30-day rolling standard deviation of daily returns for both MS and S&P 500 to track changing risk levels.
-   **Value at Risk (VaR)**: Estimates the potential maximum loss for Morgan Stanley's stock at a 95% confidence level using the normal distribution method.
-   **Sharpe Ratio**: Measures the risk-adjusted return by comparing the mean daily return to the standard deviation of returns for both MS and S&P 500.
-   **Beta Calculation**: Determines Morgan Stanley's systematic risk (sensitivity to market movements) relative to the S&P 500.
-   **Correlation Analysis**: Quantifies the linear relationship strength between MS and S&P 500 daily returns.
-   **Risk Visualization**: Generates informative plots, including rolling volatility trends and a scatter plot illustrating the stock-market relationship.

## Technologies Used
-   Python
-   Pandas, NumPy (for data manipulation and numerical operations)
-   Matplotlib, Seaborn (for data visualization)
-   yFinance (for fetching financial data)
-   SciPy (for statistical analysis, e.g., normal distribution for VaR)

## Key Insights
Based on the analysis of data from June 1, 2023, to January 1, 2024:
-   **Correlation with S&P 500**: MS stock has a **correlation of approximately 0.57** with the S&P 500. This indicates a moderate positive relationship, meaning MS generally moves in the same direction as the market, but not perfectly in sync.
-   **95% Value at Risk (VaR)**: The 95% **VaR for Morgan Stanley is -2.53%**. This means there is a 5% probability that Morgan Stanley's stock could experience a daily loss of 2.53% or more.
-   **Beta**: Morgan Stanley's **Beta is approximately 1.27**. Since Beta is greater than 1, it suggests that MS stock tends to be **more volatile** and sensitive to overall market movements than the S&P 500.
-   **Sharpe Ratio**: The Sharpe Ratio for Morgan Stanley is **0.07**, while for the S&P 500 it is **0.12**. This indicates that, during the analyzed period, the **S&P 500 offered a better risk-adjusted return** compared to Morgan Stanley's stock.
-   **Rolling Volatility**: The rolling volatility plot clearly shows that Morgan Stanley's stock volatility trends closely follow that of the S&P 500, with both exhibiting higher fluctuations in certain months within the analyzed period.

## How to Run
To run this analysis on your local machine:

1.  **Ensure you have Python installed.**
2.  **Clone this repository** (if applicable) or download the files.
3.  **Navigate to the project directory** in your terminal or command prompt.
4.  **Install the required dependencies** using `pip`:
    ```bash
    pip install -r requirements.txt
    ```
5.  **Run the analysis**: Open the `main.ipynb` notebook in a Jupyter environment (e.g., Jupyter Notebook, JupyterLab, VS Code with Jupyter extension) and execute the cells sequentially from top to bottom.

---
