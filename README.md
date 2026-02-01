## *Retail Margin Analysis: The Impact of Discounting Strategies on Profitability*
An interactive and data driven Power BI dashboard demonstrating retail analytics built on an AI‑generated synthetic dataset. Includes DAX measures, screenshots, and a short case study.

## Dataset Disclosure
This is a Power BI report that demonstrates end‑to‑end retail analytics using a fully AI‑generated synthetic dataset. The project showcases data modeling, DAX measures, M code manipulation, interactive dashboard design, and example analyses (sales trends, segmentation, inventory health, etc.). No real customer or proprietary data was used; the dataset was generated for targeted usecases to mimic realistic retail patterns for learning and demonstration purposes.

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
