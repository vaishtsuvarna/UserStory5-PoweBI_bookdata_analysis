# Book Data Analysis Dashboard - Power BI

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Version](https://img.shields.io/badge/Version-v1.0-blue)
![Dataset](https://img.shields.io/badge/Data-999%20Books-orange)
![Tool](https://img.shields.io/badge/Tool-PowerBI-yellow)

🌟 Overview
Interactive Power BI dashboard built on scraped book data to analyze **price, ratings, and availability**.  
Supports **dynamic filtering, drill-down, and KPI insights**.

⚙️Features Implemented:
Data Integration
Imported books_data.csv (999 books)

Data types: Price (decimal), Rating (integer), Availability (text)

Cleaning: Removed duplicates, trimmed whitespace, handled nulls

📊Charts and Visualizations
Bar chart: Average price by rating
Pie chart: In Stock vs Out of Stock proportion
Table: All books with conditional formatting (high price > $60 red, low ratings blue)
Clustered bar: Price category analysis
Decomposition Tree: Availability → Rating → Price Category
Scatter Plot: Price vs Rating distribution

Interactive Elements
Slicers: Rating (1-5), Stock Availability, Price Range
Drill-through from category to individual books
Dynamic updates across all visuals
Data Processing
GBP to USD conversion (1.32 exchange rate)

Price categories:
Budget: under $30
Standard: $30-$60
Premium: above $60

KPI Cards
Total Books count
Average Price (USD)
Percentage In Stock

project/
├── powerbi/
│   └── Book_Analysis_Dashboard.pbix
├── scraper.py
├── books_data.csv
└── README.md

🧪 Testing:
All acceptance criteria validated through 6 test cases:
✅ CSV import successful
✅ Data types correctly assigned
✅ Filtering works properly
✅ Calculations verified
✅ Visuals update dynamically
✅ No formatting or data errors

📈Key Insights:
Average price ~$46 USD across all ratings
Standard category: 45% of inventory
89% books in stock
No price-rating correlation

▶️Usage:
Open Book_Analysis_Dashboard.pbix in Power BI Desktop
Use slicers to filter data
Right-click table for drill-through
Export as PDF/PowerPoint if needed

🧾Requirements:
Power BI Desktop
books_data.csv (from scraper.py)

🎯 Final Result
✅ All User Story acceptance criteria implemented
✅ Fully interactive dashboard
✅ Clean and validated dataset
✅ Production-ready Power BI report
