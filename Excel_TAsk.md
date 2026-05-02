# Excel Advanced Assessment – 100 Marks

**Dataset:** `Excel_Advanced_Sales_Dataset_2000.csv`  
**Total Marks:** 100  
**Time:** 3 hours  

**Instructions:** Use the dataset to complete the tasks below. Use **formulas, formatting, pivot tables, Power Query, DAX/KPIs, charts, and dashboards** wherever required.

---

## Section 1: Data Cleaning & Formatting – 10 Marks
1. Apply **proper column headers formatting** (bold, center-aligned). (2 Marks)  
2. Format **Unit Price, Discount %, Total Sales** as **Currency**. (2 Marks)  
3. Format **Sales Date** in `DD-MMM-YYYY` format. (2 Marks)  
4. Highlight **Cancelled Orders** with **red fill** using conditional formatting. (2 Marks)  
5. Highlight **Total Sales > 1,00,000** in green using conditional formatting. (2 Marks)  

---

## Section 2: Formulas – 20 Marks
1. Create a column **Discount Amount** = `Quantity × Unit Price × Discount% / 100`. (5 Marks)  
2. Verify **Total Sales** = `Quantity × Unit Price – Discount Amount`. (5 Marks)  
3. Create **High Value Order** column: If Total Sales > 50,000 → “Yes”, else “No”. (5 Marks)  
4. Create **Delivery Status Check** column: If Delivery Status = “Pending” → “Follow-Up”, else “OK”. (5 Marks)  

---

## Section 3: Power Query / Data Transformation – 10 Marks
1. Load the dataset into **Power Query**.  
2. Remove duplicates based on **Order ID**.  
3. Split **Customer Name** into **First Name** and **Last Name**.  
4. Extract **Month** from **Sales Date**.  
5. Close & load the transformed data to Excel.  

---

## Section 4: Pivot Tables – 20 Marks
1. Create a pivot table showing **Total Sales by Region & Category**. (5 Marks)  
2. Create a pivot table showing **Average Quantity by Product Name**. (5 Marks)  
3. Count of **Cancelled Orders by Region**. (5 Marks)  
4. Top 5 **Customers by Total Sales** using pivot table. (5 Marks)  

---

## Section 5: Charts – 10 Marks
1. Create a **Column Chart** showing Total Sales per Region. (3 Marks)  
2. Create a **Pie Chart** showing Sales distribution by Category. (3 Marks)  
3. Create a **Line Chart** showing Total Sales trend by Month. (4 Marks)  

---

## Section 6: DAX Measures & KPI – 15 Marks
1. Create DAX measure **Total Revenue** = `SUM(Total Sales)`. (3 Marks)  
2. Create DAX measure **Average Order Value** = `AVERAGE(Total Sales)`. (3 Marks)  
3. Create DAX measure **High Value Orders Count** = `COUNTROWS(FILTER(Table, [Total Sales]>50000))`. (3 Marks)  
4. Create **KPI**: Target Revenue = 1,50,00,000; display actual vs target with indicator. (6 Marks)  

---

## Section 7: Dashboard – 15 Marks
1. Create a dashboard showing:  
   - Total Revenue (Card)  
   - Total Quantity Sold (Card)  
   - Total Sales by Region (Column/Bar Chart)  
   - Sales by Category (Pie/Donut Chart)  
   - Top 5 Customers (Table/Chart)  
   - Delivery Status Summary (Stacked Column / KPI)  
2. Make the dashboard **visually appealing** using colors, labels, and slicers for Region & Category.  

---

## Marking Scheme Summary

| Section                   | Marks |
|----------------------------|-------|
| Data Cleaning & Formatting | 10    |
| Formulas                   | 20    |
| Power Query                | 10    |
| Pivot Tables               | 20    |
| Charts                     | 10    |
| DAX Measures & KPI         | 15    |
| Dashboard                  | 15    |
| **Total**                  | 100   |

---

**Note:** Students are expected to demonstrate advanced Excel skills including formulas, formatting, data modeling, Power Query, DAX measures, pivot tables, charts, and dashboard creation.
