### **Explanation:**
The `LIMIT` clause is used to specify the number of records to return. It is useful for pagination or to restrict the result set to a certain number of rows.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition
ORDER BY column1
LIMIT number;
```

### **Example:**
```sql
SELECT first_name, last_name
FROM employees
WHERE department = 'Sales'
ORDER BY hire_date DESC
LIMIT 10;
```

### **Use Case:**
Fetching the top 10 most recently hired employees in the Sales department.