## Session 6 (2 Hours) – Lookup Functions & Cell References

---

### Session Objective
By the end of this session, students will be able to:
- Understand how Excel connects data across tables
- Use lookup functions to fetch values automatically
- Apply correct cell references for scalable formulas
- Handle common lookup errors professionally

---

## 1. Cell References (Foundation for Lookups)

### Types of Cell References
- **Relative Reference**  
  - Example: `A1`  
  - Changes automatically when copied

- **Absolute Reference**  
  - Example: `$A$1`  
  - Remains fixed when copied

- **Mixed Reference**  
  - Examples: `A$1`, `$A1`  
  - Used when either row or column must stay fixed

### Why Cell References Matter
- Prevent formula breakage when copying
- Essential for lookup tables
- Common interview question

### Trainer Demonstration
- Copy a formula with and without `$`
- Show incorrect vs correct results

---

## 2. VLOOKUP Function

### What is VLOOKUP?
Used to search a value in the **first column** of a table and return a related value from another column.

### Syntax
```
=VLOOKUP(lookup_value, table_array, col_index_number, FALSE)
```


### Explanation of Arguments
- `lookup_value` – Value to search (e.g., Employee ID)
- `table_array` – Data table (use absolute reference)
- `col_index_number` – Column number to return data from
- `FALSE` – Exact match (mandatory for accuracy)

### Key Rules
- Lookup value must be in the first column
- Column index must be a number
- Always use `FALSE` for exact match

---

## 3. HLOOKUP Function

### What is HLOOKUP?
Used when data is arranged **horizontally** (row-wise).

### Syntax
```
=HLOOKUP(lookup_value, table_array, row_index_number, FALSE)
```

### Difference Between VLOOKUP and HLOOKUP
- VLOOKUP → Vertical data (columns)
- HLOOKUP → Horizontal data (rows)

---

## 4. XLOOKUP Function (Modern Excel)

### Why XLOOKUP?
- Replaces VLOOKUP and HLOOKUP
- Supports left-to-right and right-to-left lookup
- No column index number needed

### Syntax
```
=XLOOKUP(lookup_value, lookup_array, return_array)
```


### Advantages
- More flexible
- Easier to understand
- Fewer errors
- Preferred in modern Excel interviews

---

## 5. Error Handling with Lookups

### Common Lookup Errors
- `#N/A` – Value not found
- `#VALUE!` – Wrong data type
- `#REF!` – Incorrect range

### Using IFERROR
```
=IFERROR(VLOOKUP(...), "Not Found")

```



### Why IFERROR is Important
- Makes reports professional
- Avoids confusion for users
- Frequently asked in interviews

---

## Student Practice Tasks

1. Employee Table
   - Use Employee ID to fetch:
     - Name
     - Department
     - Salary

2. Product Price List
   - Fetch product price using Product Code
   - Apply IFERROR for missing products

3. Reference Practice
   - Convert lookup table ranges into absolute references
   - Copy formulas correctly

---

## Trainer Tips
- Emphasize use of `$` in table ranges
- Explain lookup logic before syntax
- Compare VLOOKUP vs XLOOKUP clearly
- Relate examples to real office scenarios (HR, Sales, Inventory)

---

## Session Outcome
- Students can confidently use lookup functions
- Understand when and how to lock cell references
- Can answer lookup-related interview questions
- Ready to use lookups in real-world Excel tasks
