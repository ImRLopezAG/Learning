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