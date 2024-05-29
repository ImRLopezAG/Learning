### **Explanation:**
The `LIKE` keyword is used in a `WHERE` clause to search for a specified pattern in a column.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE column LIKE pattern;
```

### **Example:**
```sql
SELECT first_name, last_name
FROM employees
WHERE first_name LIKE 'J%';
```

### **Use Case:**
Finding employees whose first name starts with the letter 'J'.