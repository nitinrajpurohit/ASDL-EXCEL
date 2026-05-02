#  Sales Dataset Analysis Guide

**Dataset Headers:**  
`OrderID | ProductID | Region | Customer | Quantity | OrderDate | UnitPrice | Sales | Profit`

---

## 1️ Pivot Table Ideas & Corresponding Charts

### 1. Sales by Region
- **Pivot Table:**  
  - Rows → `Region`  
  - Values → `Sales` (Sum), `Profit` (Sum, optional)  
- **Charts to Make:**  
  - **Bar Chart** – Compare total sales across regions  
  - **Pie Chart** – Show % contribution of each region  

### 2. Sales by Product
- **Pivot Table:**  
  - Rows → `ProductID`  
  - Values → `Sales` & `Profit` (Sum), `Quantity` (optional)  
- **Charts to Make:**  
  - **Column Chart** – Compare product sales  
  - **Pie Chart** – Show sales distribution among top products  

### 3. Top Customers
- **Pivot Table:**  
  - Rows → `Customer`  
  - Values → `Sales` & `Profit` (Sum)  
  - Sort descending to find top 10 customers  
- **Charts to Make:**  
  - **Column Chart** – Top 10 customers by sales  
  - **Bar Chart** – Horizontal view if customer names are long  

### 4. Monthly Sales Trend
- **Pivot Table:**  
  - Rows → `OrderDate` (group by Month/Year)  
  - Values → `Sales` (Sum), `Profit` (optional)  
- **Charts to Make:**  
  - **Line Chart** – Show trend over months  
  - **Combo Chart** – Columns for Sales, Line for Profit  

### 5. Product Performance by Region (Advanced)
- **Pivot Table:**  
  - Rows → `Region`  
  - Columns → `ProductID`  
  - Values → `Sales` (Sum)  
- **Charts to Make:**  
  - **Stacked Column Chart** – See which products perform best in each region  

---



## 2 Dashboard Layout Ideas

- **Top Section (KPIs):**  
  - Total Sales, Total Profit, Average Profit Margin  

- **Left:**  
  - Sales by Region (**Bar + Pie Chart**)  

- **Right:**  
  - Top Customers (**Column Chart**)  

- **Middle:**  
  - Monthly Sales Trend (**Line / Combo Chart**)  

- **Bottom:**  
  - Product Performance by Region (**Stacked Column Chart**)  

- **Filters / Slicers:**  
  - Region, Product, Customer, Date  

---

## 3 Analysis Tips

1. **Conditional Formatting:** Highlight top/bottom performers in pivot tables (top 10 sales, negative profit).  
2. **Slicers:** Add slicers for Region, Product, or Customer to make dashboards interactive.  
3. **Filter by Date:** Compare month-over-month or year-over-year trends.  
4. **Data Cleanliness:** Remove duplicates, check for missing values in `Sales` or `Profit`.  
5. **KPIs:** Show Total Sales, Total Profit, Average Profit Margin as cards on the dashboard.  
