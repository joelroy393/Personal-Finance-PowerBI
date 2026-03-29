Project: Financial Intelligence Dashboard (Iteration 1)
Portfolio Context
This is the first project in my Data Analyst Portfolio. My goal is to master the full lifecycle of data—from raw ingestion to high-level business intelligence—and to document my progression as I advance my technical stack (Power BI, SQL, Python).

Objective
The primary objective of this iteration was to move from raw data to a functional, interactive dashboard as efficiently as possible. I focused on establishing a solid foundation in ETL (Extract, Transform, Load) processes and DAX (Data Analysis Expressions) logic.

Technical Implementation
1. Data Transformation (Power Query)
Cleaned and structured raw financial datasets.

Implemented a dynamic date hierarchy for time-series analysis.

Managed data types to ensure calculation accuracy across all measures.

2. Analytical Logic (DAX)
To move beyond basic Excel-style filtering, I developed custom measures using DAX. This allows the dashboard to recalculate instantly based on user interaction.

// Calculates total burn rate by isolating expense transactions
Total_Expense_Amount = 
CALCULATE(
    SUM('Sheet1'[Amount]), 
    'Sheet1'[Type] = "Expense"
)

// Measures net liquidity (Income vs. Expenses)
Net_Savings = [Total_Income_Calc] - [Total_Expense_Amount]
Dashboard Insights
KPI Tracking: Real-time visibility into Income, Expenses, and Savings.

Categorical Analysis: A breakdown of spending habits (e.g., Tech, Rent, Groceries) via interactive Donut Charts.

Time-Series Trends: A month-over-month comparison of earnings versus spending to track financial health.

Skills Demonstrated
Business Intelligence: Power BI Desktop

Languages: DAX, M (Power Query)

Data Modeling: Star Schema basics and Measure Branching

Workflow: Version control and iterative development

Advancement Goals for Iteration 2
[ ] Connect the dashboard to a live SQL database.

[ ] Integrate Python scripts for advanced trend forecasting.

[ ] Enhance UI/UX with custom themes and advanced drill-through actions.
