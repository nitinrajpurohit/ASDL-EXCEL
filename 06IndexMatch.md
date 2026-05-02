# Excel INDEX-MATCH Tutorial

INDEX-MATCH is a powerful lookup combination in Excel. It allows you to find data in a table **in any direction**, unlike VLOOKUP, and is more flexible with large datasets.

---

## 1. INDEX Function

**Purpose:** Returns the value of a cell at a given row and column in a range.

**Syntax:**
```excel
INDEX(array, row_num, [column_num])
```

- `array` → The range to look in  
- `row_num` → Row number in the array  
- `column_num` → Column number (optional if single column)  

**Example:**
```excel
=INDEX(B2:B6, 3)
```
Returns the **3rd value** in the range `B2:B6`.

---

## 2. MATCH Function

**Purpose:** Returns the position of a value in a range.

**Syntax:**
```excel
MATCH(lookup_value, lookup_array, [match_type])
```

- `lookup_value` → Value you want to find  
- `lookup_array` → Range to search  
- `match_type` → 0 for exact match (recommended), 1 for less than, -1 for greater than  

**Example:**
```excel
=MATCH("Charlie", B2:B6, 0)
```
Returns **3** if "Charlie" is the 3rd item in `B2:B6`.

---

## 3. Combining INDEX and MATCH

**Purpose:** Look up a value in any column based on another column.

**Syntax:**
```excel
INDEX(return_range, MATCH(lookup_value, lookup_range, 0))
```

**Example Dataset:**

| ID   | Name    | Department | Salary |
|------|---------|-----------|--------|
| E101 | Alice   | HR        | 50000  |
| E102 | Bob     | IT        | 60000  |
| E103 | Charlie | Finance   | 55000  |
| E104 | Diana   | IT        | 70000  |
| E105 | Edward  | HR        | 65000  |

**Task:** Find **Charlie’s Salary**

**Formula:**
```excel
=INDEX(D2:D6, MATCH("Charlie", B2:B6, 0))
```

**Step-by-step Logic:**

1. `MATCH("Charlie", B2:B6, 0)` → Charlie is in **row 3** of the Name column.  
2. `INDEX(D2:D6, 3)` → Returns the 3rd value in Salary column → **55000**

---

## 4. Advantages of INDEX-MATCH over VLOOKUP

- Can look **left** (VLOOKUP can’t)  
- Doesn’t break if columns are inserted or deleted  
- More efficient on large datasets  
- Can handle dynamic ranges better  

---

## 5. Tips

- Always use `0` for exact match in MATCH  
- INDEX-MATCH can replace VLOOKUP in almost all situations  
- Can be combined with other functions like `IFERROR` for error handling  

---

## 6. Practice Exercises

Use the dataset below:

| ID   | Name    | Department | Salary |
|------|---------|-----------|--------|
| E101 | Alice   | HR        | 50000  |
| E102 | Bob     | IT        | 60000  |
| E103 | Charlie | Finance   | 55000  |
| E104 | Diana   | IT        | 70000  |
| E105 | Edward  | HR        | 65000  |

**Tasks:**

1. Find **Bob’s Salary**  
2. Find **Diana’s Department**  
3. Find **ID of Edward**  
4. Find **Salary of the employee in row 4**  
5. Find **Name of the employee with Salary 55000**  

**Example Solution for Task 1:**
```excel
=INDEX(D2:D6, MATCH("Bob", B2:B6, 0))
```

---

## 7. Optional Advanced Tasks

1. Combine with `IFERROR` to avoid errors if value not found:
```excel
=IFERROR(INDEX(D2:D6, MATCH("Zack", B2:B6, 0)), "Not Found")
```

2. Horizontal Lookup: Find Department by Salary using MATCH across a row:
```excel
=INDEX(B1:E1, MATCH(55000, B2:E2, 0))
```

---

## 8. Summary

- `INDEX` → Returns a value based on row/column  
- `MATCH` → Finds position of a value  
- `INDEX-MATCH` → Flexible lookup in any direction  
- Preferred over VLOOKUP for robust, scalable Excel models
