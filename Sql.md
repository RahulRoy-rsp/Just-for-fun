

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


Perfect. Instead of making them "hard," let's make them thought-provoking. These are the kind of questions companies and technical interviews ask—they test whether someone understands what SQL is doing rather than whether they've memorized syntax.

This set assumes the learner knows:

SELECT

WHERE

GROUP BY

HAVING

ORDER BY

Aggregate Functions

NULL

Basic JOINs



---

## Set 2 (Higher Difficulty)

Q1

Consider the table:

EmpID	Name	Salary

1	Alice	50000
2	Bob	NULL
3	Charlie	70000


What is the output?

SELECT COUNT(Salary)
FROM Employees;

A. 3

B. 2

C. 1

D. NULL


---

Q2

Which query correctly returns departments having more than 5 employees?

A.

SELECT Department
FROM Employees
WHERE COUNT(*) > 5;

B.

SELECT Department
FROM Employees
GROUP BY Department
HAVING COUNT(*) > 5;

C.

SELECT Department
FROM Employees
HAVING COUNT(*) > 5;

D.

SELECT Department
WHERE COUNT(*) > 5
GROUP BY Department;


---

Q3

Given:

SELECT *
FROM Employees
WHERE Salary > 50000
AND Department = 'IT'
OR Department = 'HR';

Which statement is correct?

A. Returns IT employees earning above 50000 only

B. Returns all HR employees and IT employees earning above 50000

C. Returns only HR employees earning above 50000

D. Returns only employees earning above 50000


---

Q4

Which statement about NULL is TRUE?

A. NULL is equal to 0.

B. NULL is an empty string.

C. NULL represents an unknown or missing value.

D. NULL is treated as FALSE.


---

Q5

Which query returns the second highest salary?

A.

SELECT MAX(Salary)
FROM Employees;

B.

SELECT MAX(Salary)
FROM Employees
WHERE Salary < (
    SELECT MAX(Salary)
    FROM Employees
);

C.

SELECT Salary
FROM Employees
ORDER BY Salary;

D.

SELECT MIN(Salary)
FROM Employees;


---

Q6

Suppose Employee table contains:

Department	Salary

IT	50000
IT	70000
HR	60000
HR	55000


What is returned?

SELECT Department,
AVG(Salary)
FROM Employees
GROUP BY Department;

A. One row

B. Two rows

C. Four rows

D. Error


---

Q7

Which clause executes last logically?

A. WHERE

B. GROUP BY

C. HAVING

D. ORDER BY


---

Q8

Which query is INVALID?

A.

SELECT *
FROM Employees
ORDER BY Salary DESC;

B.

SELECT Department,
COUNT(*)
FROM Employees
GROUP BY Department;

C.

SELECT Department,
Salary
FROM Employees
GROUP BY Department;

D.

SELECT Name
FROM Employees
WHERE Salary > 50000;


---

Q9

Suppose:

Employees

ID	Name

1	Alice
2	Bob


Orders

OrderID	EmployeeID

101	1
102	1


Using

SELECT *
FROM Employees
INNER JOIN Orders
ON Employees.ID = Orders.EmployeeID;

How many rows are returned?

A. 1

B. 2

C. 3

D. 4


---

Q10

Which JOIN returns all records from the left table, whether matching rows exist or not?

A. INNER JOIN

B. RIGHT JOIN

C. LEFT JOIN

D. CROSS JOIN


---

Q11

Which aggregate function ignores NULL values?

A. COUNT(column)

B. SUM(column)

C. AVG(column)

D. All of the above


---

Q12

What does this query return?

SELECT DISTINCT Department
FROM Employees;

A. Every department including duplicates

B. Only unique department names

C. First department only

D. Departments sorted alphabetically


---

Q13

Which query returns employees not working in Sales?

A.

WHERE Department != 'Sales'

B.

WHERE NOT Department='Sales'

C.

WHERE Department <> 'Sales'

D. All of the above (assuming SQL dialect supports !=)


---

Q14

Given:

SELECT *
FROM Employees
WHERE Salary IN
(40000,50000,60000);

Which employee is returned?

A. Salary exactly equal to one of these values

B. Salary greater than 40000

C. Salary less than 60000

D. Salary between 40000 and 60000


---

Q15

Suppose table contains:

Salary

50000
50000
70000


Result of

SELECT COUNT(DISTINCT Salary)
FROM Employees;

A. 3

B. 2

C. 1

D. Error


---

Q16

Which statement best describes a Primary Key?

A. Can contain NULL

B. Can contain duplicate values

C. Must uniquely identify every row

D. Can have duplicate NULL values


---

Q17

Which statement about Foreign Keys is TRUE?

A. Must always be unique

B. Can reference only the Primary Key (or another UNIQUE key) of another table

C. Cannot contain NULL

D. Automatically sorts data


---

Q18

Consider

SELECT *
FROM Employees
WHERE Salary > ALL
(
SELECT Salary
FROM Managers
);

This returns employees whose salary is

A. Greater than at least one manager

B. Greater than every manager

C. Equal to highest manager salary

D. Lower than every manager


---

Q19

Which query returns departments whose average salary exceeds 60,000?

A.

SELECT Department
FROM Employees
WHERE AVG(Salary)>60000;

B.

SELECT Department
FROM Employees
GROUP BY Department
HAVING AVG(Salary)>60000;

C.

SELECT AVG(Salary)
WHERE Department;

D.

SELECT Department
HAVING AVG(Salary);


---

Q20

Suppose

SELECT *
FROM Employees
ORDER BY Salary ASC
LIMIT 3;

returns

A. Top 3 highest salaries

B. Top 3 lowest salaries

C. Random 3 employees

D. Employees with salary = 3


---

Q21

Which query removes duplicate rows without deleting data from the table?

A.

SELECT DISTINCT *
FROM Employees;

B.

DELETE DUPLICATE
FROM Employees;

C.

REMOVE DUPLICATE;

D.

TRUNCATE Employees;


---

Q22

Which query is more efficient for checking whether at least one matching row exists?

A.

SELECT COUNT(*)

B.

SELECT *

C.

EXISTS(...)

D.

GROUP BY


---

Q23

Given

SELECT Name
FROM Employees
WHERE Name LIKE '_a%';

Which name matches?

A. Mark

B. Sam

C. David

D. Aaron


---

Q24

Suppose an INNER JOIN is performed between two tables with no matching rows.

The result is

A. All rows from left table

B. All rows from right table

C. Empty result

D. NULL values for every row


---

Q25

Which statement is FALSE?

A. WHERE filters rows before grouping.

B. HAVING filters groups after aggregation.

C. GROUP BY is mandatory whenever COUNT() is used.

D. ORDER BY sorts the final result.


---

Excellent. For the final set, I'd aim for the level of good SQL screening rounds (internships, freshers, junior developers, data analysts). These questions require understanding SQL's behavior, but they don't rely on advanced features like window functions or recursive CTEs.

This progression gives learners a complete foundation:

Set 1: Fundamentals

Set 2: Query reasoning

Set 3: Practical SQL thinking (below)



---

## Set 3

Q1

Given the table:

ID	Name	Department	Salary

1	Alice	IT	60000
2	Bob	HR	50000
3	Charlie	IT	70000
4	David	Sales	50000


What is the output?

SELECT Department, COUNT(*)
FROM Employees
GROUP BY Department;

A. One row with total employee count

B. One row for each department with its employee count

C. Total departments only

D. Error


---

Q2

Which query correctly finds employees whose salary is not between 40,000 and 60,000?

A.

WHERE Salary NOT BETWEEN 40000 AND 60000

B.

WHERE Salary <40000 AND Salary >60000

C.

WHERE Salary !=40000 AND 60000

D.

WHERE Salary OUTSIDE (40000,60000)


---

Q3

Which SQL clause can contain aggregate functions like SUM() or AVG() directly?

A. WHERE

B. HAVING

C. ORDER

D. DISTINCT


---

Q4

What will be returned?

SELECT COUNT(*)
FROM Employees
WHERE Department='Finance';

Assume there are no Finance employees.

A. NULL

B. Error

C. 0

D. 1


---

Q5

Which query returns the highest salary in each department?

A.

SELECT MAX(Salary)
FROM Employees;

B.

SELECT Department,
MAX(Salary)
FROM Employees
GROUP BY Department;

C.

SELECT Department,
Salary
FROM Employees;

D.

SELECT Department
HAVING MAX(Salary);


---

Q6

Which statement about ORDER BY is TRUE?

A. It always sorts ascending only.

B. Multiple columns can be used for sorting.

C. It works only with numeric columns.

D. It removes duplicates before sorting.


---

Q7

Suppose

SELECT *
FROM Employees
LIMIT 5;

The table has only 3 rows.

The query returns

A. Error

B. First 3 rows

C. NULL rows

D. Empty result


---

Q8

Which operator checks whether a value exists in a list?

A. EXISTS

B. BETWEEN

C. IN

D. LIKE


---

Q9

Consider

SELECT *
FROM Employees
WHERE Salary >50000
ORDER BY Name;

Which happens first logically?

A. Sorting

B. Filtering

C. Displaying

D. Removing duplicates


---

Q10

What is returned?

SELECT MIN(Salary),
MAX(Salary)
FROM Employees;

A. One row

B. Two rows

C. Every employee

D. Error


---

Q11

Which statement is TRUE regarding DISTINCT?

A. Removes duplicate rows from the result.

B. Deletes duplicates from the table.

C. Works only with numbers.

D. Requires GROUP BY.


---

Q12

Suppose

Employees

ID	Name

1	Alice
2	Bob
3	Charlie


Orders

EmployeeID

1
1


Using a LEFT JOIN, how many rows are returned?

A. 2

B. 3

C. 4

D. 5


---

Q13

Which query returns employees whose department name contains the word Sales anywhere?

A.

LIKE '%Sales%'

B.

LIKE 'Sales%'

C.

LIKE '_Sales'

D.

LIKE 'Sales'


---

Q14

Which statement about aggregate functions is FALSE?

A. AVG ignores NULL values.

B. SUM ignores NULL values.

C. COUNT(column) counts NULL values.

D. MAX ignores NULL values.


---

Q15

Given

SELECT Department,
COUNT(*)
FROM Employees
GROUP BY Department
HAVING COUNT(*)>=2;

Which departments are returned?

A. Every department

B. Departments having at least two employees

C. Departments with highest salary

D. Departments sorted alphabetically


---

Q16

Which query checks whether a column contains NULL values?

A.

WHERE Column=NULL

B.

WHERE Column IS NULL

C.

WHERE Column==NULL

D.

WHERE Column LIKE NULL


---

Q17

Suppose

SELECT *
FROM Employees
WHERE Name LIKE '%n';

Which names match?

A. Ryan

B. John

C. Ethan

D. All of the above


---

Q18

Which SQL statement removes only the table data but keeps the table structure?

A. DROP TABLE

B. DELETE TABLE

C. TRUNCATE TABLE

D. REMOVE TABLE


---

Q19

Which statement is TRUE?

A. Every table must have exactly one Foreign Key.

B. Every table must have exactly one Primary Key (which may consist of one or more columns).

C. Foreign Keys must always contain unique values.

D. Primary Keys may contain NULL values.


---

Q20

Suppose

SELECT *
FROM Employees
WHERE Salary >
(
SELECT AVG(Salary)
FROM Employees
);

The query returns

A. Employees earning above the company average

B. Employees earning the highest salary only

C. Employees earning below average

D. Every employee


---

Q21

Which JOIN returns every possible combination of rows from both tables?

A. INNER JOIN

B. LEFT JOIN

C. CROSS JOIN

D. FULL JOIN


---

Q22

Given

SELECT COUNT(DISTINCT Department)
FROM Employees;

The result is

A. Total employees

B. Number of unique departments

C. Number of duplicate departments

D. Total rows


---

Q23

Which statement about SQL execution order is correct?

A. ORDER BY executes before WHERE.

B. WHERE executes before GROUP BY.

C. HAVING executes before GROUP BY.

D. SELECT executes before FROM.


---

Q24

Suppose

SELECT Name,
Salary
FROM Employees
ORDER BY Salary DESC,
Name ASC;

If two employees have the same salary, they are sorted by

A. ID

B. Name

C. Department

D. Random order


---

Q25

Which of the following best explains why SQL beginners should use GROUP BY carefully?

A. It automatically removes duplicate rows.

B. Every selected column that is not aggregated generally must appear in the GROUP BY clause.

C. It sorts the results automatically.

D. It works only with numeric columns.


---


