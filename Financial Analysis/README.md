# Retail Company Financial Analysis

## Project Goal

The goal of this project is to analyze and compare the 2024 financial performance of three large retail companies — **Walmart**, **Target**, and **Costco**. These companies are key players in the retail industry, with the following approximate market capitalizations in 2024:

- **Walmart** – ~$782B  
- **Costco** – ~$413B  
- **Target** – ~$48.2B

## Methodology

I used the **`yfinance` Python library** to collect financial data directly from Yahoo Finance, including income statements, balance sheets, and cash flow reports.

Based on this data, I calculated the following financial ratios for each company:

- **Return on Investment (ROI)**
- **Gross Margin**
- **Return on Sales (ROS)**
- **Current Ratio**
- **Quick Ratio**
- **Asset Turnover**
- **Debt-to-Equity Ratio**

These ratios help to understand different parts of a company’s financial health: profitability, liquiidity, activity, solvency.

To compare the companies more clearly, I built a **simple scoring model**. Each metric was given a weight depending on how important it is when analyzing retail businesses. Then, each company got a final score from **0 to 100** based on how well they performed across all these ratios.

## Outcome





