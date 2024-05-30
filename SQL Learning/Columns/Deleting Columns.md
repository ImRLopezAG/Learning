### **Explanation:**
Deleting a column removes it from the table along with all its data. This action is irreversible, so it should be done with caution.

### **Syntax:**
```sql
ALTER TABLE table_name
DROP COLUMN column_name;
```

### **Example:**
```sql
ALTER TABLE employees
DROP COLUMN date_of_birth;
```

### **Use Case:**
Removing the `date_of_birth` column from the `employees` table if it is no longer needed.
