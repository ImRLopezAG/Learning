- **Explanation:** Joins are used to combine rows from two or more tables.
- **Types of Joins:**
  - **INNER JOIN:** Returns records with matching values in both tables.
  - **LEFT JOIN (or LEFT OUTER JOIN):** Returns all records from the left table, and matched records from the right table.
  - **RIGHT JOIN (or RIGHT OUTER JOIN):** Returns all records from the right table, and matched records from the left table.
  - **FULL JOIN (or FULL OUTER JOIN):** Returns all records when there is a match in either left or right table.
- **Syntax:**
  ```sql
  SELECT columns
  FROM table1
  INNER JOIN table2
  ON table1.common_column = table2.common_column;
  ```
- **Example:**
  ```sql
  SELECT employees.first_name, employees.last_name, departments.department_name
  FROM employees
  INNER JOIN departments
  ON employees.department_id = departments.department_id;
  ```
- **Use Cases:** Fetching related data from multiple tables.

## See

### [JOINS](../Keywords/JOINS.md)
