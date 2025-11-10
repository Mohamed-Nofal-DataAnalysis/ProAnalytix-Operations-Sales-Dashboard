# ProAnalytix - Full Operations & Sales Interactive Dashboard
**(Built 100% in Power BI – 4 Pages of Pure Business Intelligence)**

## Project Objective
Create a **complete enterprise-grade Power BI dashboard** for **ProAnalytix** that combines:
- Production Efficiency & Machine Downtime
- Customer Demographics & Sales by Geography
- Return Rate & Cost Analysis
- Financial Performance 2015-2017  
All connected with **real-time slicers** across 4 pages for instant decision-making!

## Dataset Used
[Download Full Dataset (4 Excel Files + PBIX)](https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/tree/main/Dataset)

## Questions (KPIs) Answered Instantly Across 4 Pages
- **Production**: Efficiency Rate = **79.8%** | Machine Utilization = **89.86%** | Downtime = **394.9 hrs**
- **Sales**: Total Sales = **$24.15M** (+166.3% YoY) | Total Profit = **$10.14M** (+171.5% YoY)
- **Returns**: Total Returns = **960** (+1942% YoY) | Return Rate = **288.85%** | Cost of Returns = **$161K**
- **Customers**: 18K Customers | Avg Income = **$57K** | Top Category = **Bikes ($22.9M)**

## Dashboard Interaction (One slicer changes ALL 4 pages!)
[Sales Dashboard](https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Sales.png) | 
[Product Dashboard](https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Product.png) | 
[Return Dashboard](https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Return.png) | 
[Production Dashboard](https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Production.png)

## Process (Enterprise Level – Step by Step)
1. **Data Collection** → 8 tables (Orders, Returns, Products, Customers, Machines, Downtime, Geography, Calendar)
2. **Data Cleaning** → Power Query (Fixed dates, removed duplicates, merged queries, created hierarchies)
3. **Data Modeling** → **Snowflake + Star Schema** + Bidirectional relationships
4. **DAX Measures** → 40+ advanced measures including:
   ```dax
   Efficiency Rate = DIVIDE([Total Act Quantity], [Total Target Quantity]) * 100
   Return Rate = DIVIDE([Total Sales by Returns], [Total Sales]) * 100
   YoY Growth % = 
   VAR CurrentYear = SUM(Sales[Amount])
   VAR PreviousYear = CALCULATE(SUM(Sales[Amount]), PREVIOUSYEAR('Date'[Date]))
   RETURN DIVIDE(CurrentYear - PreviousYear, PreviousYear)
Interactive Slicers (Synced Across All Pages):
Year | Quarter | Region | Category | Subcategory | Machine Name | Work Center | Gender | Education
Visuals Used:

Donut Charts | Bubble Maps | Funnel | Line + Column Combo | 100% Stacked Bar | KPI Cards | Custom Icons | Drill-through

Dashboard Screenshots (Click to enlarge)
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Sales.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Product.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Return.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/Bakery-Sales-Revenue-Power-BI-Dashboard/blob/main/Home%20Page%20.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Production.png">
<img src="https://github.com/Mohamed-Nofal-DataAnalysis/ProAnalytix-Operations-Sales-Dashboard/blob/main/Modeling.png">

## Key Insights That Will Change Your Strategy

Machine2 produces 31M units but has highest downtime (120 hrs) → urgent maintenance needed!
Bachelors generate $24.1M in sales → target marketing campaigns for college grads
Return Rate exploded +1942% YoY → "Broken part" = 31.78% of complaints → quality control crisis!
Bikes category = 95% of revenue → Accessories & Clothing are dead weight
France & Australia = top returning countries → review shipping partners there

## Final Conclusion:
This isn’t just a dashboard… it’s a complete operations control room.
One click shows you:

Which machine to fix today
Which customer segment to target
Which product to kill
Which region is bleeding money

Ready-to-use Power BI file (4 pages + bookmarks + drill-through)
Download ProAnalytix_Dashboard.pbix
Built with fire by Mohamed Nofal – November 2025
