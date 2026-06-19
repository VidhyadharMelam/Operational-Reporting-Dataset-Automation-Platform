# Operational-Reporting-Dataset-Automation-Platform

## Project Overview
This project demonstrates how to build an **end‑to‑end operational reporting platform** using **Databricks, PySpark, and SQL**.  
The goal is to automate ETL workflows, prepare clean reporting datasets, and deliver dashboards that highlight **SLA compliance, workforce utilization, and processing efficiency**.  

It follows the **Medallion Architecture (Bronze → Silver → Gold)** to ensure reliable, structured, and analytics‑ready data for visualization.

---

## Tech Stack
- **Databricks + PySpark** → Data ingestion, cleaning, and transformation  
- **Delta Lake** → Reliable storage across Bronze, Silver, and Gold layers  
- **SQL** → Dimensional modeling and KPI aggregation  
- **Power BI** → Dashboard creation and KPI visualization  

---

## Dashboard Highlights
- **KPI Cards** → SLA compliance %, Avg processing time, Workforce utilization  
- **Trend Chart** → SLA breaches and performance trends over time  
- **Interactive Filters** → Department, time range, SLA category  
- **Narrative Insights** → Key takeaways for stakeholders  

---

## Data Flow

### 1. Bronze Layer
- Raw operational data ingested into Delta Lake.  
- Example fields:  
  - `Request_ID`  
  - `Department`  
  - `Start_Time`  
  - `End_Time`  
  - `SLA_Status`  
  - `Processing_Time`  

### 2. Silver Layer
- Cleaned and validated records.  
- SQL transformations applied for dimensional modeling (fact + dimension tables).  
- Example: remove duplicates, handle nulls, standardize SLA categories.  

### 3. Gold Layer
- Aggregated KPIs prepared for reporting.  
- Exported to CSV for visualization.  
- Example KPIs: SLA compliance %, Avg processing time, Workforce utilization.  

### 4. Visualization
- Power BI dashboard combining KPIs, trends, and filters.  
- Recruiter‑friendly layout: KPI cards at the top, trend chart in the middle, filters on the side, insights at the bottom.  

---

## How to Use
1. Clone the repository.  
2. Run notebooks in `notebooks/` to generate Bronze → Silver → Gold datasets.  
3. Open `gold/operational_reporting.csv` in Tableau/Power BI.  
4. Load the `.twbx` dashboard file to view KPIs and trends.  

---

## Repository Structure
├── notebooks/
│   ├── 01_data_ingestion.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_dimensional_modeling.ipynb
│   └── 04_reporting_kpis.ipynb
├── gold/
│   └── operational_reporting.csv
├── dashboard/
│   └── Operational_Reporting.twbx
└── README.md

Code

---

## Recruiter Note
This project highlights my ability to:
- Automate ETL pipelines with Databricks + PySpark  
- Apply SQL transformations for dimensional modeling  
- Deliver operational dashboards that improve KPI reporting consistency  
- Work in Agile delivery environments with clear documentation and reproducible pipelines  

---
