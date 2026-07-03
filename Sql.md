

---


Easy Level

Q1. Which SQL statement is used to retrieve data from a database?

A. GET

B. FETCH

C. SELECT

D. SHOW


---

Q2. Which clause is used to filter rows in a SQL query?

A. ORDER BY

B. WHERE

C. GROUP BY

D. HAVING


---

Q3. Which keyword removes duplicate rows from the result?

A. UNIQUE

B. DISTINCT

C. DIFFERENT

D. FILTER


---

Q4. Which SQL command is used to add a new row into a table?

A. UPDATE

B. INSERT INTO

C. ADD ROW

D. APPEND


---

Q5. Which command is used to modify existing data in a table?

A. CHANGE

B. ALTER

C. UPDATE

D. MODIFY


---

Q6. Which SQL clause is used to sort the output?

A. SORT BY

B. ORDER BY

C. GROUP BY

D. ARRANGE BY


---

Q7. What does the following query return?

SELECT COUNT(*) FROM Employees;

A. Number of columns

B. Number of rows

C. Sum of employee IDs

D. Number of NULL values


---

Q8. Which symbol is commonly used as a wildcard representing multiple characters?

A. *

B. %

C. _

D. #


---

Medium Level

Q9. Consider the query:

SELECT *
FROM Employees
WHERE Salary > 50000;

Which employees are returned?

A. Salary less than 50000

B. Salary equal to 50000

C. Salary greater than 50000

D. All employees


---

Q10. Which query correctly selects employees whose name starts with "A"?

A.

WHERE Name = 'A%'

B.

WHERE Name LIKE 'A%'

C.

WHERE Name STARTS 'A'

D.

WHERE Name MATCH 'A%'


---

Q11. What is the difference between DELETE and TRUNCATE?

A. No difference

B. DELETE removes selected rows, TRUNCATE removes all rows

C. TRUNCATE deletes one row at a time

D. DELETE removes the table structure


---

Q12. Which function returns the highest value?

A. MAX()

B. TOP()

C. HIGH()

D. UPPER()


---

Q13. Which clause is used to group rows having the same values?

A. ORDER BY

B. GROUP BY

C. SORT BY

D. DISTINCT


---

Q14. Which query returns employees working in either HR or Finance?

A.

WHERE Department = 'HR' OR 'Finance'

B.

WHERE Department IN ('HR','Finance')

C.

WHERE Department = HR, Finance

D.

WHERE Department LIKE HR|Finance


---

Q15. Which SQL statement changes only the table structure?

A. UPDATE

B. ALTER TABLE

C. INSERT

D. SELECT


---

Q16. What will this query return?

SELECT AVG(Salary)
FROM Employees;

A. Total salary

B. Average salary

C. Maximum salary

D. Number of employees


---

Q17. Which condition checks for missing values?

A.

Salary = NULL

B.

Salary == NULL

C.

Salary IS NULL

D.

Salary EQUAL NULL


---

Intermediate Level

Q18. Which query finds the total salary department-wise?

A.

SELECT Department, SUM(Salary)
FROM Employees;

B.

SELECT Department, SUM(Salary)
FROM Employees
GROUP BY Department;

C.

SELECT SUM(Salary)
GROUP Department;

D.

SELECT Department
GROUP BY Salary;


---

Q19. Consider the query:

SELECT Name
FROM Employees
ORDER BY Salary DESC;

Which employee appears first?

A. Lowest salary

B. Random employee

C. Highest salary

D. Oldest employee


---

Q20. What is the purpose of the HAVING clause?

A. Filters rows before grouping

B. Filters grouped data after GROUP BY

C. Sorts grouped data

D. Removes duplicates


---

Q21. Which query returns employees earning between 40,000 and 60,000 (inclusive)?

A.

WHERE Salary > 40000 AND Salary < 60000

B.

WHERE Salary BETWEEN 40000 AND 60000

C.

WHERE Salary = 40000 TO 60000

D.

WHERE Salary RANGE 40000,60000


---

Q22. Which SQL function converts text to uppercase?

A. CAPITAL()

B. UPPER()

C. TOUPPER()

D. UCASETEXT()


---

Q23. Which query returns the first 5 rows in MySQL?

A.

SELECT FIRST 5 * FROM Employees;

B.

SELECT TOP 5 * FROM Employees;

C.

SELECT * FROM Employees LIMIT 5;

D.

SELECT * FIRST 5;


---

Q24. Suppose the Orders table has 200 rows. What will this query return?

SELECT COUNT(OrderDate)
FROM Orders;

A. Always 200

B. Number of non-NULL OrderDate values

C. Number of unique dates

D. Total columns


---

Q25. Which statement about SQL is correct?

A. SQL is case-sensitive for keywords.

B. SQL can only retrieve data.

C. SQL can create, modify, retrieve, and delete data.

D. SQL cannot create tables.


---

