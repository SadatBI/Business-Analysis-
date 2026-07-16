# Financial Data Transformation and Performance Analysis for Nebulon

This repository contains a comprehensive business intelligence project focused on cleaning, transforming, and analyzing the financial data of **Nebulon**. The goal of this project is to turn unorganized financial data into a clean, star-schema relational model optimized for detailed financial reporting and interactive visualization.

## 📌 Project Overview
As a Business Analyst, the primary objective was to resolve data architectural limitations that prevented effective reporting. The original dataset structure made it highly difficult to build pivot tables, generate Power BI visualizations, or write Data Analysis Expressions (DAX) formulas for calculated columns and measures. 

By leveraging **Power Query** and **DAX** in Power BI, the data was successfully restructured to enable deep financial performance tracking, budget-versus-actual analysis, and efficiency metric benchmarking.

---

## 🛠️ Tech Stack & Tools
* **Power Query:** For ETL (Extract, Transform, Load) processes, unpivoting, and data cleaning.
* **Power BI Desktop:** For data modeling, DAX engineering, and report dashboard design.
* **DAX (Data Analysis Expressions):** For building custom business measures and time-intelligence calculations.

---

## 🚀 Key Tasks & Deliverables

### 1. Data Cleaning & Transformation (Power Query)
* Restructured the dataset to ensure compatibility with dimensional modeling.
* Cleaned null values, adjusted data types, and unpivoted columns to build clean fact and dimension structures.

### 2. DAX Measure Engineering
Developed core financial metrics and time-intelligence calculations to track business health:
* **Total Revenue** & **Total Expenses**.
* **Total Actual vs. Budgeted Revenue**.
* **Total Actual vs. Budgeted Expenses**.
* **June Snapshot:** Isolated actual revenue and expenses specifically for the month of June.

### 3. Financial Performance & Efficiency Analysis
Implemented explicit formulas to evaluate organizational efficiency:
* **Revenue Efficiency:** Measures how successfully actual revenues exceed established budget targets.
* **Expense Efficiency:** Tracks cost-control metrics to ensure actual expenses remain below budgeted figures.

### 4. Interactive Data Visualization
Created structured visual reports to communicate insights clearly to stakeholders:
* **Total Actual Revenue by Item Category:** Horizontal bar chart mapping performance across divisions (e.g., Fashion, Electronics, Office Supplies) featuring explicit data labels.
* **Total Actual Expenses by Expense Category:** Horizontal bar chart mapping breakdown of operational costs (e.g., Labour & Benefits, Cost of Sales, Operational Expenses).

---

## 📊 Strategic Insights Generated
The reporting dashboard directly answers critical business questions regarding Nebulon's $200K revenue performance benchmark (against its $238.96K budget goal):
* **Revenue Performance:** Identifies top-performing categories and analyzes underlying drivers like market demand and pricing.
* **Cost Management:** Highlights operational spending disparities and identifies which categories incur the heaviest cost burdens.
* **Financial Health:** Compares margin gaps where revenue outpaces or lags behind expenses to advise leadership on budget forecasting and resource allocation.
