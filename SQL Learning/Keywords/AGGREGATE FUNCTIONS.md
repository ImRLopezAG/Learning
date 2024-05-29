### **Explanation:**
Aggregate functions perform a calculation on a set of values and return a single value. Common aggregate functions include `COUNT()`, `SUM()`, `AVG()`, `MIN()`, and `MAX()`.

### **Syntax:**
```sql
SELECT aggregate_function(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT AVG(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Calculating the average salary of employees in the Sales department.
