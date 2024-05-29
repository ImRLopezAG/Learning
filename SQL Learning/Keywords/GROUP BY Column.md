### **Explanation:**
The `GROUP BY` clause groups rows that have the same values in specified columns into summary rows, like “find the number of employees in each department.” It is often used with aggregate functions like `COUNT()`, `SUM()`, `AVG()`, `MAX()`, and `MIN()` to perform operations on each group.

### **Syntax:**
```sql
SELECT column1, aggregate_function(column2)
FROM table_name
WHERE condition
GROUP BY column1;
```

### **Example:**
```sql
SELECT department, COUNT(*)
FROM employees
WHERE hire_date > '2020-01-01'
GROUP BY department;
```

### **Use Case:**
Counting the number of employees hired after January 1, 2020, grouped by department.
