#  Lecture: CONCAT / CONCATENATE & Text Functions in Excel

**Functions Covered:**
CONCAT, CONCATENATE
LEFT, RIGHT, MID, LEN
TRIM, PROPER, UPPER, LOWER


---

##  Learning Objectives


* Combine text from multiple cells
* Extract text from left, right, and middle
* Calculate text length
* Remove unwanted spaces
* Change text case
* Clean real-world messy data

---

##  1. CONCAT / CONCATENATE

### Purpose

Used to **join text from multiple cells** into one.

### Syntax

```excel
=CONCAT(text1, text2, ...)
=CONCATENATE(text1, text2, ...)
```

### Dataset

| First Name | Last Name | Full Name |
| ---------- | --------- | --------- |
| Aman       | Sharma    |           |
| Neha       | Verma     |           |
| Rohit      | Mehta     |           |

### Task 1

Combine **First Name** and **Last Name** with a space in between.

---

##  2. LEFT Function

### Syntax

```excel
=LEFT(text, number_of_characters)
```

### Dataset

| Employee Code | Extracted Code |
| ------------- | -------------- |
| EMP1023       |                |
| EMP2045       |                |

### Task 2

Extract the first **3 characters** from Employee Code.

---

##  3. RIGHT Function

### Syntax

```excel
=RIGHT(text, number_of_characters)
```

### Dataset

| Mobile Number | Last 4 Digits |
| ------------- | ------------- |
| 9876543210    |               |
| 9123456780    |               |

### Task 3

Extract the **last 4 digits** of the mobile number.

---

##  4. MID Function

### Syntax

```excel
=MID(text, start_position, number_of_characters)
```

### Dataset

| Product Code | Product Number |
| ------------ | -------------- |
| PRD-4589-IN  |                |
| PRD-7821-US  |                |

### Task 4

Extract the **4-digit product number** from the code.

---

##  5. LEN Function

### Syntax

```excel
=LEN(text)
```

### Dataset

| Text           | Length |
| -------------- | ------ |
| Excel Training |        |
| Data Analysis  |        |

### Task 5

Find the **total number of characters** in each text.

---

##  6. TRIM Function

### Purpose

Removes **extra spaces** from text.

### Syntax

```excel
=TRIM(text)
```

### Dataset

| Raw Text       | Clean Text |
| -------------- | ---------- |
| Aman   Sharma  |            |
| Excel   Course |            |

### Task 6

Remove extra spaces and clean the text.

---

##  7. PROPER Function

### Syntax

```excel
=PROPER(text)
```

### Dataset

| Raw Name    | Proper Case |
| ----------- | ----------- |
| aMAN shARMa |             |
| nEHa veRMa  |             |

### Task 7

Convert names into **Proper Case**.

---

##  8. UPPER Function

### Syntax

```excel
=UPPER(text)
```

### Dataset

| Text           | Upper Case |
| -------------- | ---------- |
| excel training |            |
| data cleaning  |            |

### Task 8

Convert text to **UPPERCASE**.

---

##  9. LOWER Function

### Syntax

```excel
=LOWER(text)
```

### Dataset

| Text          | Lower Case |
| ------------- | ---------- |
| EXCEL COURSE  |            |
| DATA ANALYSIS |            |

### Task 9

Convert text to **lowercase**.

---

##  10. Hands-on: Clean & Split Email Data

### Dataset

| Raw Email                                               |
| ------------------------------------------------------- |
| [aman.sharma@gmail.com](mailto:aman.sharma@gmail.com)   |
| [neha_verma@company.com](mailto:neha_verma@company.com) |
| [rohit.mehta@office.in](mailto:rohit.mehta@office.in)   |

### Tasks

* Remove extra spaces using TRIM
* Extract **username** using LEFT / MID
* Extract **domain name**
* Convert username into PROPER case

### Final Output Format

| Email | Username | Domain | Proper Name |
| ----- | -------- | ------ | ----------- |
|       |          |        |             |

---

##  Summary

* Text functions are heavily used in **HR, CRM, Marketing, and Data Cleaning**
* These functions improve **data accuracy and presentation**
* Mastery of text functions saves **manual effort**

---

##  Practice Assignment

1. Clean 10 messy names
2. Create Full Name from First & Last Name
3. Extract country code from phone numbers
4. Convert email usernames into Proper Case

---

##  End of Lecture
