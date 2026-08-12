# Superstore-Sales-Dashboard-Tableau
Tableau Project - Sales performance dashboard built in Tableau Public using the Superstore dataset. Identifies top-performing categories, loss-making products (Tables, Bookcases) and regional revenue distribution across 50 US states.
# 📊 Superstore Sales Performance Dashboard — Tableau

![Tableau](https://img.shields.io/badge/Tool-Tableau-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Domain](https://img.shields.io/badge/Domain-Sales%20%26%20Revenue-orange)

## Overview
Interactive Tableau dashboard analysing 4 years of US retail sales data
(2019–2022) for a fictional superstore. The dashboard enables drill-down
analysis by category, region, segment and time period to identify
revenue drivers and underperforming product lines.

## Live Dashboard
🔗 [View on Tableau Public]() ← (https://public.tableau.com/views/Book1_17863601484420/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Dataset
- **Source:** Sample Superstore (built-in Tableau dataset)
- **Records:** 9,994 orders
- **Period:** 2019 – 2022
- **Columns:** Order Date, Ship Mode, Region, State, Category,
  Sub-Category, Sales, Quantity, Discount, Profit

## Dashboard Components
| View | Chart Type | Key Insight |
|---|---|---|
| KPI Summary | BAN Cards | Total Sales, Profit, Margin %, Orders |
| Sales Trend | Line Chart | Monthly revenue with trend line by category |
| Category Performance | Bar Chart | Sub-category sales coloured by profit margin |
| Regional Map | Filled Map | Sales heatmap across US states |
| Customer Segments | Treemap | Revenue by segment and category |
| Sales vs Profit | Scatter Plot | Identify loss-making products |

## Calculated Fields
- `Profit Margin %` — SUM(Profit) / SUM(Sales)
- `Average Order Value` — SUM(Sales) / COUNTD(Order ID)
- `Profit Status` — Profitable / Break Even / Loss classification
- `YoY Sales Growth %` — year-over-year growth using LOOKUP()
- `Days to Ship` — DATEDIFF between Order Date and Ship Date

## Key Findings
1. Technology is the highest-revenue category but Furniture has the lowest margin
2. The West region leads in sales; the Central region has the lowest profit margin
3. Tables and Bookcases are consistently loss-making sub-categories
4. Consumer segment accounts for ~50% of total revenue

## Features
- Interactive filters: Category, Region, Year, Segment
- Cross-filtering: clicking any chart filters the entire dashboard
- Trend lines on time series for visual forecasting

## Project Structure
```
📂 tableau-superstore-sales/
├── README.md
├── screenshots/
│   └── dashboard_overview.png
└── data/
    └── superstore.csv
```

## Tools
- Tableau Public (Desktop + Online)
- Calculated Fields, Table Calculations, Geographic Maps
