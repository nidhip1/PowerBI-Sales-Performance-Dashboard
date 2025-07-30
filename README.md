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

