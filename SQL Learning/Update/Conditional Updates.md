- **Explanation:** Updating records based on certain conditions.
- **Syntax:**
  ```sql
  UPDATE table_name
  SET column1 = value1, column2 = value2, ...
  WHERE condition;
  ```
- **Example:**
  ```sql
  UPDATE employees
  SET department = 'Marketing'
  WHERE department = 'Sales' AND hire_date < '2020-01-01';
  ```
- **Use Cases:** Bulk updates with specific criteria.

## See

### [WHERE](../Keywords/WHERE.md)
