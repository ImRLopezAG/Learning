### **Explanation:**
The `HAVING` clause is used to filter groups based on conditions. It is similar to the `WHERE` clause but is used with the `GROUP BY` clause to apply conditions to groups, not individual rows.

### **Syntax:**
```sql
SELECT column1, aggregate_function(column2)
FROM table_name
WHERE condition
GROUP BY column1
HAVING condition;
```

### **Example:**
```sql
SELECT department, COUNT(*)
FROM employees
WHERE hire_date > '2020-01-01'
GROUP BY department
HAVING COUNT(*) > 5;
```

### **Use Case:**
Counting departments that have more than 5 employees hired after January 1, 2020.
