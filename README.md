# Candy Sales Analytics Dashboard - Power BI Portfolio Project

## Project Overview
This Power BI project analyzes sales data for Treat Link, a US-based candy distributor business, from 2021-2024. I created an interactive dashboard that helps business owners understand their sales performance, track profit margins, and make data-driven decisions about their candy products. The dashboard shows key business metrics and trends in an easy-to-understand visual format for this fictitious company scenario.

## Business Problem
Candy distributors like Treat Link need to understand which products are selling well, when sales peak, and how profitable their business is. This project answers important questions like:
- Which candy products make the most money?
- Are we hitting our sales targets across different divisions?
- What are our profit trends throughout the year?
- Which shipping methods do customers prefer?
- How do different product categories perform compared to each other?

## Technical Skills Demonstrated
**Power BI & Data Visualization**
- **Interactive Dashboards:** Built clickable charts that update other visuals automatically
- **DAX Calculations:** Created custom formulas to calculate profit margins and growth rates
- **Advanced Visuals:** Used scatter plots, combo charts, and bar charts effectively
- **Slicer Integration:** Connected all visuals so filtering one affects the entire dashboard
- **User Experience:** Added interactive buttons for switching between different charts

**Data Modeling & Relationships**
- **Multi-Table Structure:** Connected 5 different data tables properly
- **Star Schema Design:** Organized data with fact tables and dimension tables
- **Relationship Building:** Created logical connections between tables using keys
- **Date Intelligence:** Built a calendar table for time-based analysis
- **Data Quality:** Ensured clean, consistent data across all tables

## Data Model Structure
![Data Model](https://github.com/nidhip1/PowerBI-Sales-Performance-Dashboard/blob/main/Data_Model.png)

### Main Tables & How They Connect:
1. **FTSales(Fact Table)**- The main sales data containing: 
- Sales amounts, costs, and profit information
- Order details and customer information
- Links to all other tables through ID fields
2. **DimProducts**- Product information including:
- Product names
- Product costs and pricing
- Connected to sales through Product ID
3. **DimFactories**- Factory location data:
- Factory locations and coordinates
- Linked to products to show where the candy is made
4. **DimTargets**- Sales target information:
- Target numbers for each division
- Used to compare actual vs. expected performance
5. **Calendar Table**-  Date information for time analysis:
- Months, quarters, years, and days details
- Enables time-based filtering and trends

### Key Relationships:
- **FTSales ↔ DimProducts:** Connected by Product ID (shows which products were sold)
- **FTSales ↔ DimTargets:** Connected by Division (compares actual vs. target sales)
- **FTSales ↔ Calendar:** Connected by Order Date (enables time-based analysis)
- **DimProducts ↔ DimFactories:** Connected by Factory (shows product origins)

## What I Analyzed
**Main Business Numbers**
- **Total Sales:** $141.8K across all products
- **Gross Profit:** $93.4K with healthy 65.9% profit margin
- **Order Volume:** 9K total orders processed
- **Average Order:** $16.6 per order
- **Time Period:** 4 years of sales data (2021-2024)

**Product Performance**
- **Top Performers:** Wonka Bar products dominate sales
- **Category Analysis:** Chocolate products significantly outperform targets (37K vs 27K target)
- **Underperformers:** Sugar-based products consistently miss targets
- **Profit Leaders:** Triple Dazzle Caramel and Scrumpdiddlyumptious lead profitability

## Dashboard Features & What You Can See
1. **Executive Summary (Top Cards)**
- Shows the 5 most important business numbers at a glance
- Includes month-over-month change indicators
- Colour-coded to show positive (green) and negative (red) trends
2. **Time-Based Analysis**
- **Monthly Profit Trends:** Line chart showing profit patterns throughout the year
- **Seasonal Insights:** September shows consistent profit peaks
- **Growth Tracking:** Monitors performance changes over time
3. **Product Performance Analysis**
- **Profitability vs. Volume** Scatter plot showing which products are both popular AND profitable
- **Interactive Switching:** Special feature with buttons to switch between two different visuals (Orders by Country/Region and Shipping Mode)
-  **Bubble Chart:** Size represents sales volume, position shows profitability
4. **Target vs. Actual Comparison**
- **Division Performance:** Bar charts comparing planned vs. actual sales
- **Performance Gaps:** Clearly shows which areas exceed or miss targets
- **Visual Indicators:** Easy-to-spot over/under performance
5. **Shipping & Operations**
- **Shipping Mode Preferences:** Standard Class dominates customer preferences (5.1K orders)
- **Operational Insights:** Helps optimize shipping and delivery strategies
6. Detailed Product Analysis (Page 2)
- **Complete Product List:** Every Treat Link candy product with sales and profit details
- **Sales Attainment:** Percentage showing how each product performs against goals
- **Key Takeaways Panel:** Strategic recommendations specifically for Treat Link's operations

## Special Interactive Features
### Dynamic Visual Switching
- **Bottom Right Corner:** Two buttons that let users switch between different chart views
- **Seamless Transition:** Click buttons to see the same data in different visual formats
- **User Control:** Gives viewers choice in how they want to see the information
### Smart Filtering
- **Year Filter:** Dropdown to analyze specific years or all years combined
- **Quarter Filter:** Focus on seasonal performance
- **Division Filter:** Deep-dive into specific business divisions
- **Connected Visuals:** All charts update together when filters change

## Skills I Showed
- **Power BI Mastery:** Advanced dashboard creation with professional design
- **Data Modeling:** Proper table relationships and data structure
- **DAX Formulas:** Custom calculations for business metrics
- **Visual Design:** Clean, professional layout that's easy to understand
- **User Experience:** Interactive features that make exploration intuitive
- **Business Analysis:** Turning data into actionable business insights
- **Storytelling:** Presenting data in a way that tells a clear business story

## Key Findings
### What I Discovered
- **Seasonal Patterns:** September consistently shows the highest profits
- **Product Success:** Wonka Bar products are clear winners in both sales and profit
- **Division Performance:** The Chocolate division exceeds targets, while the Sugar division struggles
- **Customer Preferences:** 5.1K customers prefer Standard Class shipping
- **Profit Health:** Strong 65.9% overall profit margin indicates a healthy business
- **Growth Opportunity:** Treat Link's Sugar products need strategic review and repositioning

## Project Structure
```
TreatLinkSalesAnalytics/
├── Dashboard Pages/
│   ├── Overview (Main KPI dashboard)
│   └── Product Details (Detailed analysis)
├── Data Model/
│   ├── FTSales (Main sales fact table)
│   ├── DimProducts (Product master data)
│   ├── DimFactories (Location data)
│   ├── DimTargets (Sales targets)
│   └── Calendar (Date dimension)
├── DAX Measures/
│   ├── Profit calculations
│   ├── Growth rate formulas
│   └── Target comparison metrics
└── Visualizations/
    ├── Interactive charts
    ├── KPI cards
    └── Custom buttons
```
## Tools I Used
- **Microsoft Power BI Desktop:** Main dashboard creation tool
- **DAX (Data Analysis Expressions):** Custom formulas and calculations
- **Power Query:** Data cleaning and transformation
- **Data Modeling:** Relationship building and table connections
