# Growth-Infrastructure-Automation
This project focused on building a scalable analytics pipeline. I integrated customer and transaction data using Python, applied data quality checks to ensure reliability, and created KPI tables that feed Power BI dashboards. The goal was to eliminate manual reporting and provide stakeholders with trusted, up-to-date performance insights.

# Scalable Growth Infrastructure & Automation — Synthetic Dataset

This folder contains **synthetic** (fake but realistic) data to build an end-to-end analytics project:
- system integration (Python + SQL),
- data validation / QC checks,
- recurring performance reporting and dashboards (Power BI / Excel).

## Files
- `customer_data.csv`
- `sales_data.csv`
- `performance_metrics_daily.csv`
- `sales_leaderboard_monthly.csv`
- `data_quality_issues_sample.csv`
- `data_dictionary.json`

## Suggested Flow
1. Load `sales_data.csv` and `customer_data.csv`
2. Join on `customer_id`
3. Run validation checks (missing values, duplicates, outliers)
4. Build SQL views for KPIs (daily/monthly)
5. Create dashboards in Power BI (trends, approval rate, failures, leaderboard)

## Project Overview
This project demonstrates an end-to-end analytics workflow focused on building reliable, scalable reporting infrastructure. The goal was to integrate multiple data sources, ensure data quality, generate KPI-driven insights, and deliver interactive dashboards to support business decision-making.

---

## Step-by-Step Workflow

### Step 1: Load & Understand the Data
I loaded each dataset using Python (Pandas) and performed an initial review by checking column data types, identifying missing values, and detecting duplicate records. This early inspection helped prevent data issues from propagating into later stages of analysis.

---

### Step 2: Data Quality & Reliability Checks (QA/QC)
Before performing any analysis, I conducted data validation checks to identify missing customer records, duplicate transactions, invalid dates, and revenue outliers using IQR-based logic. Instead of deleting data blindly, I flagged issues, documented counts, and summarized quality findings to maintain transparency and trust in reporting.

---

### Step 3: System Integration
I merged sales transaction data with customer master data to create a single, unified dataset. This integration eliminated manual joins, standardized metrics, and established a single source of truth for reporting and analysis.

---

### Step 4: KPI & Reporting Tables
From the unified dataset, I created KPI-driven reporting tables, including daily KPIs (revenue, approval rate, dispute rate), monthly segmented KPIs by region, channel, and product, and leaderboard tables for performance tracking. These tables were designed to be SQL-ready, BI-ready, and reusable for dashboards, making the reporting process scalable.

---

### Step 5: Trend & Performance Analysis
I analyzed revenue trends, approval rate behavior, operational failure patterns, and performance across regions and channels. Rolling averages were applied to smooth short-term fluctuations and highlight meaningful trends, supporting data-driven decision-making rather than static reporting.

---

### Step 6: Visualization (Power BI)
Using the cleaned KPI tables, I built interactive Power BI dashboards that provide executive-level performance overviews, detailed breakdowns by region and channel, and sales leaderboards with incentive tracking. These dashboards allow stakeholders to filter by time, compare performance, and quickly identify potential issues.

---

## Final Outputs
By the end of the project, I delivered:
- A reproducible Jupyter Notebook
- Clean and validated datasets
- KPI tables ready for BI tools
- Interactive Power BI dashboards

---

## Skills Demonstrated
This project demonstrates the ability to:
- Clean and validate real-world data
- Integrate multiple datasets into a unified model
- Automate reporting workflows
- Build KPI-driven dashboards
- Focus on data reliability, not just visual presentation
- Communicate insights clearly to stakeholders

