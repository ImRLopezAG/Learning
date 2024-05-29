### **Explanation:**
A subquery is a query nested inside another query. It can be used in various clauses like `SELECT`, `FROM`, `WHERE`, etc.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE column = (SELECT column FROM another_table WHERE condition);
```

### **Example:**
```sql
SELECT first_name, last_name
FROM employees
WHERE department_id = (SELECT department_id FROM departments WHERE department_name = 'Sales');
```

### **Use Case:**
Fetching employees who belong to the 'Sales' department by using a subquery to get the department ID.