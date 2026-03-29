# Financial Intelligence Dashboard (Iteration 1)

**Personal Finance Analytics Dashboard built with Power BI**

![Power BI](https://img.shields.io/badge/Power%20BI-FF0000?style=for-the-badge&logo=powerbi&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-00B4A8?style=for-the-badge)

## Overview

This is the **first project** in my Data Analyst portfolio. The goal of this iteration was to take raw financial transaction data through the complete data lifecycle — from ingestion and cleaning to building an interactive, production-ready business intelligence dashboard.

### Objective
Transform messy raw financial data into actionable insights with real-time KPI tracking, spending analysis, and trend visualization using Power BI.

---

## Key Features

- **Live KPI Cards**: Track Total Income, Total Expenses, Net Savings, and Burn Rate
- **Spending Breakdown**: Interactive donut charts by category (Rent, Groceries, Tech, etc.)
- **Time-Series Analysis**: Month-over-month trends comparing Income vs Expenses
- **Dynamic Date Hierarchy**: Drill down from Year → Quarter → Month → Day
- **Fully Interactive**: All visuals cross-filter and update instantly

---

## Technical Implementation

### 1. Data Transformation (Power Query)
- Cleaned and standardized raw transaction data
- Proper data type handling for accurate calculations
- Created a dynamic date table for advanced time intelligence
- Implemented star schema data modeling

### 2. Analytical Logic (DAX)
```dax
// Total Income
Total_Income_Calc = CALCULATE(SUM('Sheet1'[Amount]),'Sheet1'[Type] = "Income")

// Total Expenses
Total_Expense_Amount = CALCULATE(SUM('Sheet1'[Amount]),'Sheet1'[Type] = "Expense")

// Net Savings
Net_Savings = [Total_Income_Calc] - [Total_Expense_Amount]
```
- **Custom DAX measures with proper measure branching
- **Time intelligence functions for MoM comparisons
- **Dynamic calculations that respond to slicers and filters


Dashboard Insights

- Real-time financial health monitoring
- **Clear visibility into spending patterns by category
- **Identification of monthly trends and seasonality
- **Quick detection of cash flow issues through burn rate tracking


Skills Demonstrated

- **Business Intelligence: Power BI Desktop (Report & Model view)
- **Languages: DAX, M (Power Query)
- **Data Modeling: Star Schema, Relationships, and Measure Branching
- **Workflow: Iterative development, version control, and documentation
- **Analytics: KPI design, trend analysis, and stakeholder-friendly visualizations


Project Goals Achieved

- ** End-to-end data transformation pipeline
 - **Production-quality interactive dashboard
 - **Advanced DAX calculations beyond basic Excel logic
 - **Clean, professional, and user-friendly design


Advancement Goals – Iteration 2

 - **Connect dashboard to a live SQL database
 - **Integrate Python scripts for forecasting (trend & anomaly detection)
 - **Custom themes and advanced UI/UX (bookmarks, drill-through, tooltips)
 - **Automated data refresh pipeline

 - **Custom DAX measures with proper measure branching
- **Time intelligence functions for MoM comparisons
- **Dynamic calculations that respond to slicers and filters


