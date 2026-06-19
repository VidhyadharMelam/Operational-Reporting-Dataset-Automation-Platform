Project Flow (Medallion + Dashboard)
1. Data Ingestion
Load raw CSV/API data into Bronze layer.

Preserve all records exactly as received (no cleaning yet).

2. Data Cleaning
Apply null handling, type casting, and standardization.

Deduplicate on Request_ID if duplicates exist.

Output → Silver layer (clean, validated data).

3. Dimensional Modeling
Build Fact table (requests) and Dimension tables (employees, departments, priorities).

Fact table row count matches Silver unless filtering rules applied.

4. Gold Layer KPIs
Business metrics derived from Fact tables:

Step 4.1 → SLA Compliance % (overall).

Step 4.2 → Processing Time KPIs (avg/min/max, by dept/priority).

Step 4.3 → Departmental SLA KPIs.

Step 4.4 → Priority‑based SLA KPIs.

Step 4.5 → Combined Department + Priority SLA KPIs.

Step 4.6 → Trend Analysis KPIs (daily/weekly SLA + processing).

Step 4.7 → Anomaly Detection KPIs (spikes in SLA breaches/processing).

Step 4.8 → Forecasting KPIs (Prophet/ARIMA predictions).

Step 4.9 → Scenario Analysis KPIs (what‑if workload/staffing/efficiency).

Step 4.10 → Insights & Narrative (business story around KPIs).

5. Dashboard Visualization
Build a Tableau dashboard showcasing:

SLA compliance (overall, dept, priority, combined).

Processing time metrics.

Trends (time‑series charts).

Anomalies (highlighted spikes).

Forecasts (line projections).

Scenarios (what‑if comparisons).

Final deliverable → Recruiter‑ready dashboard file (.twb or .twbx).
