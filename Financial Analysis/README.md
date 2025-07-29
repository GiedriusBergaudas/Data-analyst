# Retail Company Financial Analysis

## Project Goal

This project aims to analyze and compare the 2024 financial performance of three major retail companies — **Walmart**, **Target**, and **Costco**. These are some of the biggest players in retail, with approximate market values as follows:

- **Walmart** – $782 billion  
- **Costco** – $413 billion  
- **Target** – $48.2 billion

## Methodology

I used the **`yfinance` Python library** to download financial data straight from Yahoo Finance. This included income statements, balance sheets, and cash flow reports.

From this data, I calculated key financial ratios for each company:

- **Return on Investment (ROI)**
- **Gross Margin**
- **Return on Sales (ROS)**
- **Current Ratio**
- **Quick Ratio**
- **Asset Turnover**
- **Debt-to-Equity Ratio**

These ratios show different aspects of a company's financial health — like profitability, liquidity, efficiency, and debt levels.

To make it easier to compare the companies, I created a simple scoring system. Each ratio was given a weight based on how important it is when evaluating retail businesses. Then, I combined these to give each company a final score from **0 to 100**.

### Ratio Scoring Ranges

Before scoring, I defined **expected value ranges** for each financial ratio based on typical benchmarks in the retail industry. These ranges help normalize values and give context — what’s considered strong or weak performance for each metric:

| Metric            | Low–High                  |                                                              
|-------------------|---------------------------|
| **ROI**           | 5% – 20%                  | 
| **Gross Margin**  | 10% – 30%                 |
| **ROS**           | 2% – 6%                   |
| **Current Ratio** | 0.5 – 1.5                 | 
| **Quick Ratio**   | 0.2 – 1.0                 | 
| **Asset Turnover**| 1 – 3                     |
| **Debt-to-Equity**| 2.5 – 0.5                 | 

These ranges were used to **scale each ratio between 0 and 100** before applying the weighted scoring model.

### Weighting Explanation

Here’s why I assigned the weights the way I did:

- **ROI (30%)** — It is the most important because good returns are crucial for growth.
- **Gross Margin (25%)** — Since retail depends a lot on controlling costs of goods sold, this ratio is very important.
- **ROS (10%)** — Shows how efficiently the company turns sales into profit.
- **Current Ratio (10%)** — Measures short-term financial health and liquidity.
- **Quick Ratio (5%)** — A stricter liquidity test than the Current Ratio, but slightly less critical, so it has a smaller weight.
- **Asset Turnover (10%)** — Shows how well the company uses its assets to generate sales, important for retail low margin environment.
- **Debt-to-Equity (5%)** — Retail companies usually carry moderate debt, so it has the lowest weight.

This scoring model helps to compare Walmart, Target, and Costco fairly and see which company has the strongest overall financial position based on these key ratios.

## Results

| Company         | ROI (%) | Gross Margin (%) | ROS (%) | Current Ratio  | Quick Ratio  | Asset Turnover | Debt-to-Equity |
|---------------  |---------|------------------|---------|----------------|--------------|----------------|----------------|
| Walmart       | 18.50   | 24.38            | 3.78    | 0.83           | 0.24         | 2.57           | 1.93           |
| Target Corp    | 30.81   | 27.54            | 5.40    | 0.91           | 0.29         | 1.94           | 3.12           |
| Costco        | 31.19   | 12.61            | 3.89    | 0.97           | 0.44         | 3.64           | 1.96           |


Financial scores:

**Target** - 70
**Walmart** - 62
**Costco** - 56



