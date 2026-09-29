# BrightMart Retail Sales Dashboard

## Project Overview

This project presents an interactive Power BI dashboard developed to analyze BrightMart's retail sales performance. 
The dashboard provides insights into sales, profit, regional performance, product performance, customer segments,
and order fulfilment.


## Dashboard Pages

### 1. Executive Overview
- Total Sales
- Total Profit
- Profit Margin
- Total Orders
- Average Order Value
- Sales trend over time
- Revenue by region

### 2. Regional & City Performance
- Sales and profit by region
- State and city-level performance
- Regional comparison

### 3. Product & Category Analysis
- Sales and profit by category and sub-category
- Top and bottom performing products
- Discount vs Profit analysis

### 4. Customer & Segment Insights
- Sales by customer segment
- Profit by customer segment
- Top customers
- New vs Repeat customer analysis

### 5. Order Fulfilment
- Orders by Ship Mode
- Average fulfilment days by region
- On-time vs delayed dispatch analysis


## Dataset
The dataset contains retail transaction information including:

- Order details
- Customer information
- Region, State and City
- Product, Category and Sub-Category
- Quantity and Unit Price
- Discount
- Sales and Profit
- Ship Date and Ship Mode
- Customer Segment


## Tools Used

- Microsoft Power BI
- Power Query
- DAX


## Key DAX Measures

```DAX
Total Sales =
SUM(retail_sales_dataset[Sales])

Total Profit =
SUM(retail_sales_dataset[Profit])

Total Orders =
DISTINCTCOUNT(retail_sales_dataset[OrderID])

Profit Margin % =
DIVIDE([Total Profit], [Total Sales], 0)

Average Order Value =
DIVIDE([Total Sales], [Total Orders], 0)
