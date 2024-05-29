### **Explanation:**
Aliases are used to give a table or a column a temporary name. They are often used to make column names more readable.

### **Syntax:**
```sql
SELECT column_name AS alias_name
FROM table_name;
```

### **Example:**
```sql
SELECT first_name AS fname, last_name AS lname
FROM employees;
```

### **Use Case:**
Simplifying or clarifying column names in the result set.
