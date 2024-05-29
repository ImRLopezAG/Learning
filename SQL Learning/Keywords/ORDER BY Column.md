### **Explanation:**
The `ORDER BY` clause is used to sort the result set of a query by one or more columns. The sorting can be in ascending (`ASC`) or descending (`DESC`) order.

### **Syntax:**
```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition
ORDER BY column1 [ASC|DESC], column2 [ASC|DESC], ...;
```

### **Example:**
```sql
SELECT first_name, last_name, hire_date
FROM employees
WHERE department = 'Sales'
ORDER BY hire_date DESC, last_name ASC;
```

### **Use Case:**
Fetching employees in the Sales department, ordered by hire date in descending order and then by last name in ascending order.
