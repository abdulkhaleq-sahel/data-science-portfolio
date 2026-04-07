# Project 1 - Data Analysis

📊 Superstore Strategic Business Discovery (EDA)
Data-driven insights to optimize retail profitability and sales performance.

📌 Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on the sales.csv dataset. By analyzing over 9,000 transactions, we identified key financial drivers, seasonal trends, and operational bottlenecks. This analysis serves as the strategic foundation for predictive modeling.

📂 Data Architecture
Dataset Path: project-1-data-analysis/data/sales.csv

Key Features: Sales, Profit, Discount, Category, Region, and Ship Mode.

🔍 Executive Summary of Findings
1. Risk & Outlier Audit
Median Profit: $8.67 per transaction.

Extreme Outlier: Detected a maximum loss of -$6,599.98, highlighting the need for stricter risk management in high-value orders.

2. Seasonal Sales Intelligence
Peak Performance: November 2017 was the highest-grossing month with $118,447.82 in sales.

Insight: Sales show a significant surge in Q4, indicating a strong holiday season impact.

3. Product Portfolio Analysis
Category Leader: Technology is the most profitable category ($145,454.95).

Profitability Gap: Furniture brings in high revenue ($741k) but suffers from very thin margins, yielding only $18,451 in total profit.

4. Regional Market Insights
Top Performer: The West Region is the company's primary profit engine, contributing $108,418.45.

5. The Correlation of Discounts
Finding: A negative correlation of -0.22 between Discount and Profit.

Business Rule: As discounts increase, profit margins consistently drop into negative territory, especially in the Furniture and Office Supplies segments.

6. Customer Value & Operations
High-Value Segment: Our top customer, Tamara Chand, generated $8,981.32 in net profit.

Logistics: First Class shipping proves to be the most profitable mode on average ($31.84), outperforming Standard Class.

💡 Strategic Recommendations
Discount Optimization: Implement a 20% "hard-cap" on manual discounts to prevent margin erosion.

Furniture Pricing Review: Re-evaluate the supply chain and shipping costs for Furniture to improve its low profit-to-sales ratio.

Inventory Management: Increase stock levels in the West region during October to prepare for the November sales peak.

VIP Retention: Focus marketing efforts on top-tier customers like Tamara Chand to ensure recurring high-margin revenue.

🛠️ Technical Stack
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Framework: Exploratory Data Analysis (EDA) & Statistical Correlation
