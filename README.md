# 📊 Sales Data Analysis Using DAX & Data Visualisation

This project demonstrates how to analyze sales data using Power BI, DAX (Data Analysis Expressions), and interactive data visualizations. The dataset is transformed into meaningful business insights by creating calculated measures, Calculated columns, Calculated table, KPIs, and dynamic dashboards. The report helps users understand sales performance, profit trends, customer behavior, product performance, and regional sales through interactive visuals.

## 📑 Table of Contents
* [Project Overview](#-project-overview)
* [Data Sources & Architecture](#-data-sources--architecture)
* [Data Transformation ETL](#-data-transformation-etl)
* [Data Model DAX](#-data-model-dax)
* [Dashboard Features](#-dashboard-features)
* [Key Insights](#-key-insights)
* [How To Use](#-how-to-use)

---

## 🎯 Project Overview

* **Business Problem:**
  Businesses generate large volumes of sales data every day, making it difficult to identify trends and measure performance using raw data alone. Without proper analysis, organizations may struggle to answer important business questions such as:

* Which products and categories generate the highest sales and profit?
* Which regions or cities perform the best?
* How are sales changing over time?
* What are the key business performance indicators?
* Which areas require improvement to increase revenue and profitability?

This project addresses these challenges by using DAX calculations and Power BI visualizations to transform raw sales data into actionable insights through an interactive dashboard.
  
* **Objective:**
  The primary objectives of this project are to:

* Analyze sales data using DAX measures and calculations.
* Build an interactive Power BI dashboard for business reporting.
* Track key performance indicators (KPIs) such as Total Sales, Total Profit, Average Sales, and Order Count.
* Identify top-performing products, categories, and regions.
* Monitor sales trends over time using Year-to-Date (YTD) and time-based analysis.
* Enable data-driven decision-making through clear and interactive visualizations
.
* **Target Audience:**
  Identify the primary users of Executive Leadership, Customers and Sales Operations.

## 🗃️ Data Sources & Architecture
* **Source Systems:** Text/Csv files.
* **Data Volume:** Maximum Thousand Five Hundred rows are listed in the files.
* **Storage Mode:** Using Import Mode.

## ⚙️ Data Transformation (ETL)
* **Tool Used:** Power Query Editor.
* **Key Cleanups:** Row Limiting & Data Type, Text Formatting, Merging Data using Joins,andling Missing Data & Duplicate Data, Sorting and Filtering Data.
* **Custom Functions:**
    1.	To find the Profit Margin  
               Formula: Profit / Amount
    

## 🧠 Data Model & DAX
* **Model Type:** This is Star Schema.
* **Fact Tables:** Order details table.
* **Dimension Tables:** List of Orders and Sales target Tables.
* **Key Measures:**
  ```dax
  Average Profit in Delhi = CALCULATE(AVERAGE('Order Details (2)'[Profit]),'List of Orders (2)'[City]="Delhi") 
  ```
  ```dax
  Year to Date Sales = TOTALYTD(SUM('Order Details (2)'[Revenue]),'Date'[Date])
  ```

## 🖥️ Dashboard Features
* **Page 1: Overview:** High-level KPI cards and strategic macro trends.
* **Page 2: Deep Dive:** Interactive granularity with cross-filtering matrices.
* **Page 3: Performance:** Interactive drill-down features and customized tooltips.
* **Design Theme:** Highlight custom color palettes, JSON themes, or accessibility choices.

## 💡 Key Insights
* **Trend A:** First major operations of Data Preparation, Data Cleaning and Data Aggregations are accomplished.
* **Trend B:** Data Integration and Data Modeling, DAX calculations are performed.
* **Recommendation:** Translating business logic into data models.

## 🚀 How To Use
1. **Prerequisites:**
   Ensure you have the latest Power BI Desktop installed.
   Prior knowledge in Power BI Interface operations, DAX Calculations and Data Visualisation.
   
3. **File Formats:** Clone the repository to access the `Sales Data Analysis Using DAX & Data visualisation.pbix` file.
   
5. **Data Refresh:** Change the source path under **Data Source Settings** to point to your data files.

  

