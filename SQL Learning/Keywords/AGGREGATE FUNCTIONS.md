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

---

## **17. TRANSACTIONS**

### **Explanation:**
Transactions are used to execute a sequence of SQL statements as a single unit of work. They ensure data integrity by allowing commit and rollback operations.

### **Syntax:**
```sql
BEGIN TRANSACTION;
-- SQL statements
COMMIT;
-- or
ROLLBACK;
```

### **Example:**
```sql
BEGIN TRANSACTION;
UPDATE employees SET salary = salary * 1.10 WHERE department = 'Sales';
DELETE FROM employees WHERE hire_date < '2000-01-01';
COMMIT;
```

### **Use Case:**
Ensuring that either all salary updates and deletions are executed successfully or none of them are, maintaining data consistency.