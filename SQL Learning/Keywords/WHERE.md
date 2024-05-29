## **1. WHERE Condition**

### **Explanation:**
The `WHERE` clause is used to filter records based on specified conditions. It is commonly used in `SELECT`, `UPDATE`, `DELETE`, and other SQL statements to restrict the rows returned or affected by the query.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT first_name, last_name
FROM employees
WHERE department = 'Sales' AND hire_date > '2020-01-01';
```

### **Use Case:**
Fetching employees who are in the Sales department and were hired after January 1, 2020.