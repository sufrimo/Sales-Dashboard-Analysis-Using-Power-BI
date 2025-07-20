# Sales Dashboard Analysis Using Power BI

---

## 1. Introduction

In retail and e-commerce, understanding sales performance across products, regions, and time periods is essential for strategic planning and operational effectiveness. This project presents an automated Power BI sales dashboard that processes raw data from multiple Excel files, enabling interactive reporting and detailed sales analysis. The dashboard helps business users monitor KPIs, identify trends, and make data-driven decisions.

---

## 2. Description of Project

The project uses 12 Excel files downloaded from Shopee, stored in a designated folder. Power BI’s Power Query is used to load and transform the data. This process includes merging tables, changing data formats, and creating calculated columns.

The resulting data model supports interactive analysis using charts and filters. Users can explore sales data by month, day, and hour, evaluate regional performance, and identify top-selling products.

---

## 3. Objective

The Power BI sales dashboard is designed to:

1. Track and visualize total sales performance  
2. Identify top-selling products for timely restocking or replenishment  
3. Analyze monthly, daily, and hourly sales trends to support marketing decisions, such as the timing of advertising and promotions  
4. Evaluate regional sales distribution to assist with location-based ad targeting and budget allocation  
5. Monitor key performance indicators (KPIs) using visual tools such as charts, cards, gauges, slicers, and filters  
6. Assess shipping and item preparation performance to improve order fulfillment and customer satisfaction  

---

## 4. Scope and Limitations

### Scope

- Utilizes Power Query for automatic integration of monthly data across the year  
- Focuses on key metrics such as total sales, order count, order volume, product performance, regional performance, and seller fulfillment performance  
- Employs Power BI visuals and DAX formulas to enhance interactivity and reporting functionality  

### Limitations

- Dataset is static and sourced from Shopee exports; not connected to a live or real-time system  
- Covers only one year of data, based on 12 Excel files (one per month)  
- Designed for small to medium datasets  

---

## 5. Methodology

### Data Extraction

- Sales data is extracted monthly from Shopee exports.  
- The January file is imported into Power BI using Power Query as a sample for schema definition.  
- The remaining 11 monthly files are integrated automatically through folder-based loading and do not require manual import.  

### Data Preparation (ETL) in Power Query

- Sales data containing long product titles is merged with metadata tables for improved readability.  
- Data types are corrected, and formats are standardized across all columns.  
- Calculated columns are added, including metrics such as profit, sales amount, and processing time difference.  
- Additional time-based columns (e.g., month, day) are extracted from the date field for trend analysis.  

### Data Modeling with DAX

Key DAX measures and functions used include:

- `SUMX` – to calculate total revenue  
- `COUNT`, `DISTINCTCOUNT` – to track order quantities and unique values  
- `CALCULATE`, `FILTER` – for dynamic filtering and conditional aggregations  
- `RANKX` – for ranking top products and high-performing regions  
- `MIN`, `MAX`, `AVERAGE` – for performance metrics  

### Reporting and Visualization

The dashboard includes a variety of visuals to support interactive analysis:

- **Map** – Displays sales by region  
- **Pie Chart** – Shows distribution by location  
- **Area Chart** – Visualizes daily and hourly sales trends  
- **Clustered Column Chart** – Highlights monthly sales patterns  
- **Card** – Displays KPIs such as total sales, total orders, and number of products sold  
- **Gauge** – Indicates seller fulfillment performance  
- **Slicer** – Filters data by month  
- **Bookmark** – Switches between daily and hourly views for time-based analysis  

---


## 6. Full Sales Dashboard 

![Sales Dashboard Preview](https://github.com/sufrimo/Sales-Dashboard-Analysis-Using-Power-BI/blob/main/DASHBOARD.jpg)

---


## 7. Techniques Used

- **Power Query** – Used for folder-based data import, data cleaning, table merging, and transformation  
- **Calculated Columns** – Created in Power Query and DAX to derive additional fields such as month numbering, sales amount, and time difference  
- **DAX Functions** – Applied for custom calculations and measures, including:  
  - `SUMX` – total revenue  
  - `CALCULATE`, `FILTER` – dynamic aggregations  
  - `RANKX` – ranking of products and regions  
  - `COUNT`, `DISTINCTCOUNT`, `MIN`, `MAX`, `AVERAGE` – for various KPIs  
- **Power BI Visuals** – Includes cards, gauges, maps, area charts, clustered column charts, and pie charts  
- **Slicers & Bookmarks** – Enables interactivity and allows users to filter data and switch between views  

---

## 8. Key Findings

- 💰 **Total Sales:** ₱1.78M over 12 months  
- 🎯 **Quantity Sold:** 5,994 units  
- 📦 **Top 3 Products:**  
  1. Rockbros Bike Arm Sleeves  
  2. Reumafonds Bike Patch Kit  
  3. Giyo Bike Pump  
- 🌍 **Top Region:** Metro Manila (49.85% of total sales)  
- 📊 **Monthly Trend:** Sales were low in November–December (as buyers allocated budgets for upcoming holiday expenses), with a further dip in January–February during post-holiday consumer recovery  
- 🏆 **Best Performing Month:** August (due to restocking of high-value preorder Bike Trainer)  
- 📈 **Daily Trend:** Strong during the 1st–15th of the month, peaking on the 15th due to mid-month platform promotions  
- 🕒 **Hourly Trend:** Lowest sales between 1 AM–dawn, rising in the morning, medium-high during business hours (10 AM–5 PM), and high into late evening  

---

## 9. Recommendations

### 📦 Inventory Management (November–February)

- Implement reduced stock thresholds for non-holiday products during November–December and January–February to minimize inventory holding costs and free up working capital during slow demand periods.

### 📺 Advertising Strategy (6 PM–10 PM)

- Schedule digital advertising campaigns between 6 PM and 12 PM, when online shopping activity is highest in the Philippines.

### 📦 Product Spotlighting During Lean Months

- Feature top three products online during November to February. Emphasize these proven sellers through banners, product spotlights, or bundled offers to maintain visibility and sales momentum in low-demand periods.

### 🎯 Targeted Regional Advertising Strategy

- Implement region-specific advertising campaigns targeting high-performing areas such as Metro Manila, Laguna, Rizal, Bulacan, Cavite, Pampanga, Cebu, Iloilo, Davao del Sur, and Negros Occidental. These regions have demonstrated significant online shopping activity, making them prime markets for your products.

---


