- **Explanation:** Using transactions to ensure safe delete operations.
- **Syntax:**
  ```sql
  BEGIN TRANSACTION;
  DELETE FROM employees WHERE condition;
  COMMIT;
  -- Or use ROLLBACK in case of error
  ```
- **Example:**
  ```sql
  BEGIN TRANSACTION;
  DELETE FROM employees WHERE last_name = 'Doe';
  COMMIT;
  ```
- **Use Cases:** Ensuring data integrity during delete operations.

## See

### [TRANSACTIONS](../Keywords/TRANSACTIONS.md)
