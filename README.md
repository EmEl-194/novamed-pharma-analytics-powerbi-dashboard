# Novamed-pharma-analytics-powerbi-dashboard


## Overview
NovaMed Solutions is a leading pharmaceutical distributor serving diverse healthcare markets across multiple countries. This project provides a comprehensive analysis of NovaMed’s 2023 sales performance using Power BI, focusing on product profitability, customer behaviour, demographic trends, and geographic revenue distribution.
The goal of this analysis was to support data‑driven decision‑making by identifying high‑value products, key customer segments, operational inefficiencies, and strategic growth opportunities.


## Business Problem
NovaMed faces challenges in:
- Optimising sales performance
- Managing inventory across high‑ and low‑performing drugs
- Understanding customer behaviour and revenue concentration
- Identifying demographic and geographic growth opportunities
- Improving monthly sales consistency
These challenges impact profitability, operational efficiency, and long‑term market competitiveness.


## Project Objectives
This analysis aims to:
- Evaluate overall sales performance and profitability
- Identify top‑ and bottom‑performing drugs
- Analyse customer behaviour and revenue contribution
- Understand demographic drivers of revenue
- Assess geographic market performance
- Provide actionable recommendations to improve business outcomes


## Key Insights
- NovaMed generated $61.68M in revenue with an 81.9% profit margin, indicating strong cost efficiency.
- Revenue is highly concentrated — the top 5 drugs contribute 27% of total revenue.
- Monthly revenue and profit fluctuate significantly, suggesting seasonal demand or operational inefficiencies.
- Customer revenue is heavily skewed — top customers generate disproportionately higher revenue.
- Older customers (54–65) are the primary revenue drivers, contributing $17.17M.
- Revenue is evenly distributed across gender, with males contributing slightly more (47%).
- Sellers account for 88% of total revenue, indicating reliance on wholesale buyers.
- Canada and Australia dominate revenue generation, highlighting strong market concentration.


## Features of the Dashboard
- **KPI Overview:** Displays total revenue ($61.68M), total units sold, profit margin (81.9%), and total customers.
- **Top & Bottom Drug Performance:** Identifies high‑performing and underperforming drugs by revenue, profit, and units sold.
- **Monthly Sales Trends:** Shows revenue and profit fluctuations across the year, highlighting seasonal patterns and operational inconsistencies.
- **Customer Segmentation:** Breaks down customer performance by revenue, orders, and ranking.
- **Demographic Insights:** Analyses revenue by age group, gender, and buyer type (Seller vs User).
- **Geographic Performance:** Highlights revenue distribution across countries, showing market concentration and growth opportunities.
- **Interactive Filters:** Allows users to explore performance by drug, customer, year, and demographic attributes.


## How to Use This Dashboard
- **Explore KPIs:** Start with the KPI cards to understand overall business performance.
- **Analyse product performance:** Use the Top/Bottom visuals to identify high‑value and low‑value drugs.
- **Review monthly trends:** Hover over the line charts to compare revenue and profit month‑by‑month.
- **Segment customers:** Use the customer table to identify top customers and underperforming segments.
- **Investigate demographics:** Filter by age, gender, and buyer type to understand who drives revenue.
- **Examine geographic patterns:** Use the map and country charts to identify high‑performing markets.
- **Combine filters:** Apply multiple filters (e.g., drug + customer + country) to uncover deeper insights.


## Data Model
The data model follows a star schema with one fact table and two dimension tables:
### **1. FactTable**
Contains transactional sales data including:
- DrugID  
- CustomerID  
- Revenue  
- Profit  
- Units sold  
- Date fields  

### **2. DrugLookup**
Provides drug‑level metadata:
- Drug name  
- Unit sales price  
- Cost of production  
- Regulatory compliance  
- Treatment category  

### **3. CustomerTable**
Contains customer demographics:
- Age  
- Gender  
- Country  
- Customer type (Preferred, Frequent, New)  

### **Model Structure**
- FactTable is the central fact table.
- DrugLookup and CustomerTable are dimension tables.
- Relationships:
  - FactTable[DrugID] → DrugLookup[DrugID]
  - FactTable[CustomerID] → CustomerTable[CustomerID]
This structure supports efficient filtering, aggregation, and drill‑down analysis.


## Datasets Used
[FactTable.csv](data/FactTable.csv) — Transaction-level sales data  
[DrugLookup.csv](data/DrugLookup.csv) — Drug metadata including pricing and production cost  
[CustomerTable.csv](data/CustomerTable.csv) — Customer demographics and attributes  
These datasets were cleaned, modelled, and transformed in Power BI using Power Query and DAX


## Dashboard Screenshots
[KPI_Overview1.png](Overview1.png)
[KPI_Overview2.png](Overview2.png)
[Top_5_Drugs.png](Top_5_Drugs.png)
[Bottom_5_Drugs.png](Bottom_5_Drugs.png)
[Monthly_Performance.png](Monthly_Performance.png)
[Customer_Performance_Bottom5.png](Customer_Performance_Bottom5.png)
[Customer_Performance_Top5.png](Customer_Performance_Top5.png)
[Age_and_Gender_Distribution.png](Age_and_Gender_Distribution.png)
[Buyer_Type_Distribution.png](Buyer_Type_Distribution.png)
[Revenue_by_Country.png](Revenue_by_Country.png)


## Business Recommendations
1. **Prioritise high‑performing drugs**  
   Focus marketing, distribution, and inventory on the top 5 drugs, which contribute 27% of total revenue.

2. **Reassess low‑performing drugs**  
   Evaluate whether to reposition, promote, or discontinue bottom‑performing drugs to reduce inefficiencies.

3. **Improve monthly sales consistency**  
   Implement better demand forecasting and targeted campaigns to stabilise revenue across months.

4. **Strengthen relationships with top customers**  
   Develop loyalty programmes and personalised engagement strategies for high‑value customers.

5. **Optimise buyer type strategy**  
   Since Sellers contribute 88% of revenue, strengthen partnerships while expanding direct‑to‑User strategies.

6. **Protect and grow top countries**  
   Canada and Australia generate the highest revenue; invest in retention and expansion in these markets.

7. **Evaluate underperforming countries**  
   Reassess market strategy in low‑performing regions to improve penetration and profitability.

8. **Adopt continuous data‑driven decision‑making**  
   Use the dashboard regularly to monitor trends, identify risks, and support strategic planning.


## Conclusion
This Power BI case study provides a comprehensive view of NovaMed Solutions’ sales performance, highlighting key revenue drivers, customer behaviour, demographic patterns, and geographic opportunities. The insights and recommendations presented here support strategic decision‑making and operational improvement within the pharmaceutical distribution sector.

