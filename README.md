# Online Retail Sales Analysis using Power BI

## Project Overview

This project focuses on analyzing online retail transaction data using Microsoft Power BI to understand sales performance, identify revenue trends, and generate actionable business insights.

The project involves data preparation, KPI development, interactive dashboard creation, and analysis of revenue across different months, items, customers, and countries.

## Objectives

- Analyze overall sales and revenue performance.
- Identify monthly revenue trends.
- Evaluate country-wise sales performance.
- Identify top revenue-generating items and customers.
- Develop an interactive Power BI dashboard.
- Generate business insights and recommendations based on the analysis.

## Dataset Description

The project uses an online retail transactional dataset covering the period from December 2010 to December 2011.

The dataset contains the following attributes:

| Column | Description |
|---|---|
| InvoiceNo | Invoice identifier for a transaction |
| StockCode | Product or item identifier |
| Description | Item description |
| Quantity | Number of units purchased |
| InvoiceDate | Date and time of the transaction |
| UnitPrice | Price per unit |
| CustomerID | Customer identifier |
| Country | Country associated with the transaction |

**Dataset source:** [UCI Machine Learning Repository – Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail)

## Tools and Technologies

- **Microsoft Power BI Desktop** – Dashboard development and visualization
- **Power Query** – Data cleaning and preparation
- **DAX** – KPI calculations and measures
- **Data Visualization** – Analysis of revenue trends and sales performance

## Data Cleaning and Preparation

The dataset was prepared using Power Query in Power BI.

The following steps were performed:

- Filtered records using the `Valid_Sale` column to retain valid sales transactions.
- Excluded cancelled invoices identified by invoice numbers beginning with `C`.
- Excluded transactions with non-positive quantities or unit prices according to the validation rules.
- Created a `MonthYear` field from the invoice date for chronological monthly analysis.
- Developed DAX measures to calculate the key performance indicators.

## Key Performance Indicators (KPIs)

| KPI | Value |
|---|---:|
| Total Revenue | £10,666,669.24 |
| Total Orders | 19,960 |
| Total Customers | 4,339 |
| Total Units Sold | 5,588,370 |
| Average Order Value | £534.40 |

## Dashboard Preview

The Power BI dashboard includes:

- KPI cards for overall sales performance
- Monthly Revenue Trend
- Top 10 Items by Revenue
- Top 10 Countries by Revenue
- Top 10 Customers by Revenue
- Month and Country slicers for interactive filtering

### Dashboard Screenshot

<img width="1037" height="626" alt="image" src="https://github.com/user-attachments/assets/0b452a31-e2ed-4830-994d-7725cbdd807e" />


## Key Insights

### 1. Country-wise Revenue Performance

The United Kingdom generated approximately **£9.03 million**, accounting for around **84.6% of total revenue**. The Netherlands ranked second, generating **£28,544.36**.

This indicates a high concentration of recorded revenue in the UK market.

### 2. Monthly Revenue Trend

November 2011 recorded revenue of **£1,509,496.33**, making it the highest-revenue month identified in the analysis.

This highlights the importance of examining seasonal purchasing patterns and end-of-year sales performance.

### 3. Item-wise Revenue Performance

DOTCOM POSTAGE generated **£206,248.77** in recorded revenue. Since it represents a postage-related charge rather than a conventional physical product, it should be considered separately when interpreting merchandise performance.

### 4. Overall Sales Performance

The business generated approximately **£10.67 million in revenue** across **19,960 valid orders**, with **5,588,370 units sold**. The average order value was **£534.40**.

## Business Recommendations

- **Market diversification:** Explore opportunities to increase revenue in markets outside the UK.
- **Seasonal analysis:** Investigate the products and purchasing patterns contributing to the November revenue peak.
- **Improved item classification:** Distinguish merchandise from postage charges when evaluating product performance.
- **Performance monitoring:** Track revenue, order volume, customer count, units sold, and average order value over time.
- **Data-driven decisions:** Use the interactive month and country filters to explore market and period-specific performance.

## Limitations

- The dataset covers December 2010 to December 2011.
- Product cost data is unavailable, so profit and profitability cannot be calculated.
- Explicit product category information is not available.
- The observed revenue concentration does not independently explain the reasons behind customer purchasing behaviour.
- Findings depend on the completeness and accuracy of the available transaction records.

## How to View the Project

1. Clone or download this repository.
2. Open the `.pbix` file in Microsoft Power BI Desktop.
3. Explore the dashboard using the Month and Country slicers.
4. Refer to the dashboard screenshot and project report for the main findings.

## Conclusion

This project demonstrates the use of Power BI, Power Query, and DAX to prepare transactional data, develop key performance indicators, visualize sales performance, and derive business insights.

The interactive dashboard provides an overview of monthly revenue trends, country-wise sales distribution, and top revenue-generating items and customers. The analysis highlights opportunities for market diversification, seasonal sales investigation, and improved item-level reporting.
