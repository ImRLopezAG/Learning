### **Explanation:**
The `IN` keyword allows you to specify multiple values in a `WHERE` clause.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE column IN (value1, value2, ...);
```

### **Example:**
```sql
SELECT first_name, last_name
FROM employees
WHERE department IN ('Sales', 'Marketing');
```

### **Use Case:**
Filtering records to include only those that belong to specified departments.