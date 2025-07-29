# Retail Company Financial Analysis

## Project Goal

The goal of this project is to evaluate and compare the financial performance of three major companies in the retail sector — **Walmart**, **Target**, and **Costco**.

## Methodology

Financial data was extracted using the **`yfinance` Python library**, which pulls stock and financial statement data directly from Yahoo Finance.

From the raw data, I calculated the following financial ratios for each company:

- **Return on Investment (ROI)**
- **Gross Margin**
- **Return on Sales (ROS)**
- **Current Ratio**
- **Quick Ratio**
- **Asset Turnover**
- **Debt-to-Equity Ratio**

Each of these metrics represents a different aspect of a company's financial health — such as profitability, liquidity, efficiency, and leverage.

To make a meaningful comparison, I developed a **custom scoring model**, assigning specific weights to each ratio based on its importance in retail industry analysis. The final score for each company ranges from **0 to 100**.

## Outcome

The scores help benchmark each company’s overall financial position, making it easier to identify which one may be in the strongest condition based on financial fundamentals.
