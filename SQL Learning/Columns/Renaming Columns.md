### **Explanation:**
Renaming a column changes its name without altering the data or its properties. This is useful for improving readability or standardizing column names.

### **Syntax:**
- **MySQL:**
  ```sql
  ALTER TABLE table_name
  CHANGE old_column_name new_column_name datatype;
  ```
- **SQL Server:**
  ```sql
  EXEC sp_rename 'table_name.old_column_name', 'new_column_name', 'COLUMN';
  ```
- **PostgreSQL:**
  ```sql
  ALTER TABLE table_name
  RENAME COLUMN old_column_name TO new_column_name;
  ```

### **Example:**
- **MySQL:**
  ```sql
  ALTER TABLE employees
  CHANGE date_of_birth dob DATE;
  ```
- **SQL Server:**
  ```sql
  EXEC sp_rename 'employees.date_of_birth', 'dob', 'COLUMN';
  ```
- **PostgreSQL:**
  ```sql
  ALTER TABLE employees
  RENAME COLUMN date_of_birth TO dob;
  ```

### **Use Case:**
Renaming the `date_of_birth` column to `dob` for brevity.
