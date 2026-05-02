# Microsoft Excel – Basic Math & Counting Functions

---

## 1. Introduction to Math Functions

- Excel provides **predefined functions** to perform calculations quickly  
- These functions reduce manual errors and save time for large datasets  

### Key Points
- Functions always start with `=`  
- Parentheses `()` are used to pass **arguments** (cells or ranges)  
- Supports arithmetic, aggregation, and counting operations  

---

## 2. SUM Function

- **Purpose:** Adds a range of numbers  
- **Syntax:** `=SUM(number1, number2, …)` or `=SUM(B2:B7)`  
- **Example:** Add total marks or sales amounts  

> **Tip:** Always select the **range of cells**, not individual numbers, for efficiency  

---

## 3. AVERAGE Function

- **Purpose:** Calculates the mean of a range of numbers  
- **Syntax:** `=AVERAGE(B2:B7)`  
- **Use Case:** Find average sales, scores, or performance metrics  

---

## 4. MIN / MAX Functions

- **MIN:** Returns the smallest number in a range  
- **MAX:** Returns the largest number in a range  
- **Syntax:** `=MIN(B2:B7)` / `=MAX(B2:B7)`  
- **Use Case:** Identify top-performing student or highest/lowest sales  

---



## 5. COUNT Functions

- **COUNT:** Counts numeric cells in a range  
  - `=COUNT(B2:B7)`  
- **COUNTA:** Counts non-empty cells (numbers or text)  
  - `=COUNTA(A2:A7)`  
- **COUNTBLANK:** Counts empty cells  
  - `=COUNTBLANK(B2:B7)`  

> **Tip:** Use COUNT functions to quickly check dataset completeness  

---

## 6. Dataset for Practice

| Date       | Sales Amount | Region  | Units Sold |
|------------|-------------|--------|------------|
| 01-Jan-26  | 4500        | North  | 10         |
| 02-Jan-26  | 12000       | East   | 15         |
| 03-Jan-26  | 8000        | West   | 12         |
| 04-Jan-26  | 25000       | South  | 20         |
| 05-Jan-26  | 3000        | North  | 8          |
| 06-Jan-26  | 15000       | East   | 18         |

---

## 7. Exercises

1. **Calculate total sales** using `=SUM(B2:B7)`  
2. **Calculate average sales** using `=AVERAGE(B2:B7)`  
3. **Find the minimum and maximum units sold** using `=MIN(D2:D7)` / `=MAX(D2:D7)`  
5. **Count numeric cells** in Units Sold column using `=COUNT(D2:D7)`  
6. **Count non-empty cells** in Region column using `=COUNTA(C2:C7)`  
7. **Count blank cells** in Sales Amount column using `=COUNTBLANK(B2:B7)`  

---

## 8. Hands-on Outcomes

By the end of this session, students will be able to:  
- Use **SUM, AVERAGE, MIN, MAX** for basic calculations  
- Use **COUNT, COUNTA, COUNTBLANK** to analyze data completeness  
- Quickly summarize **daily transactions or student scores**  

---
