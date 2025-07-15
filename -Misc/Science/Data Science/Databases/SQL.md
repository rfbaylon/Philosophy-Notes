---
Course: Database Design
---

SQL is based on multisets where [[Relational Algebra]] is based on sets. Data is also in some order in SQL, where order doesnt matter in RA. 

SELECT is the querying powerhouse of SQL

#### Syntax
if an identifier has a space, you write it within backticks (eg \`Customer Name\`)

#### Simple Stuff
General form of a simple SELECT statement:
```
SELECT <col1>[, <col2>, etc]
FROM <table>
```
SELECT is equal to $\pi$ in [[Relational Algebra]]

\* is a wildcard and returns all columns.
```
SELECT *
FROM <table>
```

You can rename / alias attributes
```
SELECT <col1> AS <newname>
FROM <table>
```

You can do basic calculations
```
SELECT (<col1> * <col2>) AS <product>
FROM <table>
```

You can do a where clause that selects only a subset of the data (like $\sigma$ in [[Relational Algebra]])

```
SELECT LastName, HireDate
FROM Employees
WHERE HireDate >= '2014-01-20'
```
WHERE clauses include
- equals (=)
- Not equal to (<>)
- Greater/Less than (<, >)
- Greater/ Less than or equal ot (<=, >=)
- Matches pattern (LIKE)
	- \% Matches any sequance in a string (like ctrl+f) 
		- WHERE CompanyName LIKE 'fo%'
	- _ Matches any single character in the string 
		- WHERE FirstName LIKE 'J___'
		- Returns: Jake, Jess but NOT Jonathan, Jordan
- Within a set (IN)
- Compare to NULL (IS or IS NOT)
- Inclusive range (esp. dates) (BETWEEN)

#### Sorting
```
SELECT <list of columns>
FROM <table name>
WHERE <condition list>
ORDER BY <column-order list>
```
you can ORDER BY either ascending (ASC) (default) or descending (DESC)

Remove duplicates with `SELECT DISTINCT` 


#### Aggregate Functions
There are 5 aggregate functions
1. MAX
2. MIN
3. SUM
4. AVG
5. COUNT


#### Sets
UNION, INTERSECT, EXCEPT
Equal to $\cup , \cap$ and except is just english. 

```
# Select cities where both an employee and customer live
SELECT City
FROM Employees
WHERE Country = 'USA'
	INTERSECT
SELECT City
FROM Customers
WHERE Country = 'USA'
```

#### Joins
**Inner** Join - returns rows that match the predicate
**Equi** Join - join predicate that uses = (basically a theta join)
**Natural** Join - predicate is based on attributes withthe same nameds and data types
**Outer** Join - the type of outer join indicates what to do with rows from either or both tables that do not match the join predicate.

![[Pasted image 20250709110924.png]]

Level 0: Join
```
SELECT ProductName, CategoryName
FROM Products JOIN Categories
	ON Products.CategoryID = Categories.CategoryID;
```
Level 1: Natural Join
(it autmaticall matches based on columns with the same name and datatype)
(Fontenot thinks I should NEVER use this)
```
SELECT ProductName, CategoryName
FROM Products JOIN Categories
```

Level 2: Outer Join
Includes everything from the inner join, but also includes:
- all rows from the left or right operand (or both) that the other does not include.
- Will add rows with `NULL` after the joins happen

```
SELECT *
FROM Student LEFT OUTER JOIN Grades
	ON Student.sID = Grades.sID
```

Level 3: Self Joins??

```
SELECT emp.FirstName, emp.LastName, mgr.FirstName, mgr.LastName
FROM Employees mgr
	JOIN Employees emp
		ON mgr.EmployeeID = emp.ReportsTo
```

```
SELECT *
FROM Employees e1
	JOIN Employees e2
	ON e1.FirstName = e2.FirstName
	AND e1.LastName = e2.LastName
WHERE e1.EmployeeID <> e2.EmployeeID
```

### Limits
Just returns the first x rows from a list
```
SELECT *
FROM orders
LIMIT 5 OFFSET 5
```
Limit 5 shows 5 rows, OFFSET 5 shows the 5th-10th row (skips the first 5)