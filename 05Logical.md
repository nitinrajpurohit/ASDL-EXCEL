#  Lecture : Logical Formulas in Excel

##  Lecture Objective

- Understand logical formulas in Excel
- Apply IF, AND, OR, NOT, and IFERROR functions
- Use logical formulas for decision-making tasks

---

##  Introduction to Logical Formulas

Logical formulas help Excel make decisions based on conditions.  
They return values like:
- TRUE / FALSE  
- Pass / Fail  
- Yes / No  

Logical formulas are commonly used in:
- Result calculation  
- Eligibility checks  
- Grading systems  
- Error handling  

---

##  IF Function

### Definition
The IF function checks a condition and returns:
- One value if the condition is TRUE
- Another value if the condition is FALSE

### Syntax
=IF(condition, value_if_true, value_if_false)

---

### Dataset: Student Result

| Roll No | Name | Marks | Result |
|--------|------|-------|--------|
| 1 | Aman | 75 | |
| 2 | Bharti | 38 | |
| 3 | Rohan | 60 | |
| 4 | Deepa | 29 | |
| 5 | Farhan | 82 | |

### Activity
- If Marks ≥ 40 → Pass  
- Else → Fail  

---

##  AND Function

### Definition
The AND function checks multiple conditions.  
It returns TRUE only if **all conditions are TRUE**.

### Syntax
=AND(condition1, condition2)

---

### Dataset: Eligibility Check

| Name | Age | Experience (Years) | Eligibility |
|------|-----|-------------------|-------------|
| Rohit | 25 | 2 | |
| Simran | 19 | 1 | |
| Vijay | 30 | 5 | |
| Nisha | 22 | 0 | |

### Activity
Eligible if:
- Age ≥ 21  
- Experience ≥ 1 year  

---

##  OR Function

### Definition
The OR function returns TRUE if **any one condition is TRUE**.

### Syntax
=OR(condition1, condition2)

---

### Dataset: Discount Eligibility

| Customer | Purchase Amount | Membership | Discount |
|---------|-----------------|------------|----------|
| A | 8000 | No | |
| B | 12000 | No | |
| C | 5000 | Yes | |
| D | 3000 | No | |

### Activity
Discount given if:
- Purchase Amount ≥ 10000  
- OR Membership = Yes  

---

##  NOT Function

### Definition
The NOT function reverses logical values.
- TRUE → FALSE  
- FALSE → TRUE  

### Syntax
=NOT(condition)

---

### Dataset: Attendance Status

| Name | Present | Status |
|------|---------|--------|
| Aman | TRUE | |
| Bharti | FALSE | |
| Rohan | TRUE | |
| Deepa | FALSE | |

### Activity
- If Present is FALSE → Absent  
- Else → Present  

---

##  IFERROR Function

### Definition
IFERROR handles errors such as:
- #DIV/0!
- #VALUE!

### Syntax
=IFERROR(formula, value_if_error)

---

### Dataset: Division Example

| Number 1 | Number 2 | Result |
|---------|----------|--------|
| 10 | 2 | |
| 15 | 0 | |
| 20 | 5 | |
| 8 | 0 | |

### Activity
- Divide Number 1 by Number 2  
- If error → display "Invalid"  

---

##  Introduction to Nested IF

### Definition
Nested IF means using one IF function inside another IF function.

---

### Dataset: Grading System

| Marks | Grade |
|-------|-------|
| ≥ 75 | A |
| ≥ 60 | B |
| ≥ 40 | C |
| < 40 | Fail |

### Activity
Assign grades based on marks using Nested IF.

---

##  Hands-on Practice

Students will:
1. Calculate Pass/Fail using IF  
2. Check eligibility using AND  
3. Apply discount logic using OR  
4. Mark attendance using NOT  
5. Handle errors using IFERROR  

---

##  Key Takeaways

- IF is the base of logical formulas  
- AND checks all conditions  
- OR checks any one condition  
- NOT reverses logic  
- IFERROR improves output quality  

---


##  End of Lecture
