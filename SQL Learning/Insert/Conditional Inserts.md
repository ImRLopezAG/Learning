- **Explanation:** Conditional inserts can be managed using logic in the application layer or using procedures in SQL.
- **Syntax:**
  ```sql
  INSERT INTO table_name (column1, column2, ...)
  SELECT value1, value2, ...
  WHERE NOT EXISTS (SELECT 1 FROM table_name WHERE condition);
  ```
- **Example:**
  ```sql
  INSERT INTO employees (first_name, last_name, department)
  SELECT 'John', 'Doe', 'Sales'
  WHERE NOT EXISTS (SELECT 1 FROM employees WHERE first_name = 'John' AND last_name = 'Doe');
  ```
- **Use Cases:** Preventing duplicate records.

## See

### [WHERE](../Keywords/WHERE.md)
