# 🛒 Walmart Market End-to-End Data Analytics Platform (USA • Mexico • Canada)

> **Created & Architected by [Aman Dwivedi](https://github.com/)**  
> *A comprehensive enterprise data analytics portfolio spanning **Python**, **SQL**, **Power BI**, **Excel**, and **Tableau**.*

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-0071CE?style=for-the-badge&logo=github)](https://YOUR_GITHUB_USERNAME.github.io/YOUR_REPOSITORY_NAME/)
[![Author](https://img.shields.io/badge/Author-Aman%20Dwivedi-FFC220?style=for-the-badge&logo=linkedin&logoColor=black)](https://github.com/)
[![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![SQL](https://img.shields.io/badge/SQL-SQLite%20%2F%20PostgreSQL-4479A1?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)
[![Power BI](https://img.shields.io/badge/Power_BI-Desktop-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Excel](https://img.shields.io/badge/Excel-Financial_Model-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](https://www.microsoft.com/excel)
[![Tableau](https://img.shields.io/badge/Tableau-Public%20%2F%20Desktop-E97627?style=for-the-badge&logo=tableau&logoColor=white)](https://public.tableau.com/)

---

## 🎯 Project Overview

This project delivers a multi-tool **Data Analytics & Business Intelligence Solution** analyzing Walmart's cross-border retail performance across **Canada, Mexico, and the United States (1998)**.

The project demonstrates complete proficiency across the entire data lifecycle:
1. **Python**: Exploratory Data Analysis (EDA), Statistical **Ordinary Least Squares (OLS)** linear trend modeling, and automated ETL.
2. **SQL**: Relational database modeling (`walmart_analytics.db`), Window functions (`LAG`, `LEAD`, `DENSE_RANK`), CTEs, and quality anomaly detection flags.
3. **Power BI**: Star Schema data modeling, 1-to-many relationships, dynamic DAX measures, time-intelligence, and interactive slicers.
4. **Excel**: Multi-sheet financial model with dynamic formulas (`XLOOKUP`, `SUMIFS`), margin calculations, and conditional formatting.
5. **Tableau**: Visual calculated fields, Level of Detail (LOD) expressions, parameters, and 5-sheet interactive dashboard canvas architecture.

---

## 🚀 Interactive Live Web App & Localhost

Run the unified interactive portfolio locally or access the web app:


[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-0071CE?style=for-the-badge&logo=github)](https://aman2dwivedi.github.io/walmart-data-analytics/)
```bash

---

## 🛠️ Tool-by-Tool Implementation Breakdown

### 🐍 1. Python Data Science & Statistical OLS Suite
- **Script**: [`python/walmart_eda_analysis.py`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/python/walmart_eda_analysis.py)
- **Jupyter Notebook**: [`walmart_data_analytics.ipynb`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/walmart_data_analytics.ipynb)
- **Statistical Regression**:
  - Linear Trend Equation: $y = 374.53 \cdot x + 20247.96$
  - Coefficient of Determination: $R^2 = 0.7302$
  - P-Value: $7.81 \times 10^{-16}$ (Statistically significant revenue acceleration into Q4)
- **Run Command**:
  ```bash
  python python/walmart_eda_analysis.py
  ```

---

### 🗄️ 2. SQL Analytics Studio (SQLite / PostgreSQL / MySQL)
- **Schema DDL**: [`sql/walmart_schema.sql`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/sql/walmart_schema.sql)
- **Analytical Queries**: [`sql/walmart_queries.sql`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/sql/walmart_queries.sql)
- **Database File**: `walmart_analytics.db`
- **Key Techniques Used**:
  - Common Table Expressions (`WITH ... AS`) for Pareto distribution
  - Window Functions (`LAG()`, `LEAD()`, `DENSE_RANK() OVER (PARTITION BY store_country)`)
  - Anomaly Flagging (`CASE WHEN return_rate >= 0.0110 THEN '🚨 HIGH RISK'`)
- **Run Command**:
  ```bash
  python sql/run_queries.py
  ```

---

### 📊 3. Power BI Desktop & DAX Architecture
- **PBIX Report**: [`Wallmart Market Report(Power BI).pbix`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/Wallmart%20Market%20Report(Power%20BI).pbix)
- **DAX Measures Catalog**: [`powerbi/dax_measures.dax`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/powerbi/dax_measures.dax)
- **Key DAX Formulas**:
  - `Total Profit = [Total Revenue] - [Total Cost]`
  - `Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)`
  - `Return Rate = DIVIDE([Total Returns], [Total Transactions], 0)`
  - `MoM Growth % = DIVIDE([Current Month Txns] - [Last Month Txns], [Last Month Txns], 0)`

---

### 📑 4. Excel Financial Modeling
- **Workbook File**: [`excel/walmart_executive_model.xlsx`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/excel/walmart_executive_model.xlsx)
- **Structure**:
  - `Executive Summary`: High-level BAN cards and variance benchmarks.
  - `Brand Performance`: 25-brand matrix with `=G2/F2` profit margin formulas and `=J2/E2` return rate formulas with conditional formatting.
  - `Weekly Financials`: 52-week rolling revenue with cumulative running total formulas `=SUM($D$2:D2)`.

---

### 📈 5. Tableau Public & Desktop Architecture
- **Implementation Guide**: [`tableau/tableau_workbook_guide.md`](file:///c:/Users/dwive/Downloads/Power-BI-Walmart-Dashboard-main/tableau/tableau_workbook_guide.md)
- **Calculated Fields & LODs**:
  - Profit Margin: `SUM([Profit]) / SUM([Revenue])`
  - Fixed Country Revenue (LOD): `{ FIXED [Store Country] : SUM([Revenue]) }`
  - MoM Table Calculation: `(ZN(SUM([Revenue])) - LOOKUP(ZN(SUM([Revenue])), -1)) / ABS(LOOKUP(ZN(SUM([Revenue])), -1))`

---
Top-Tier Visual Badges & Header:

Dynamic badges for Live Interactive Demo, Author (Aman Dwivedi), Python 3.13, SQLite/SQL, Power BI Desktop, Excel Financial Model, Tableau, and Tailwind CSS.
Full-Stack Architecture & Workflow Diagram:

Clean Mermaid diagram illustrating the complete data pipeline from raw relational data → SQL database → Python OLS analysis → Power BI & Tableau → Web Hub.
Side-by-Side Dashboard & Model Screenshots:

Visual preview comparing the Topline Performance Dashboard, Star Schema Data Model, Market Insights, and Interactive Slicers.
Executive KPI Scorecard Table:

Structured breakdown of actual vs target benchmarks for 18,325 Transactions (+5.69%), 
71
,
682
P
r
o
f
i
t
(
+
5.61
71,682Profit(+5.61449,627 Net Revenue (59.94% Margin).
Tool-by-Tool Technical Deep Dive:

🐍 Python: Ordinary Least Squares (OLS) Linear Trend Regression (
Revenue
=
374.53
⋅
Week
+
20247.96
Revenue=374.53⋅Week+20247.96, 
R
2
=
0.7302
R 
2
 =0.7302, 
p
<
0.001
p<0.001), scatter plots, and Jupyter notebook walkthrough.
🗄️ SQL: Relational database architecture, CTEs, Window functions (LAG, LEAD, DENSE_RANK), and CASE WHEN return risk anomaly detection.
📊 Power BI: Star Schema (Fact tables: Transaction_Data, Return_Data, Dimensions: Calendar, Products, Stores, Regions), and DAX measures catalog.
📑 Excel: Multi-sheet financial model with =G2/F2 margins, =J2/E2 return rates, and =SUM($D$2:D2) cumulative revenue formulas.
📈 Tableau: Level of Detail (LOD) expressions ({FIXED [Store Country]: SUM([Revenue])}), calculated fields, and 5-sheet canvas layout.
Strategic Business Recommendations:

Portland December milestone replication, Top 10 brands Pareto rebates, return rate quality audits for Horatio and Nationeel, and Mexico logistics capital allocation.
Clean Directory Tree & Terminal Commands:

Step-by-step commands to clone, run the local server, run SQL queries, execute Python OLS regression, and launch Jupyter Notebook.

## 👤 Author

**Aman Dwivedi**  
- **Role**: Data Analyst / Business Intelligence Engineer  
- **Stack**: Python • SQL • Power BI • Excel • Tableau  
- **GitHub**: [github.com](https://github.com/)
