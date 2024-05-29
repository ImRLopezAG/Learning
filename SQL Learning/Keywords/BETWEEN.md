### **Explanation:**
The `BETWEEN` keyword is used to filter the result set within a certain range. The values can be numbers, text, or dates.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE column BETWEEN value1 AND value2;
```

### **Example:**
```sql
SELECT first_name, last_name, hire_date
FROM employees
WHERE hire_date BETWEEN '2020-01-01' AND '2021-12-31';
```

### **Use Case:**
Fetching employees hired within a specific date range.