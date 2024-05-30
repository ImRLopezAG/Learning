### **Explanation:**
Adding a column to a table involves altering the table structure to include a new column. You can specify the data type and other attributes (e.g., default values, constraints) for the new column.

### **Syntax:**
```sql
ALTER TABLE table_name
ADD column_name datatype [constraint];
```

### **Example:**
```sql
ALTER TABLE employees
ADD date_of_birth DATE;
```

### **Use Case:**
Adding a `date_of_birth` column to the `employees` table to store employees' birth dates.
