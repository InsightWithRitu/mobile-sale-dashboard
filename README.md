# 📊 Mobile Sales Performance Dashboard

## 🧾 Overview  
This Power BI project visualizes **mobile sales performance** across various brands, models, cities, and payment methods.  
It provides actionable insights through **interactive dashboards**, enabling users to compare **current metrics**, **month-to-date (MTD)** progress, and **same period last year (SPLY)** trends for informed decision-making.

---

## 🚀 Features

### 🏠 Main Dashboard
- 📈 **KPIs Overview:**  
  - Total Sales  
  - Total Quantity Sold  
  - Total Transactions  
  - Average Price  
- 🗺️ **Sales by City** (Geographical Map)
- 📅 **Total Quantity by Month** (Trend Line)
- 🏷️ **Brand-wise and Model-wise Sales**
- 💳 **Payment Method Distribution**
- ⭐ **Customer Ratings Breakdown**
- 📊 **Interactive Filters:**  
  - Mobile Model  
  - Payment Method  
  - Brand  

---

### 📅 MTD (Month-To-Date) Report

- Tracks **daily cumulative performance** throughout the month.  
- Shows **growth trends** for Total Sales and Quantity.  
- Compares performance across **Year, Quarter, Month, and Day**.  
- KPIs:  
  - Total Sales  
  - Total Quantity  
  - Transactions  
  - Average Price  

---

### 🔁 Same Period Last Year (SPLY) Comparison


- Year-over-Year (YoY) comparison for:
  - Total Sales vs. SPLY  
  - Quarter-wise and Month-wise performance  
- Highlights growth or decline in key metrics.  
- Ideal for evaluating yearly performance trends.

---

## 📍 Key Insights
- 🏙️ Identify **top-performing cities** and regions.  
- 💼 Discover **best-selling brands and models**.  
- 💳 Analyze **payment preferences** (UPI, Card, Cash, etc.).  
- 🌟 Track **customer satisfaction levels** through ratings.  
- 📊 Understand **sales growth patterns** by month, quarter, and year.

---

## 🧩 Tools & Technologies Used
| Category | Tools |
|-----------|--------|
| Data Visualization | Power BI Desktop |
| Data Source | CSV / Excel (Mobile Sales Data) |
| Languages | DAX, Power Query (M) |
| Charts Used | Map, Line, Bar, Donut, KPI Cards |
| Features | Dynamic Filters, MTD, SPLY, YoY Analysis |

---

## 🧮 DAX Measures (Examples)
```DAX
Total Sales = SUM(Sales[Amount])

Total Quantity = SUM(Sales[Quantity])

Average Price = DIVIDE([Total Sales], [Total Quantity])

MTD Sales = TOTALMTD([Total Sales], 'Date'[Date])

SPLY Sales = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))

