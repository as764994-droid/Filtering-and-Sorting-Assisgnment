# SQL Filtering and Sorting Assignment - PwSkills

This repository contains the MySQL Workbench file for the Filtering and Sorting assignment from the Java + DSA course by PwSkills.

## Assignment Details

**Course:** Data Analytics with GenAI
**Topic:** Filtering and Sorting  
**Database Used:** MySQL Workbench

## Contents

This assignment covers the following SQL concepts:

- WHERE clause for filtering data
- OR and AND logical operators
- IN clause for multiple value matching
- BETWEEN operator for range queries
- LIKE operator with wildcards for pattern matching
- NOT operator for exclusion
- ORDER BY clause for sorting results
- Date functions (YEAR) for filtering

## Questions Covered

### Query Questions (Q1-Q8)

1. **OR Operator:** Show employees in 'IT' or 'HR' departments
2. **IN Clause:** Retrieve employees in 'Sales', 'IT', or 'Finance'
3. **BETWEEN Operator:** Display employees with salary between ₹50,000 and ₹70,000
4. **LIKE with Prefix:** List employees whose names start with 'A'
5. **LIKE with Substring:** Find employees whose names contain 'an'
6. **Combined Conditions:** Show employees from 'Delhi' or 'Mumbai' earning > ₹55,000
7. **NOT Operator:** Display all employees except those from 'HR'
8. **Date Filtering + Sorting:** Get employees hired between 2019-2022, ordered by HireDate

## MySQL Workbench File

**File Name:** `SQL_Filtering_Sorting_Assignment.mwb` (or your workbench file name)

### Workbench File Password
```
AyushSingh@1707
```

## How to Use

1. Clone this repository
2. Open MySQL Workbench
3. Open the `.mwb` file from this repository
4. When prompted, enter the password: `AyushSingh@1707`
5. Execute the CREATE TABLE and INSERT statements first
6. Run each query to see the filtered and sorted results

## Database Schema

### Employees Table
- `EmpID` (INT, PRIMARY KEY)
- `EmpName` (VARCHAR)
- `Department` (VARCHAR)
- `City` (VARCHAR)
- `Salary` (INT)
- `HireDate` (DATE)

### Sample Data (10 Records)
The table contains employee information including:
- 10 employees across different departments (Sales, HR, IT, Marketing, Finance)
- Multiple cities (Delhi, Mumbai, Bengaluru, Pune, Chennai, etc.)
- Salary range: ₹45,000 - ₹81,000
- Hire dates from 2018 to 2023

## SQL Operators Used

| Operator | Purpose | Example |
|----------|---------|---------|
| `OR` | Multiple conditions (any true) | `WHERE Dept = 'IT' OR Dept = 'HR'` |
| `AND` | Multiple conditions (all true) | `WHERE City = 'Delhi' AND Salary > 50000` |
| `IN` | Match any value in list | `WHERE Dept IN ('IT', 'HR')` |
| `BETWEEN` | Range query (inclusive) | `WHERE Salary BETWEEN 50000 AND 70000` |
| `LIKE` | Pattern matching | `WHERE Name LIKE 'A%'` |
| `NOT` | Negation/Exclusion | `WHERE NOT Dept = 'HR'` |
| `ORDER BY` | Sort results | `ORDER BY HireDate ASC` |

## LIKE Wildcard Patterns

- `'A%'` - Starts with 'A'
- `'%an%'` - Contains 'an' anywhere in the string
- `'%a'` - Ends with 'a'
- `'_a%'` - Second character is 'a'

## Author

**Ayush Singh**

## Course Information

**Provider:** PwSkills  
**Program:** Data Analytics with GenAI

---

*Note: This is an educational assignment. Practice writing queries yourself to better understand SQL filtering and sorting concepts.*
