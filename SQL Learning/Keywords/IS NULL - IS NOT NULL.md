### **Explanation:**
These keywords are used to check for NULL values in a column.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE column IS NULL;

SELECT column1, column2, ...
FROM table_name
WHERE column IS NOT NULL;
```

### **Example:**
```sql
SELECT first_name, last_name
FROM employees
WHERE department IS NULL;
```

### **Use Case:**
Fetching employees who do not have an assigned department.
