# HR-ANALYTICS-Workforce-growth-and-Current-Staff-Insights
Power BI HR Analytics Dashboard using Nazdate Chocolate Company's HR Data, focusing on workforce growth and current staff insights. It Includes headcount trends, Qualification vs salary analysis, leave balance monitoring, age and gender breakdowns and cumulative growth trajectory to support HR decision-making and workforce planning.
# HR Analytics Dashboard (Nazdate Chocolate Company)

## Overview
This repository contains a Power BI dashboard analyzing HR data from **Nazdate Chocolate Company**.  
The dashboard provides insights into workforce demographics, salary distribution, leave balance, and staff growth trends over time.  

The goal is to help HR teams monitor employee metrics, identify patterns, and make data-driven decisions.

---

## Key Steps in Building the Dashboard
1. **Data Preparation**
   - Imported Nazdate Chocolate HR dataset into Power BI.
   - Renamed dataset to **Staff**.
   - Converted:
     - `Date of join` → Date type
     - `Salary`, `Age`, `Leave balance` → Numeric type
   - Created **Age bins** (5-year intervals) column for demographic analysis.
   - Built a separate **Qual** table for educational qualifications with numeric IDs.
   - Established one-to-many relationship between `Staff` and `Qual`.

2. **Measures & Calculations**
   - **Headcount** = `COUNTROWS(Staff)`
   - **Average Salary**, **Max Salary**, **Min Salary**
   - **Top N earners** per job role
   - **Average Leave Balance**
   - **Employees with >20 Days Leave Balance**
   - **Cumulative Headcount** (running total of staff growth)

3. **Visualizations**
   - **Clustered Bar Chart**: Headcount by Job Title
   - **Pie Chart**: Gender breakdown per job role
   - **Stacked Column Chart**: Gender wise Age distribution (grouped bins)
   - **Table**: High Paying Job role compared with headcount
   - **Table**: Top earners in each job
   - **Scatter Chart**: Salary vs. Qualification ID
   - **Line Chart**: Cumulative headcount growth over time
   - **Slicer**: Employee name filter that begins with start letter
   - **Table**: Employee and job role with conditional formatting on salary
   - **Stacked Bar Chart**: Leave Balance Analysis
   - **Cards**: KPIs (Headcount, Avg. Salary, Average leave balance, Leave Balance over 20 Days)

4. **Formatting & UX**
   - Applied currency formatting to salary measures.
   - Conditional formatting with data bars for salary columns.
   - Formatting to Rectangular shape for dashboard title and inserted Nazdate chocolate company logo image.
   - Dashboard named **HR Analytics Dashboard**.

---

## Insights
- Rapid staff growth observed between **Sep 2018 – Dec 2018**.
- Product Managers have the highest average salaries, supported by decent headcount.
- Leave balance analysis shows some employees saving >20 days, indicating possible overwork.
- No clear qualification vs. salary trend (data appears random).
- Overall cumulative headcount: **161 employees**.

---

## Repository Contents
- `Nazdate_Hr_Data.xlsx` → Raw HR dataset (Nazdate Chocolate HR Data).
- `HR Analytics Dashboard.pbix` → Power BI dashboard file.
- `HR ANALYTICS.png` → Image of the dashboard.
- `README.md` → Documentation.


---

## Dashboard Preview
https://github.com/Parveen-Patel/HR-ANALYTICS-Workforce-growth-and-Current-Staff-Insights/blob/main/HR%20ANALYTICS.png



