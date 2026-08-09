# 🏠 Real Estate Market Dashboard — CodeAlpha Power BI Internship

## 📌 Project Overview
This project is developed as part of the **CodeAlpha Power BI Virtual Internship**. The goal is to build an interactive dashboard analyzing real estate market dynamics to support investment and development decisions.

## 🎯 Objective
Build a dashboard to analyze real estate market dynamics for investment and development decisions.

## 🛠 Tools Used
- **Power BI Service** (app.powerbi.com)
- **Dataset:** USA Real Estate Dataset
- **DAX** for measures and calculations

## 📂 Dataset
The dataset used is the **USA Real Estate Dataset** (sourced from Kaggle), containing property-level data including price, bedrooms, bathrooms, acre lot, house size, city, state, and listing status.

## 📈 Key Features
- **KPI Cards:** Average Price, Total Listings, Average House Size, Price per Sqft
- **Market Hotspot Analysis:** Treemap of Average Price by State
- **State Comparison:** Bar chart of Average Price by State
- **Bedroom Analysis:** Average Price by number of Bedrooms
- **Listing Status Breakdown:** Total Listings by Status (For Sale, Sold, Ready to Build)

## 🧮 DAX Measures Used
```DAX
Average Price = AVERAGE('realtor-data zip'[price])
Median Price = MEDIAN('realtor-data zip'[price])
Total Listings = COUNTROWS('realtor-data zip')
Average House Size = AVERAGE('realtor-data zip'[house_size])
Price per Sqft = DIVIDE([Average Price], [Average House Size], 0)
Average Bedrooms = AVERAGE('realtor-data zip'[bed])
Average Acre Lot = AVERAGE('realtor-data zip'[acre_lot])
```

## 🖼 Dashboard Preview

### Page 1 — Overview & State-wise Analysis
![Overview Page](Page1_Overview.png)

### Page 2 — Bedrooms & Listing Status Analysis
![Bedrooms and Status Page](Page2_BedroomsStatus.png)

## 📌 Key Insights
- Identified states with the highest average property prices (market hotspots).
- Analyzed relationship between number of bedrooms and average price.
- Broke down listings by status to understand market activity (for sale, sold, ready to build).
- Calculated price per square foot as a value indicator across the market.

## 🎓 Internship
This project is submitted as part of the **CodeAlpha Power BI Internship Program**.

🔗 [CodeAlpha Website](https://www.codealpha.tech)
