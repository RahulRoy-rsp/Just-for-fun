
---

# SQL MCQs (Medium to Intermediate)

## 1. Which query returns departments having more than 5 employees?

A.

```sql
SELECT department_id
FROM employees
GROUP BY department_id
HAVING COUNT(*) > 5;
```

B.

```sql
SELECT department_id
FROM employees
WHERE COUNT(*) > 5;
```

C.

```sql
SELECT department_id
FROM employees
HAVING COUNT(*) > 5;
```

D.

```sql
SELECT department_id
FROM employees
WHERE department_id > 5;
```


---

## 2. What is the output of the following?

```sql
SELECT COUNT(column_name)
FROM table_name;
```

A. Counts all rows

B. Counts only non-NULL values

C. Counts only NULL values

D. Counts distinct values


---

## 3. Which JOIN returns only matching rows from both tables?

A. LEFT JOIN

B. RIGHT JOIN

C. INNER JOIN

D. FULL JOIN


---

## 4. What is the result of this query?

```sql
SELECT DISTINCT city
FROM customers;
```

A. Removes duplicate city values

B. Removes duplicate rows only

C. Sorts city alphabetically

D. Returns NULL values only


---

## 5. Which clause is evaluated after GROUP BY?

A. WHERE

B. ORDER BY

C. HAVING

D. FROM


---

## 6. Which function can assign a unique rank without gaps?

A. RANK()

B. DENSE_RANK()

C. ROW_NUMBER()

D. NTILE()


---

## 7. Which query finds the second highest salary?

A.

```sql
SELECT MAX(salary)
FROM employees;
```

B.

```sql
SELECT MAX(salary)
FROM employees
WHERE salary < (SELECT MAX(salary) FROM employees);
```

C.

```sql
SELECT MIN(salary)
FROM employees;
```

D.

```sql
SELECT salary
FROM employees;
```


---

## 8. Which constraint prevents duplicate values?

A. CHECK

B. PRIMARY KEY

C. UNIQUE

D. FOREIGN KEY


---

## 9. What happens when a PRIMARY KEY is defined?

A. NULL values allowed

B. Duplicate values allowed

C. Values must be unique and NOT NULL

D. Only unique NULL values allowed


---

## 10. Which SQL statement removes duplicate rows?

A.

```sql
DELETE DUPLICATES
```

B.

```sql
DISTINCT
```

C.

```sql
UNIQUE ROWS
```

D.

```sql
REMOVE DUPLICATES
```


---

## 11. Which operator checks for NULL values?

A.

```sql
= NULL
```

B.

```sql
IS NULL
```

C.

```sql
== NULL
```

D.

```sql
NULL()
```


---

## 12. Which query returns employees who do not belong to any department?

A.

```sql
SELECT *
FROM employees
WHERE department_id = NULL;
```

B.

```sql
SELECT *
FROM employees
WHERE department_id IS NULL;
```

C.

```sql
SELECT *
FROM employees
WHERE department_id <> NULL;
```

D.

```sql
SELECT *
FROM employees
WHERE department_id != NULL;
```


---

## 13. Which JOIN returns all rows from the left table even if no match exists?

A. INNER JOIN

B. LEFT JOIN

C. RIGHT JOIN

D. CROSS JOIN


---

## 14. Which aggregate function ignores NULL values?

A. COUNT(column)

B. SUM()

C. AVG()

D. All of the above


---

## 15. Which clause filters groups after aggregation?

A. WHERE

B. GROUP BY

C. HAVING

D. ORDER BY


---

## 16. Which window function gives the same rank for ties and skips the next rank?

A. ROW_NUMBER()

B. RANK()

C. DENSE_RANK()

D. NTILE()


---

## 17. What is the output?

```sql
SELECT COALESCE(NULL, NULL, 10, 20);
```

A. NULL

B. 20

C. 10

D. Error


---

## 18. Which statement about indexes is TRUE?

A. They slow down SELECT queries.

B. They improve search performance but may slow INSERT/UPDATE/DELETE.

C. They prevent duplicate rows.

D. They replace PRIMARY KEY.


---

## 19. Which command permanently removes a table and its data?

A. DELETE

B. REMOVE

C. DROP

D. TRUNCATE


---

## 20. Which SQL clause is executed first logically?

A. SELECT

B. FROM

C. ORDER BY

D. HAVING


---

## 21. Which query returns employees earning above the average salary?

A.

```sql
SELECT *
FROM employees
WHERE salary >
(
SELECT AVG(salary)
FROM employees
);
```

B.

```sql
SELECT AVG(salary)
FROM employees;
```

C.

```sql
SELECT *
FROM employees
HAVING salary > AVG(salary);
```

D.

```sql
SELECT *
FROM employees
GROUP BY salary;
```


---

## 22. Which transaction property ensures completed transactions remain permanent?

A. Atomicity

B. Consistency

C. Isolation

D. Durability


---

## 23. Which query finds duplicate email addresses?

A.

```sql
SELECT email
FROM users
GROUP BY email
HAVING COUNT(*) > 1;
```

B.

```sql
SELECT DISTINCT email
FROM users;
```

C.

```sql
SELECT email
FROM users
ORDER BY email;
```

D.

```sql
SELECT COUNT(email)
FROM users;
```



---

## 24. Which JOIN returns the Cartesian product of two tables?

A. FULL JOIN

B. INNER JOIN

C. CROSS JOIN

D. LEFT JOIN


---

## 25. Consider the query:

```sql
SELECT department_id,
       AVG(salary)
FROM employees
GROUP BY department_id
HAVING AVG(salary) > 50000;
```

What does this query return?

A. Employees earning more than 50,000

B. Departments where the average salary exceeds 50,000

C. Highest-paid employee in each department

D. Departments with more than 50,000 employees

---

# SQL MCQs Set 2 (Theory | Intermediate–Advanced)

### 1. Which SQL clause cannot directly use an aggregate function?

A. HAVING

B. SELECT

C. WHERE

D. ORDER BY


---

### 2. Which of the following is **not** an ACID property of a transaction?

A. Atomicity

B. Consistency

C. Integrity

D. Durability

---

### 3. What is the primary purpose of normalization?

A. Increase redundancy

B. Improve query speed

C. Reduce data redundancy and improve data integrity

D. Reduce storage only


---

### 4. Which normal form eliminates partial dependency?

A. First Normal Form (1NF)

B. Second Normal Form (2NF)

C. Third Normal Form (3NF)

D. Boyce-Codd Normal Form (BCNF)

---

### 5. Which normal form primarily removes transitive dependency?

A. 1NF

B. 2NF

C. 3NF

D. 4NF

---

### 6. Which statement about a PRIMARY KEY is correct?

A. It may contain NULL values.

B. A table can have multiple primary keys.

C. It uniquely identifies each row and cannot contain NULL values.

D. It automatically references another table.


---

### 7. Which statement about UNIQUE constraints is true?

A. They always become clustered indexes.

B. They prevent duplicate values but generally allow a NULL value.

C. They automatically become foreign keys.

D. They prevent NULL values.

---

### 8. Which statement best describes a FOREIGN KEY?

A. It uniquely identifies rows.

B. It enforces referential integrity between tables.

C. It speeds up joins automatically.

D. It prevents duplicate rows.


---

### 9. What happens if a FOREIGN KEY references a value that does not exist in the parent table?

A. SQL automatically inserts the parent row.

B. The child row is ignored.

C. The operation fails due to referential integrity violation.

D. The database creates a NULL value.


---

### 10. Which SQL operation generally benefits the most from an index?

A. INSERT

B. UPDATE

C. DELETE

D. SELECT


---

### 11. Why can excessive indexing negatively impact database performance?

A. Indexes consume no storage.

B. Every data modification may require index updates.

C. Indexes prevent joins.

D. Indexes increase table redundancy.

---

### 12. Which join returns every possible combination of rows from two tables?

A. INNER JOIN

B. FULL OUTER JOIN

C. CROSS JOIN

D. LEFT JOIN



---

### 13. What is the difference between WHERE and HAVING?

A. WHERE filters rows before grouping; HAVING filters groups after aggregation.

B. They are identical.

C. HAVING executes before WHERE.

D. WHERE only works with joins.



---

### 14. Which SQL operator is commonly used to compare a value against the result of a subquery returning multiple rows?

A. =

B. ANY

C. EXISTS

D. LIKE



---

### 15. Which statement about EXISTS is true?

A. It checks whether a subquery returns at least one row.

B. It returns only numeric values.

C. It always performs faster than JOIN.

D. It cannot be used with correlated subqueries.



---

### 16. Which of the following is **not** a window function?

A. ROW_NUMBER()

B. RANK()

C. DENSE_RANK()

D. COUNT_ROWS()



---

### 17. What is the main advantage of window functions over GROUP BY?

A. They reduce storage.

B. They allow aggregate calculations while preserving individual rows.

C. They automatically remove duplicates.

D. They eliminate NULL values.


---

### 18. Which transaction isolation level allows dirty reads?

A. Serializable

B. Repeatable Read

C. Read Committed

D. Read Uncommitted


---

### 19. Which transaction isolation level provides the highest consistency?

A. Read Uncommitted

B. Read Committed

C. Repeatable Read

D. Serializable



---

### 20. What is a dirty read?

A. Reading uncommitted data from another transaction.

B. Reading duplicate records.

C. Reading deleted records.

D. Reading NULL values.


---

### 21. Which SQL command removes all rows but keeps the table structure?

A. DELETE

B. DROP

C. TRUNCATE

D. REMOVE



---

### 22. Which statement best distinguishes DELETE from TRUNCATE?

A. DELETE cannot use WHERE.

B. TRUNCATE removes rows without logging individual row deletions in most database systems, making it generally faster.

C. TRUNCATE removes only duplicate rows.

D. DELETE also removes the table definition.

---

### 23. Which of the following is generally true about views?

A. They always store data physically.

B. They are virtual tables defined by a query.

C. They cannot contain joins.

D. They always improve performance.


---

### 24. Why are indexes generally **not** recommended on columns with very low cardinality (few distinct values)?

A. They cannot be created.

B. They often provide little performance benefit because many rows share the same value.

C. They prevent sorting.

D. SQL databases reject such indexes.



---

### 25. Which statement best describes a correlated subquery?

A. It executes only once.

B. It references columns from the outer query and is evaluated for each outer row.

C. It cannot appear in the WHERE clause.

D. It always returns a single row.


---

# SQL MCQs Set 3 (Advanced Theory) — 

### 1. Which of the following best describes **referential integrity** in a relational database?

A. Ensuring every column contains unique values

B. Ensuring relationships between tables remain consistent

C. Ensuring every table has a primary key

D. Ensuring duplicate rows are automatically removed

---

### 2. Which statement about **candidate keys** is correct?

A. Every candidate key must contain multiple columns.

B. A table can have only one candidate key.

C. Every candidate key is a minimal set of attributes that can uniquely identify a row.

D. Candidate keys always become foreign keys.

---

### 3. Which of the following anomalies is primarily eliminated by normalization?

A. Compilation anomaly

B. Update anomaly

C. Execution anomaly

D. Syntax anomaly

---

### 4. Which statement about **NULL** values in SQL is true?

A. NULL is equivalent to zero.

B. NULL is treated as an empty string in all databases.

C. NULL represents an unknown or missing value.

D. NULL is always ignored in comparisons.

---

### 5. Why is a **surrogate key** often preferred over a natural key?

A. It always reduces storage requirements.

B. It is generated independently of business data and remains stable over time.

C. It automatically creates indexes on all columns.

D. It eliminates the need for foreign keys.

---

### 6. Which statement about **database indexes** is correct?

A. Every column should have an index.

B. Indexes generally improve data retrieval but may slow down data modification operations.

C. Indexes reduce the size of a table.

D. Indexes are useful only for primary keys.

---

### 7. Which of the following best describes a **composite primary key**?

A. A primary key containing duplicate values.

B. A primary key created from two or more columns.

C. Two separate primary keys in the same table.

D. A primary key that references another table.

---

### 8. Which SQL feature is specifically designed to maintain **data consistency** when multiple users access the database simultaneously?

A. Constraints

B. Transactions

C. Views

D. Aliases

---

### 9. Which transaction isolation level provides the **highest level of isolation**?

A. Read Uncommitted

B. Read Committed

C. Repeatable Read

D. Serializable

---

### 10. Which of the following statements about **views** is true?

A. A view always stores data physically.

B. A view can simplify complex queries by presenting data as a virtual table.

C. A view can never be based on multiple tables.

D. A view always improves query performance.

---

### 11. Which SQL object is primarily used to **enforce data integrity** by restricting the values that can be stored in a column?

A. View

B. Constraint

C. Trigger

D. Index

---

### 12. Which of the following best describes the purpose of **GROUP BY**?

A. To sort query results.

B. To combine rows with similar values so aggregate functions can be applied.

C. To remove duplicate rows.

D. To filter rows before retrieval.

---

### 13. Which of the following is **not** considered a Data Manipulation Language (DML) statement?

A. INSERT

B. UPDATE

C. DELETE

D. ALTER

---

### 14. Which statement about **INNER JOIN** is correct?

A. It returns all rows from both tables regardless of matching values.

B. It returns only the rows where matching values exist in both tables.

C. It returns all rows from the left table only.

D. It returns the Cartesian product of both tables.

---

### 15. Which of the following best explains the purpose of **database normalization**?

A. To increase data redundancy for faster queries.

B. To organize data in a way that minimizes redundancy and improves data integrity.

C. To replace indexes with constraints.

D. To ensure every table contains only one column.
