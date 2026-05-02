# Microsoft Excel – Formatting & Data Types

---

## 1. Understanding Data Types

### 1.1 Text, Number & Date
- **Text:** Contains letters or alphanumeric characters. Excel treats these as labels, not numbers.  
  *Example:* `John`, `A12`  
  *Use case:* Names, IDs, descriptions.  

- **Number:** Numeric values that Excel can calculate with.  
  *Example:* `4500`, `23.5`  
  *Use case:* Sales amounts, scores, quantities.  

- **Date:** Special numeric type recognized by Excel for calculations and formatting.  
  *Example:* `28-Jan-2026`  
  *Use case:* Order dates, deadlines, timelines.  

> **Teaching Tip:** Show students how entering `"4500"` (with quotes) or pasting from a CSV can make a number become text, causing calculation errors.

### 1.2 Why Data Types Matter
- Formulas like `SUM`, `AVERAGE`, `MAX` work **only on numbers**  
- Text formatted numbers are **ignored** in calculations  
- Dates allow automatic calculations like adding days or finding difference between dates  

---

## 2. Formatting Numbers

### 2.1 Currency & Percentage
- **Currency:** Adds a symbol and formats decimals.  
  *Example:* ₹4500.00  
- **Percentage:** Multiplies number by 100 and adds `%`.  
  *Example:* 0.5 → 50%  

> **Tip:** Currency is critical in financial reports; percentage is useful for targets, growth rates, and KPIs.

### 2.2 General Number Formatting
- **General:** Default format when nothing is applied  
- **Number:** Allows decimal control and separators (commas)  
- **Date & Time:** Converts numeric date codes into readable formats  
  *Example:* `44568` → `28-Jan-2022`  

---

## 3. Text Formatting & Alignment

### 3.1 Basic Text Formatting
- Font style, size, and emphasis (Bold, Italic, Underline)  
- Font color for emphasis or categorization  
- Cell fill color to highlight important data  

### 3.2 Alignment & Orientation
- **Horizontal Alignment:** Left, Center, Right  
- **Vertical Alignment:** Top, Middle, Bottom  
- **Wrap Text:** Display long content in multiple lines within a cell  
- **Merge & Center:** Combine multiple cells for headings  

> **Tip:** Proper alignment makes large datasets readable and professional-looking.

---

## 4. Hidden Formula Logic

### 4.1 Why SUM Fails on Text Numbers
- Excel ignores numbers formatted as text when using `SUM` or other arithmetic formulas.  
- **Example:** `"4500"` + 5000 → only 5000 is counted  

**Fix Options:**  
1. `=VALUE(A2)` → converts text to number  
2. Paste Special → Multiply by 1 → bulk convert numbers  
3. Text to Columns → converts text numbers from CSV files  

> **Teaching Tip:** Show students how to identify text numbers quickly: select cells → look at alignment (text aligns left by default, numbers right).

---

## 5. Dataset for Practice

| Order ID | Sales Amount | Date       | Region    |
|----------|-------------|------------|-----------|
| O101     | 4500        | 01-Jan-26  | North     |
| O102     | "12000"     | 02-Jan-26  | East      |
| O103     | 8000        | 03-Jan-26  | West      |
| O104     | "25000"     | 04-Jan-26  | South     |
| O105     | 3000        | 05-Jan-26  | North     |
| O106     | "15000"     | 06-Jan-26  | East      |

> **Note:** Some numbers are stored as text (in quotes) to simulate real-world messy data.

---

## 6. Exercises

1. Identify the **data type** of each column (Text, Number, Date)  
2. Convert **text numbers** to numeric values using `=VALUE()` or Paste Special → Multiply  
3. Apply **Currency** formatting to Sales Amount column  
4. Apply **Percentage** formatting for target calculations  
5. Wrap text in the **Region** column  
6. Align numeric data to the right and headers to center  
7. Test formula `=SUM(B2:B7)` and observe errors caused by text numbers → fix them  

---

## 7. Hands-on Outcomes

After completing this session, students will be able to:  
- Identify and differentiate **Text, Number, and Date** in Excel  
- Apply **number formatting** such as Currency and Percentage  
- Use **text formatting and alignment** to improve readability and presentation  
- Detect and fix issues caused by **text numbers** in calculations  

---

