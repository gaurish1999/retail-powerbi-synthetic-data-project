## *Retail Margin Analysis: The Impact of Discounting Strategies on Profitability*
An interactive and data driven Power BI dashboard demonstrating retail analytics built on an AI‑generated synthetic dataset. Includes DAX measures, screenshots, and a short case study.

## Dataset Disclosure
This is a Power BI report that demonstrates end‑to‑end retail analytics using a fully AI‑generated synthetic dataset. The project showcases data modeling, DAX measures, M code manipulation, interactive dashboard design, and example analyses (sales trends, segmentation, inventory health, etc.). No real customer or proprietary data was used; the dataset was generated for targeted usecases to mimic realistic retail patterns for learning and demonstration purposes.

## 📌 Project Overview
This project investigates the "Profitability Paradox" within a mid-sized retail chain. While top-line revenue has shown consistent growth, overall profit margins have stagnated. This Power BI report was developed to determine if aggressive store-level discounting strategies are driving genuine business growth or merely eroding margins to inflate sales volume.

## Business Question
- **Business Context:** **Total Revenue** is hitting record highs this year, the company's **Total Profit** is flat or even slightly declining.
- **Objective**: Are our aggressive discounting strategies actually driving profitable growth, or are we just eroding our margins to move volume?

## Key Intelligence Questions
#1. **The Executive Check:** *Is the volume making up for the lower price?*
- **The Analysis:** A Comparison of **Total Sales Growth** vs. **Total Profit Growth** year-over-year.

#2. **Root cause identification:** *Which specific products or stores are the worst offenders?*
- **The Analysis:** A Scatter Plot showing **Average Discount %** on the X-axis and **Profit Margin %** on the Y-axis.
* *Insight:* Dots in the bottom-right corner are the "problem products" (High Discount, Low Profit).
* **The Drill Down:** A matrix showing which Stores are giving the highest discounts. Are they selling more units than stores that don't discount?

#3 **Customer Impact:** *Are we discounting for the wrong people?*
* **The Analysis:** A Stacked Bar Chart of **Sales by Customer Segment**, split by "Discounted" vs. "Full Price" transactions.
* *Insight:* Might discover that the high-income customers are buying mostly discounted items. This suggests the company is losing money unnecessarily.

By analyzing customer demographics, product categories, store performance, and discount tiers, this project provides actionable intelligence to optimize pricing strategies and protect the bottom line.

## 🛠️ Tech Stack & Methodologies
* **Business Intelligence:** Power BI
* **Data Transformation (ETL):** Power Query (M Language) for data profiling, cleansing, and outlier handling.
* **Data Modeling:** Robust Star Schema architecture ensuring optimized 1-to-many relationships and rigorous referential integrity.
* **Calculations:** Advanced DAX measures for dynamic time intelligence, percentage profit calculations, root cause analysis, field parameteres and bookmarks.

## 📂 Dataset Architecture
The data model is structured into a highly optimized Star Schema to separate transactional metrics from descriptive attributes:
* **Fact Table:** `Fact_Sales` (Transactions, Quantities, Revenue, Discounts)
* **Dimension Tables:** * `Dim_Customer` (Demographics, Segments)
  * `Dim_Product` (SKU, Categories, Base Costs)
  * `Dim_Store` (Locations, Store Types)
  * `Dim_Date` (Time Intelligence)

## 📊 Report Structure & Key Insights

The interactive `.pbix` file is structured into three targeted layers to serve different business audiences:

### 1. Executive Summary/Sales Breakdown (The "What")
* **Target:** C-Suite / VPs
* **Focus:** High-level KPI tracking comparing Total Revenue vs. Total Profit year-over-year.
* **Key Feature:** Identifies the point of divergence where volume growth fails to compensate for margin loss due to heavy discounting.

### 2. Root Cause Analysis (The "Why")
* **Target:** Regional Managers / Sales Directors
* **Focus:** Granular breakdown of discounting behaviors by store and product category.
* **Key Feature:** Scatter plot analysis mapping Average Discount % against Profit Margin % to isolate "problem products" and identify which store locations are over-utilizing discounts.

### 3. Customer Impact (The "Who")
* **Target:** Marketing & Operations
* **Focus:** Demographic segmentation of discount utilization.
* **Key Feature:** Highlights purchasing behaviors, revealing if high-value customer segments (who may have purchased at full price) are unnecessarily capturing discount margins.

## 🚀 How to Run the Project
1. Download the `Retail_Margin_Analysis.pbix` file from this repository.
2. Open the file using **Power BI Desktop**.
3. Utilize the custom left-hand navigation pane to seamlessly switch between the Executive, Root Cause, and Customer report pages.
4. Interact with the slicers (Date, Region, Store Type) to see the DAX measures dynamically recalculate.

## 💡 Key Takeaway
This project demonstrates the ability to look beyond surface-level descriptive statistics (like Total Sales) and leverage data modeling and DAX to answer complex, margin-focused business questions.
