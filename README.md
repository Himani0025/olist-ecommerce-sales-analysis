# Olist E-Commerce Sales Performance Analysis

End-to-end data analysis project on 100K+ Brazilian e-commerce orders 
using Python and Power BI.

## Tools Used
Python (Pandas, NumPy, Matplotlib, Seaborn) | Power BI (DAX, Data Modeling)

## Dataset
[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
8 relational tables, 100K+ orders (2016-2018)

## Business Problem
Analyze sales performance, delivery efficiency, and customer satisfaction
to identify growth opportunities and operational bottlenecks.

## Key Findings
- Total Revenue: R$13.20M across 96,286 orders
- Average delivery time: 12 days (93.4% delivered on time or early)
- Health & Beauty is the top revenue category (R$1.23M)
- Average customer review score: 4.05/5

## Process
1. Profiled 8 relational CSV tables individually using Pandas — checked
   nulls, duplicates, and data types
2. Merged tables using Pandas with careful handling of one-to-many
   relationships — aggregated payments before merging to avoid revenue
   duplication
3. Created 5 KPI columns using datetime calculations (delivery days,
   approval hours, seller handling time, carrier delivery time, 
   delivery vs estimate)
4. Performed EDA and built visualizations in Python (Matplotlib/Seaborn)
5. Built an interactive Power BI dashboard with DAX measures, 5 KPI
   cards, 5 charts, and 3 slicers — connected through a single data
   model for real-time filtering

## Dashboard Preview
![Dashboard](outputs/dashboard_screenshot.png)

## How to View the Interactive Dashboard
Download `powerbi/olist_dashboard.pbix` and open it in 
[Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/downloads) (free)

## Project Structure
- `notebooks/` - Python data cleaning, merging, and EDA
- `outputs/` - Charts and dashboard screenshots
- `powerbi/` - Power BI dashboard file (.pbix)
