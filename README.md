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

```bash
1. Run local server (opens automatically at http://localhost:8002/)
python server.py

# Or double-click run_local.bat on Windows
```

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

## 🌐 How to Push to GitHub & Deploy 100% Free Live Demo

### Step 1: Commit Local Changes
```bash
git add .
git commit -m "feat: Add full Data Analytics stack (Python, SQL, Power BI, Excel, Tableau) - by Aman Dwivedi"
git branch -M main
```

### Step 2: Push to GitHub
```bash
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/walmart-data-analytics.git
git push -u origin main
```

### Step 3: Enable Free Live Demo (GitHub Pages)
1. Go to repository **Settings** &rarr; **Pages**.
2. Select **Source**: `Deploy from a branch`.
3. Set **Branch**: `main` and folder `/(root)` &rarr; Click **Save**.
4. Your live link will be ready at:
   ```
   https://YOUR_GITHUB_USERNAME.github.io/walmart-data-analytics/
   ```

---

## 👤 Author

**Aman Dwivedi**  
- **Role**: Data Analyst / Business Intelligence Engineer  
- **Stack**: Python • SQL • Power BI • Excel • Tableau  
- **GitHub**: [github.com](https://github.com/)
