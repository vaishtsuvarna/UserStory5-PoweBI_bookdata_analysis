#Book Data Analysis Dashboard - Power BI
Power BI dashboard visualizing scraped book data from BooksToScrape.com. Analyzes pricing trends, ratings distribution, and stock availability across 999 books.

Features Implemented:
Data Integration
Imported books_data.csv (999 books)

Data types: Price (decimal), Rating (integer), Availability (text)

Cleaning: Removed duplicates, trimmed whitespace, handled nulls

Charts and Visualizations
Bar chart: Average price by rating

Pie chart: In Stock vs Out of Stock proportion

Table: All books with conditional formatting (high price > $66 red, low ratings blue)
Clustered bar: Price category analysis
Decomposition Tree: Availability → Rating → Price Category
Scatter Plot: Price vs Rating distribution

]]Interactive Elements
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

File Structure
text
project/
├── powerbi/
│   └── Book_Analysis_Dashboard.pbix
├── scraper.py
├── books_data.csv
└── README.md
Key DAX Formulas

Testing Results
All 6 test cases passed:
CSV import successful (999 rows)
Data types correct
Filtering functional
Calculations accurate
Slicers update visuals
No formatting errors

Key Insights
Average price ~$46 USD across all ratings
Standard category: 45% of inventory
89% books in stock
No price-rating correlation

Usage
Open Book_Analysis_Dashboard.pbix in Power BI Desktop
Use slicers to filter data
Right-click table for drill-through
Export as PDF/PowerPoint if needed

Requirements:
Power BI Desktop
books_data.csv (from scraper.py)

Results
- All 6 test cases passed
-All User Story 5 acceptance criteria implemented and tested.
