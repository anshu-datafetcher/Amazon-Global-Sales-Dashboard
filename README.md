# Amazon-Global-Sales-Dashboard
Amazon Global Sales Dashboard - Power BI Project
Overview
This repository features a visually compelling Power BI dashboard designed to analyze Amazon's global sales data. The dashboard offers insights into sales performance, market distribution, customer profitability, product trends, and geographic sales. It is an excellent tool for stakeholders to identify opportunities and address challenges in Amazon's global operations.

Key Features

KPIs
Sales Projection: Total revenue generated ($12.64M).
Product Unit: Number of units sold (3,788).
KPI Rating: Performance rating (178K).
Return: Total product returns (1,464).
Detailed Insights

Sales by Segment:
Breakdown of sales across segments: Consumer (30.25%), Corporate (18.27%), and Home Office (51.48%).
Pie chart visualization for easy interpretation.

Sales by Market:
Regional sales performance in Asia Pacific, Europe, USCA, LATAM, and Africa.
Market share analysis through a doughnut chart.

Sales by Region:
Interactive map displaying sales distribution across global regions.
Bubble sizes represent sales volumes.

Profit by Customer Name:
Top 10 customers by profit contribution.
Horizontal bar chart for comparison.

Loss by Product Name:
Identification of products causing losses.
Bar chart showcasing the highest loss-making products.

Profit by Product Name:
Analysis of top-performing products by profit.
Horizontal bar chart for easy reference.

Dataset
The dataset includes the following columns:
Sales Details: Total sales, units sold, returns, and KPI ratings.
Customer Details: Names and profitability.
Product Details: Product names, profit/loss metrics.
Geographic Data: Regional and market-specific sales.
Tools and Techniques
Data Cleaning: Processed raw data using Power Query.
Data Modeling: Established relationships to support in-depth analysis.
DAX Measures: Created custom calculations to derive KPIs.

Profit Calculation:
DAX
Profit = SUM(Sales[Revenue]) - SUM(Sales[Cost])

Loss Calculation:
DAX
Loss = IF(Sales[Profit] < 0, ABS(Sales[Profit]), 0)

Sales Contribution by Segment:
DAX
Segment Contribution % = DIVIDE(SUM(Sales[Segment Sales]), SUM(Sales[Total Sales])) * 100

Visuals
The dashboard includes:

Cards for KPIs like Sales Projection, Product Unit, and Returns.
Pie and Doughnut Charts for segment and market distribution.
Map Visualization for sales by region.
Bar Charts for profit/loss analysis by customer and product.
