### **Explanation:**
The `CASE` statement is used to create conditional logic in SQL queries, similar to `IF-THEN-ELSE` statements in programming.

### **Syntax:**
```sql
SELECT column1,
       CASE
           WHEN condition1 THEN result1
           WHEN condition2 THEN result2
           ELSE result3
       END AS alias_name
FROM table_name;
```

### **Example:**
```sql
SELECT first_name, last_name,
       CASE
           WHEN department = 'Sales' THEN 'Sales Department'
           WHEN department = 'Marketing' THEN 'Marketing Department'
           ELSE 'Other Department'
       END AS department_name
FROM employees;
```

### **Use Case:**
Creating custom labels based on department values.