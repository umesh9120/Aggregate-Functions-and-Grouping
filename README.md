# Aggregate-Functions-and-Grouping

**Objective:**
Learn to use aggregate functions and grouping in SQL for summarizing and analyzing data.

**Tool Used:**
MySQL Workbench / DB Browser for SQLite

**Database Overview**

Database: employees

Table: employees_data

Fields: id, name, gender, age, salary

**Queries Performed**

1️⃣ Aggregate Functions

SELECT COUNT(*) FROM employees_data WHERE salary > 40000;

SELECT MIN(salary) AS min_salary, MAX(salary) AS max_salary FROM employees_data;

SELECT SUM(salary) AS total_salary FROM employees_data;

SELECT AVG(salary) AS average_salary FROM employees_data;

2️⃣ Grouping & Filtering Groups

SELECT gender, AVG(salary) AS average_salary 
FROM employees_data 
GROUP BY gender;

SELECT gender, AVG(salary) AS average_salary 
FROM employees_data 
GROUP BY gender 
HAVING AVG(salary) > 30000;

**Key Learnings**

Use COUNT, MIN, MAX, SUM, and AVG for summarizing data.

Group results by a column using GROUP BY.

Apply conditions to groups with HAVING.
