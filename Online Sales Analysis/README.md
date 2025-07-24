# Project Goal
The main goal was to **evaluate annual sales** by identifying valuable customer segments and tracking revenue and retention trends, helping **define strategic focus areas for the next financial year**.

## Tools Used
- **SQL** for data filtering, RFM analysis, cohort analysis, and retention metrics  
- **Power BI** for data visualization

## Data set
[Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail)

This is a transactional data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

The dataset contains over 500,000 transactions, including customer IDs, countries, timestamps, quantities, and prices.

## Key Insights & Results
### RFM Analysis

RFM segmentation was done using SQL by assigning scores based on quantiles:

**Recency**: Calculated as days since the last purchase.

**Frequency**: Number of orders per customer.

**Monetary**: Total spend per customer.

| Segment Name            | Recency Score | Frequency/Monetary Score | Description                                     |
| ----------------------- | ------------- | ------------------------ | ----------------------------------------------- |
| **Best Customers**      | 4             | 4                        | Most loyal and valuable customers.              |
| **Loyal Customers**     | 4 or 3        | 3 or 4                   | Frequent and consistent buyers.                 |
| **Potential Loyalists** | 4 or 3        | 2 or 3                   | Growing loyalty, good potential.                |
| **Recent Customers**    | 4             | 1                        | New customers with only one purchase.           |
| **Promising**           | 3             | 2                        | Recently active but not yet fully engaged.      |
| **At Risk**             | 2             | 4                        | High past value but haven’t purchased recently. |
| **Need Attention**      | 2             | 2 or 3                   | Average customers who need re-engagement.       |
| **Can't Lose Them**     | 1             | 3 or 4                   | Previously loyal, now inactive – risk of churn. |
| **Lost Customers**      | 1 or 2        | 1 or 2                   | Low recent activity and value – likely lost.    |

