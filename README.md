# 📊 Customer Cohort Retention Analysis (MySQL & Power BI)

## 📌 Project Overview
This project demonstrates an end-to-end Business Intelligence workflow, from database engineering to data visualization. The objective is to analyze customer retention and churn rates over an 18-month period using Cohort Analysis. 

By tracking user activities and transactions based on their acquisition month, this dashboard provides actionable insights into customer lifecycle and engagement trends, which are crucial for calculating Customer Lifetime Value (CLV) and improving retention strategies.

## 🛠️ Tech Stack & Skills Demonstrated
* **Relational Database:** MySQL / MariaDB (Data Definition, Data Manipulation)
* **Advanced SQL:** Common Table Expressions (CTEs), Window Functions (`FIRST_VALUE`), Date/Time formatting, and Aggregations.
* **Data Connector:** MySQL ODBC 64-bit Driver
* **Data Visualization:** Power BI Desktop (Matrix Heatmap, DAX Measures, Conditional Formatting)

## 🗄️ Architecture & Workflow
1.  **Database Design:** Created a relational database `cohort_analysis_db` with Star Schema architecture (`dim_members`, `fact_activity_logs`, `fact_transactions`).
2.  **Data Generation:** Populated tables with synthetic data spanning 24 months, simulating varying subscription tiers (Basic, Standard, Premium) and realistic user states (Active, Inactive, Churned).
3.  **Data Transformation:** Built a robust SQL View (`vw_cohort_retention`) using CTEs to calculate cohort index and retention percentage per month natively in the database.
4.  **Dashboarding:** Connected Power BI directly to the MySQL View via ODBC. Developed a gradient heatmap matrix to visualize the churn naturally and utilized DAX to calculate the overall Average Retention Rate.

## 📈 Key Insights
* **Retention Heatmap:** Visualizes the progressive drop-off of users from Month 0 to Month 18.
* **Average Retention:** Successfully maintained an overall average retention metric (KPI) of **85.09%** across all cohorts.
* **Churn Pattern:** Distinct churn behavior is accurately captured, indicating active periods for specific membership groups before drop-off.

## 📂 Files Included
* `cohort_analysis_full.sql` : Full SQL script containing database schema setup, synthetic data generation, and the core retention view logic.
* `Cohort_Analysis_Portfolio.pbix` : The final interactive Power BI dashboard.
* `Dashboard_Preview.png` : High-resolution preview of the final dashboard heatmap and KPI.

<img width="1086" height="603" alt="image" src="https://github.com/user-attachments/assets/bbdcc895-64fa-4940-bf2a-4d32f1904568" />

