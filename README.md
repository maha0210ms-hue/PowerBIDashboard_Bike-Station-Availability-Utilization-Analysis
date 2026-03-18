# Bike Station Availability & Utilization Analysis
A comprehensive analysis of bike-sharing network performance across station capacity, bike availability, utilization efficiency, and geographic distribution to identify operational gaps and support smarter mobility decisions.

## 📖 Table of Contents
- [Project Overview](#-project-overview)
- [Data Source](#-data-source)
- [Tools & Technologies](#-tools--technologies)
- [Data Cleaning & Preparation](#-data-cleaning--preparation)
- [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [Key Insights](#-key-insights)
- [Recommendations](#-recommendations)
- [How to Use](#-how-to-use)

---

## 📊 Project Overview
This project analyzes a bike-sharing network to understand operational performance across **bike availability, station capacity, utilization rate, station-level performance, and country-wise distribution**.

The goal of this analysis is to identify underutilized capacity, uneven bike allocation, and regional usage patterns to improve operational efficiency and support data-driven decision-making.

The primary objectives were:

- To analyze **overall bike availability and station capacity**
- To evaluate **utilization efficiency across the network**
- To identify **high-performing and low-performing stations**
- To compare **bike availability across countries**
- To study the **growth trend of bikes over time**
- To understand **regional differences in station usage**

An **interactive Power BI dashboard** was created to present insights using multiple visuals and filters for better operational planning.

---

## 🗂️ Data Source
- **Source:** Entri Elevate
- **Format:** Excel
- **Domain:** Transportation Analytics / Urban Mobility

### Key Variables
#### Fact_Bike_Status
- station id
- bike stands
- available bike stands
- available bikes
- date

#### Dim_station
- station_number
- station_name
- latitude
- longitude
- city
- country
- banking
- bonus
- status

The dataset contains station-level bike-sharing data used to analyze availability, utilization, and geographic performance.

---

## 🛠️ Tools & Technologies
- **Visualization Tool:** Power BI Desktop  
- **Data Preparation:** Microsoft Excel  
- **Data Transformation:** Power Query  
- **Data Modeling:** Fact and Dimension Table Model  
- **DAX Measures:** Custom KPI calculations  
- **Interactive Features:** Slicers, Filters, KPI Cards, Maps, Trend Charts

---

## 🧹 Data Cleaning & Preparation
The following steps were performed before analysis:

1. Removed duplicate and unnecessary records.
2. Checked and corrected **data types** for numeric and date columns.
3. Handled **missing values** and removed blank station names.
4. Split the **position** column into **latitude** and **longitude**.
5. Split the **last update** column into separate **date** and **time** values.
6. Extracted clean **station names** from the name field.
7. Standardized text formatting for city names.
8. Generated **city** and **country** values using latitude and longitude.
9. Created separate **fact** and **dimension** tables for modeling.
10. Created DAX measures for core KPIs such as:
   - Total Bikes
   - Total Stands
   - Total Capacity
   - Utilization %

These steps ensured **clean, structured, and analysis-ready data**.

---

## 🔍 Exploratory Data Analysis (EDA)

The following business questions were explored:

- How many **bikes are currently available** across the network?
- What is the **total station capacity** and how much is underutilized?
- Which **countries have the highest bike availability**?
- Which **stations perform as major hubs**?
- How does **bike availability change over time**?
- Which regions show **low demand or inefficient distribution**?
- What is the **overall utilization rate** of the bike-sharing system?

### Visualizations Created
- KPI Cards (Total Bikes, Total Capacity, Available Bike Stands, Utilization %)
- Country-wise Bike Distribution Chart
- Station-wise Performance Chart
- Bike Trend Over Time (Line Chart)
- Geographic Map of Stations
- Utilization Comparison Visuals

---

## 💡 Key Insights
- The network has **13K available bikes** with a **total station capacity of 40K**.
- There are **22K available bike stands**, showing a large amount of unused capacity.
- The **overall utilization rate is 32.76%**, indicating underutilization across the network.
- **France** accounts for the highest share of bike availability in the system.
- Stations such as **Balzac Boulevard** and **Magellan** maintain higher bike counts and act as operational hubs.
- The bike availability trend shows **steady network growth over time**.
- Some regions have a higher number of empty stands than bikes, suggesting **lower demand or inefficient redistribution**.

---

## 🚀 Recommendations
- Optimize **bike redistribution** from low-demand stations to high-demand locations.
- Expand capacity at **high-performing stations** where demand is consistently strong.
- Promote service adoption in **low-usage regions** through awareness campaigns or pricing strategies.
- Implement **demand forecasting** using historical trends to improve allocation planning.
- Improve **real-time accessibility** through digital platforms showing current bike availability.

---

## ⚙️ How to Use

To explore this project:

1. Download the **.pbix file** from this repository.
2. Open the file using **Power BI Desktop**.
3. Use available **filters/slicers** to analyze data by:
   - Country
   - Year
4. Hover over visuals to view detailed metrics.
5. Explore station trends, utilization, and geographic distribution through the interactive dashboard.

No additional dependencies are required beyond **Power BI Desktop**.
