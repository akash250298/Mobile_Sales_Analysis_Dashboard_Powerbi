# Mobile_Sales_Analysis_Dashboard_Powerbi

# 📱 Mobile Sales Power BI Project by
**By Akash Kharche**  

## 📌 Project Overview

This dynamic Power BI project analyzes mobile sales across time, location, payment channels, and product lines.  
The dashboard delivers clear insights into **total sales, quantity, transaction volume, and pricing**—demonstrating technical expertise in DAX-driven KPIs, interactive reporting, and actionable business intelligence.

***

## 📋 Project Link (Power BI File - pbix):

[Mobile Sales Power BI Project](#)  
https://github.com/akash250298/Mobile_Sales_Analysis_Dashboard_Powerbi

***

## Dataset Description

Data is sourced from a comprehensive mobile sales transactional dataset.  
**Cleaning and enrichment were performed in Python** prior to Power BI import, ensuring accuracy and analytical readiness across all visualizations.

***

## 📊 Key Insights (Interactive Dashboard Highlights)

- **MTD (Month-to-Date) Sales Trend**
  - February 2022 sales reached **20M** on the dashboard, with growth tracked daily for actionable trend analysis.[1]
  - Visual MTD progression illustrates consistent performance increases through the month.

- **Sales Volume and Pricing Metrics**
  - Total Quantity sold: **445 (Feb) & 19K (annual)**.
  - Average Price Per Unit: **₹44.1K (Feb)** and **₹40.11K (annual)**.
  - Total Transactions: **96 (Feb)** and **4K (annual)**.

- **Yearly and Quarterly Performance**
  - 2022 sales: **¥769M**, with detailed quarter-by-quarter and month-by-month comparisons against the previous year.[2][3]
  - Bar & line charts empower rapid historical benchmarking and growth targeting.

- **Regional, Brand, and Payment Insights**
  - Top-performing cities and states mapped for regional targeting.
  - Brand-wise KPIs showcase major players (Apple, Samsung, OnePlus, Vivo) alongside model breakdowns.
  - Diverse payment method analysis (UPI, Debit, Credit, Cash) and transaction distribution visualized.

***

## 🛠️ Skills and Tools Demonstrated

### 🔹 Power BI Analysis & Visualization

- Developed a robust, interactive dashboard with **MTD, YTD, Regional, and Transactional KPIs** for all business stakeholders.
- Implemented slicers (month, mobile model, payment method, brand) and filters for on-demand drill-down.
- Delivered storytelling visuals (line, bar, pie, map, rating breakdown) for rapid, data-driven decisions.

### 🔹 Python Data Cleaning & Preparation

- Utilized **pandas** and **numpy** for efficient preprocessing:
  - Removal of anomalies, missing values, and duplications.
  - Conversion and formatting of numeric and date values for seamless Power BI analysis.
- Ensured one-source data integrity for Power BI transformations and DAX calculations.

### 🔹 DAX Calculations

The business logic leans on critical, reusable DAX formulas, including:
```DAX
MTD = TOTALMTD([Total_Sales], Custom_Calender[Date].[Date])
Same Period Last Year = CALCULATE([Total_Sales], SAMEPERIODLASTYEAR(Custom_Calender[Date].[Date]))
Total_Transactions = COUNTROWS(Mobile_Sales_Data)
Average_Price = AVERAGE(Mobile_Sales_Data[Price Per Unit])
Total_Sales = SUMX(Mobile_Sales_Data, Mobile_Sales_Data[Units Sold] * Mobile_Sales_Data[Price Per Unit])
Total_Quantity = SUM(Mobile_Sales_Data[Units Sold])
```
- Employed **conditional formatting** to contextualize performance surges (high-price/high-volume).
- Leveraged DAX aggregations and calculated columns for precise, rapid dashboarding.

### 🔹 Data Modeling & Power Query Steps

- Modeled a denormalized table for high-performance reporting and easy aggregations.
- Power Query Editor steps:
  - Imported the Python-cleaned dataset.
  - Promoted headers and set correct data types.
  - Created new calculated columns: “Total_Quantity”, “Average_Price”, and MTD measures.
  - Ensured logical column order and aggregation readiness.

***

## 🎯 Key Learnings

- Combining **Python for cleaning** and **Power BI for analytics** delivers scalable, reliable insights.
- Building effective, audience-ready dashboards with interactive visuals and custom DAX.
- Benchmarking sales across periods, locations, and brands to support operational strategy.
- Sharpened skills in end-to-end BI workflow: data cleaning, data modeling, dashboarding, and stakeholder storytelling.

***

## 📸 Screenshots  
1. Dashboard 1 : 
<img src="https://github.com/akash250298/Mobile_Sales_Analysis_Dashboard_Powerbi/blob/main/Dashboard_Screenshots/Dashboard%201.png" class="img-fluid">

2. MTD Report Dashboard 2 :
<img src="https://github.com/akash250298/Mobile_Sales_Analysis_Dashboard_Powerbi/blob/main/Dashboard_Screenshots/MTD%20report.png" class="img-fluid">

3. Same period last year Dashboard 3 :
<img src="https://github.com/akash250298/Mobile_Sales_Analysis_Dashboard_Powerbi/blob/main/Dashboard_Screenshots/Same%20period%20last%20year.png" class="img-fluid">

