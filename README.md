# Manufacturing Downtime Analysis Project

<div align="center">
  <img width="334" height="355" alt="Logo" src="https://github.com/user-attachments/assets/0e72a058-f0d4-41d2-bf00-22bba5bd5b19" />


  <br>

  <img src="https://img.shields.io/badge/Business%20Intelligence-Tableau-blue?style=for-the-badge&logo=Tableau" alt="Tableau">
  <img src="https://img.shields.io/badge/Data%20Analysis-SQL-orange?style=for-the-badge" alt="SQL">
  <img src="https://img.shields.io/badge/Data%20Cleaning-Python%20%28Pandas%29-green?style=for-the-badge&logo=Python" alt="Python">
</div>

---

This analysis will support data-driven decision-making to enhance production efficiency.

## 1. Project Overview
This project analyzes production line stoppages to identify critical points affecting operational efficiency. By integrating production, operator, and downtime data, we built interactive dashboards for data-driven decision-making.

## 2. Objective
The objective of this project is to analyze manufacturing downtime to:
* Identify the main causes of production stoppages
* Reduce downtime duration
* Improve operational & production line efficiency

## 3. Problem Statement
The manufacturing process experiences frequent downtime events without a clear understanding of their root causes. This leads to reduced productivity and increased operational costs.

## 4. Data Description

### Dataset 1: Line Downtime
* **Batch:** Production batch ID
* **Downtime Factors (1-12):** Causes of downtime
* **Downtime:** Time lost per event

### Dataset 2: Downtime Factors
* **Factor:** Downtime factor ID
* **Description:** Explanation of each factor
* **Operator Error:** Indicates whether the cause is human-related (Yes/No)

### Dataset 3: Products
* **Product:** Product code and size
* **Flavor**
* **Size**
* **Min Batch Time:** Minimum time needed for batch production (with no downtime)

### Dataset 4: Line Productivity
* **Batch ID:** Production batch identifier
* **Product:** Product code and size
* **Operator:** Operator name responsible for the batch
* **Start DateTime:** Batch start date and time
* **End DateTime:** Batch end date and time
* **Duration:** Total batch run time calculated from Start and End DateTime

## 5. Data Preparation
* Cleaning data using PYTHON
* Transform data from wide format to long format using Unpivot
* Ensure correct data types
* Create a relationship between datasets using the "Factor" and "Batch" columns

## 6. Key Analysis Questions
* What are the most frequent downtime causes?
* Which factors contribute the most to total downtime?
* What is the average downtime per batch?
* Are most downtime events caused by operator errors or system issues?
* How do different shifts affect production line performance?

## 7. Key Performance Indicators (KPIs)
* Total Downtime (minutes)
* Average Downtime per event
* Number of Downtime Events
* Percentage of Operator Errors
* Average Cycle Time
* Total Production Output
* Line Availability
* MTBF (Mean Time Between Failures)
* MTTR (Mean Time to Repair)
* Operator with highest downtime rate

## 8. Dashboard Requirements
* Bar chart showing downtime by factor (Pareto Chart)
* Pie chart showing operator vs non-operator errors (both by no. of incident & Total downtime in min)
* KPI indicators (total and average downtime, Total Events, Operator Error %, Non-Operator Error %)
* Filters (Batch, Factor, Operator, Product, Date range, operator error (yes/no))
* Downtime trend analysis
* Products with highest downtime rate
* Heatmap Showing the best system of production
* Heatmap showing the weak point for every product
* Operator Downtime Rate for each Operator
* Operational Cost of CO-2L vs. CO-600 ml
* Total impact for each factor

## 9. Expected Outcomes
* Identification of major downtime causes
* Understanding the impact of human vs machine-related issues
* Actionable insights to reduce downtime

## 10. Dashboards & Insights

### 10.1 Operational Overview Dashboard
Focuses on high-level KPIs including Availability, Downtime Rate, MTTR, and MTBF. It tracks the daily production trend and highlights critical peaks in downtime.

<img width="1286" height="686" alt="لقطة شاشة 2026-05-18 181654" src="https://github.com/user-attachments/assets/1742cc99-5417-4b41-8560-fed7b9d380e3" />


### 10.2 Products Performance Analysis
Analyzes downtime impact across different product sizes (e.g., CO-600 vs. CO-2L). It highlights which products suffer from the most frequent stoppages and the associated costs.

<img width="1288" height="687" alt="لقطة شاشة 2026-05-18 181721" src="https://github.com/user-attachments/assets/de703d59-42ff-44f9-bde3-a58c0633502f" />


### 10.3 Operator Performance (Best Systems of Productions)
Evaluates individual operator efficiency and identifies their 'Best Systems of Productions'. It differentiates between machine failure and human-related errors.

<img width="1287" height="689" alt="لقطة شاشة 2026-05-18 181752" src="https://github.com/user-attachments/assets/c921d569-109a-48e0-8546-0718b088db03" />


### 10.4 Root Cause (Pareto Analysis)
Utilizes the 80/20 rule to pinpoint the vital few factors causing the majority of downtime. The dashboard highlights the 'Most Frequent Factor' for targeted intervention.

<img width="1289" height="688" alt="لقطة شاشة 2026-05-18 181816" src="https://github.com/user-attachments/assets/b7146e9c-7cbe-4473-b175-6a36cfea8404" />



## 11. Tech Stack
* **Python:** Data cleaning, unpivoting, and transformation.
* **Tableau:** Advanced visualization and Elite Dashboard design.

## 12. Strategic Recommendations
* Implement specialized training programs for operators focusing on "Machine Adjustment" procedures to reduce Operator Errors.
* Re-distribute production loads based on operator-specific efficiency metrics.
* Optimize maintenance schedules for products with high machine-adjustment downtime.
* Improve preventive maintenance strategies.
