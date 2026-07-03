# SQL Multiple Choice Questions

---

# Set 1 – SQL Fundamentals

## Easy Level

### Q1. Which SQL statement is used to retrieve data from a database?

A. GET  
B. FETCH  
C. SELECT  
D. SHOW

---

### Q2. Which clause is used to filter rows in a SQL query?

A. ORDER BY  
B. WHERE  
C. GROUP BY  
D. HAVING

---

### Q3. Which keyword removes duplicate rows from the result?

A. UNIQUE  
B. DISTINCT  
C. DIFFERENT  
D. FILTER

---

### Q4. Which SQL command is used to add a new row into a table?

A. UPDATE  
B. INSERT INTO  
C. ADD ROW  
D. APPEND

---

### Q5. Which command is used to modify existing data in a table?

A. CHANGE  
B. ALTER  
C. UPDATE  
D. MODIFY

---

### Q6. Which SQL clause is used to sort the output?

A. SORT BY  
B. ORDER BY  
C. GROUP BY  
D. ARRANGE BY

---

### Q7. What does the following query return?

```sql
SELECT COUNT(*)
FROM Employees;
```

A. Number of columns  
B. Number of rows  
C. Sum of employee IDs  
D. Number of NULL values

---

### Q8. Which symbol is commonly used as a wildcard representing multiple characters?

A. *  
B. %  
C. _  
D. #

---

## Medium Level

### Q9. Consider the query:

```sql
SELECT *
FROM Employees
WHERE Salary > 50000;
```

Which employees are returned?

A. Salary less than 50000  
B. Salary equal to 50000  
C. Salary greater than 50000  
D. All employees

---

### Q10. Which query correctly selects employees whose name starts with `"A"`?

A.

```sql
WHERE Name = 'A%'
```

B.

```sql
WHERE Name LIKE 'A%'
```

C.

```sql
WHERE Name STARTS 'A'
```

D.

```sql
WHERE Name MATCH 'A%'
```

---

### Q11. What is the difference between `DELETE` and `TRUNCATE`?

A. No difference  
B. DELETE removes selected rows, TRUNCATE removes all rows  
C. TRUNCATE deletes one row at a time  
D. DELETE removes the table structure

---

### Q12. Which function returns the highest value?

A. MAX()  
B. TOP()  
C. HIGH()  
D. UPPER()

---

### Q13. Which clause is used to group rows having the same values?

A. ORDER BY  
B. GROUP BY  
C. SORT BY  
D. DISTINCT

---

### Q14. Which query returns employees working in either HR or Finance?

A.

```sql
WHERE Department = 'HR' OR 'Finance'
```

B.

```sql
WHERE Department IN ('HR', 'Finance')
```

C.

```sql
WHERE Department = HR, Finance
```

D.

```sql
WHERE Department LIKE HR|Finance
```

---

### Q15. Which SQL statement changes only the table structure?

A. UPDATE  
B. ALTER TABLE  
C. INSERT  
D. SELECT

---

### Q16. What will this query return?

```sql
SELECT AVG(Salary)
FROM Employees;
```

A. Total salary  
B. Average salary  
C. Maximum salary  
D. Number of employees

---

### Q17. Which condition checks for missing values?

A.

```sql
Salary = NULL
```

B.

```sql
Salary == NULL
```

C.

```sql
Salary IS NULL
```

D.

```sql
Salary EQUAL NULL
```

---

## Intermediate Level

### Q18. Which query finds the total salary department-wise?

A.

```sql
SELECT Department, SUM(Salary)
FROM Employees;
```

B.

```sql
SELECT Department, SUM(Salary)
FROM Employees
GROUP BY Department;
```

C.

```sql
SELECT SUM(Salary)
GROUP Department;
```

D.

```sql
SELECT Department
GROUP BY Salary;
```

---

### Q19. Consider the query:

```sql
SELECT Name
FROM Employees
ORDER BY Salary DESC;
```

Which employee appears first?

A. Lowest salary  
B. Random employee  
C. Highest salary  
D. Oldest employee

---

### Q20. What is the purpose of the `HAVING` clause?

A. Filters rows before grouping  
B. Filters grouped data after GROUP BY  
C. Sorts grouped data  
D. Removes duplicates

---

### Q21. Which query returns employees earning between 40,000 and 60,000 (inclusive)?

A.

```sql
WHERE Salary > 40000
AND Salary < 60000
```

B.

```sql
WHERE Salary BETWEEN 40000 AND 60000
```

C.

```sql
WHERE Salary = 40000 TO 60000
```

D.

```sql
WHERE Salary RANGE 40000,60000
```

---

### Q22. Which SQL function converts text to uppercase?

A. CAPITAL()  
B. UPPER()  
C. TOUPPER()  
D. UCASETEXT()

---

### Q23. Which query returns the first 5 rows in MySQL?

A.

```sql
SELECT FIRST 5 * FROM Employees;
```

B.

```sql
SELECT TOP 5 * FROM Employees;
```

C.

```sql
SELECT *
FROM Employees
LIMIT 5;
```

D.

```sql
SELECT * FIRST 5;
```

---

### Q24. Suppose the `Orders` table has 200 rows. What will this query return?

```sql
SELECT COUNT(OrderDate)
FROM Orders;
```

A. Always 200  
B. Number of non-NULL `OrderDate` values  
C. Number of unique dates  
D. Total columns

---

### Q25. Which statement about SQL is correct?

A. SQL is case-sensitive for keywords.  
B. SQL can only retrieve data.  
C. SQL can create, modify, retrieve, and delete data.  
D. SQL cannot create tables.

---

# Set 2 – Query Reasoning

> These questions focus on understanding SQL behavior rather than memorizing syntax.

### Q1

Given the table:

| EmpID | Name | Salary |
|------:|------|-------:|
| 1 | Alice | 50000 |
| 2 | Bob | NULL |
| 3 | Charlie | 70000 |

What is the output?

```sql
SELECT COUNT(Salary)
FROM Employees;
```

A. 3  
B. 2  
C. 1  
D. NULL

---

### Q2

Which query correctly returns departments having more than 5 employees?

A.

```sql
SELECT Department
FROM Employees
WHERE COUNT(*) > 5;
```

B.

```sql
SELECT Department
FROM Employees
GROUP BY Department
HAVING COUNT(*) > 5;
```

C.

```sql
SELECT Department
FROM Employees
HAVING COUNT(*) > 5;
```

D.

```sql
SELECT Department
WHERE COUNT(*) > 5
GROUP BY Department;
```

---

### Q3

Given:

```sql
SELECT *
FROM Employees
WHERE Salary > 50000
AND Department = 'IT'
OR Department = 'HR';
```

Which statement is correct?

A. Returns IT employees earning above 50000 only  
B. Returns all HR employees and IT employees earning above 50000  
C. Returns only HR employees earning above 50000  
D. Returns only employees earning above 50000

---

### Q4

Which statement about `NULL` is TRUE?

A. NULL is equal to 0.  
B. NULL is an empty string.  
C. NULL represents an unknown or missing value.  
D. NULL is treated as FALSE.

---

### Q5

Which query returns the second highest salary?

A.

```sql
SELECT MAX(Salary)
FROM Employees;
```

B.

```sql
SELECT MAX(Salary)
FROM Employees
WHERE Salary < (
    SELECT MAX(Salary)
    FROM Employees
);
```

C.

```sql
SELECT Salary
FROM Employees
ORDER BY Salary;
```

D.

```sql
SELECT MIN(Salary)
FROM Employees;
```

---

### Q6

Suppose the `Employees` table contains:

| Department | Salary |
|------------|-------:|
| IT | 50000 |
| IT | 70000 |
| HR | 60000 |
| HR | 55000 |

What is returned?

```sql
SELECT Department, AVG(Salary)
FROM Employees
GROUP BY Department;
```

A. One row  
B. Two rows  
C. Four rows  
D. Error

---

### Q7

Which clause executes last logically?

A. WHERE  
B. GROUP BY  
C. HAVING  
D. ORDER BY

---

### Q8

Which query is **INVALID**?

A.

```sql
SELECT *
FROM Employees
ORDER BY Salary DESC;
```

B.

```sql
SELECT Department, COUNT(*)
FROM Employees
GROUP BY Department;
```

C.

```sql
SELECT Department, Salary
FROM Employees
GROUP BY Department;
```

D.

```sql
SELECT Name
FROM Employees
WHERE Salary > 50000;
```

---

### Q9

Suppose:

**Employees**

| ID | Name |
|---:|------|
| 1 | Alice |
| 2 | Bob |

**Orders**

| OrderID | EmployeeID |
|--------:|-----------:|
| 101 | 1 |
| 102 | 1 |

Using:

```sql
SELECT *
FROM Employees
INNER JOIN Orders
ON Employees.ID = Orders.EmployeeID;
```

How many rows are returned?

A. 1  
B. 2  
C. 3  
D. 4

---

### Q10

Which JOIN returns all records from the left table, whether matching rows exist or not?

A. INNER JOIN  
B. RIGHT JOIN  
C. LEFT JOIN  
D. CROSS JOIN

---

### Q11

Which aggregate function ignores NULL values?

A. COUNT(column)  
B. SUM(column)  
C. AVG(column)  
D. All of the above

---

### Q12

What does this query return?

```sql
SELECT DISTINCT Department
FROM Employees;
```

A. Every department including duplicates  
B. Only unique department names  
C. First department only  
D. Departments sorted alphabetically

---

### Q13

Which query returns employees not working in Sales?

A.

```sql
WHERE Department != 'Sales'
```

B.

```sql
WHERE NOT Department = 'Sales'
```

C.

```sql
WHERE Department <> 'Sales'
```

D. All of the above (assuming the SQL dialect supports `!=`)

---

### Q14

Given:

```sql
SELECT *
FROM Employees
WHERE Salary IN (40000, 50000, 60000);
```

Which employee is returned?

A. Salary exactly equal to one of these values  
B. Salary greater than 40000  
C. Salary less than 60000  
D. Salary between 40000 and 60000

---

### Q15

Suppose the table contains:

| Salary |
|-------:|
| 50000 |
| 50000 |
| 70000 |

Result of:

```sql
SELECT COUNT(DISTINCT Salary)
FROM Employees;
```

A. 3  
B. 2  
C. 1  
D. Error

---

### Q16

Which statement best describes a Primary Key?

A. Can contain NULL  
B. Can contain duplicate values  
C. Must uniquely identify every row  
D. Can have duplicate NULL values

---

### Q17

Which statement about Foreign Keys is TRUE?

A. Must always be unique  
B. Can reference only a Primary Key (or another UNIQUE key) in another table  
C. Cannot contain NULL  
D. Automatically sorts data

---

### Q18

Consider:

```sql
SELECT *
FROM Employees
WHERE Salary > ALL (
    SELECT Salary
    FROM Managers
);
```

This returns employees whose salary is:

A. Greater than at least one manager  
B. Greater than every manager  
C. Equal to the highest manager salary  
D. Lower than every manager

---

### Q19

Which query returns departments whose average salary exceeds 60,000?

A.

```sql
SELECT Department
FROM Employees
WHERE AVG(Salary) > 60000;
```

B.

```sql
SELECT Department
FROM Employees
GROUP BY Department
HAVING AVG(Salary) > 60000;
```

C.

```sql
SELECT AVG(Salary)
WHERE Department;
```

D.

```sql
SELECT Department
HAVING AVG(Salary);
```

---

### Q20

Suppose:

```sql
SELECT *
FROM Employees
ORDER BY Salary ASC
LIMIT 3;
```

Returns:

A. Top 3 highest salaries  
B. Top 3 lowest salaries  
C. Random 3 employees  
D. Employees with salary = 3

---

### Q21

Which query removes duplicate rows **without deleting data from the table**?

A.

```sql
SELECT DISTINCT *
FROM Employees;
```

B.

```sql
DELETE DUPLICATE
FROM Employees;
```

C.

```sql
REMOVE DUPLICATE;
```

D.

```sql
TRUNCATE Employees;
```

---

### Q22

Which query is more efficient for checking whether **at least one matching row exists**?

A.

```sql
SELECT COUNT(*)
```

B.

```sql
SELECT *
```

C.

```sql
EXISTS(...)
```

D.

```sql
GROUP BY
```

---

### Q23

Given:

```sql
SELECT Name
FROM Employees
WHERE Name LIKE '_a%';
```

Which name matches?

A. Mark  
B. Sam  
C. David  
D. Aaron

---

### Q24

Suppose an `INNER JOIN` is performed between two tables with **no matching rows**.

The result is:

A. All rows from the left table  
B. All rows from the right table  
C. Empty result  
D. NULL values for every row

---

### Q25

Which statement is **FALSE**?

A. WHERE filters rows before grouping.  
B. HAVING filters groups after aggregation.  
C. GROUP BY is mandatory whenever COUNT() is used.  
D. ORDER BY sorts the final result.

---

