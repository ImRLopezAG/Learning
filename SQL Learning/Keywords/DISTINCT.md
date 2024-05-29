### **Explanation:**
The `DISTINCT` keyword is used to return only distinct (different) values in the result set. It eliminates duplicate records.

### **Syntax:**
```sql
SELECT DISTINCT column1, column2, ...
FROM table_name;
```

### **Example:**
```sql
SELECT DISTINCT department
FROM employees;
```

### **Use Case:**
Fetching a list of unique departments from the employees table.
