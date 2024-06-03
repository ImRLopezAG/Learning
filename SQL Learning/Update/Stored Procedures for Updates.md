- **Explanation:** Encapsulating update logic in a stored procedure.
- **Syntax:**
  ```sql
  CREATE PROCEDURE update_department (
    IN employee_id INT,
    IN new_department VARCHAR(50)
  )
  BEGIN
    UPDATE employees
    SET department = new_department
    WHERE id = employee_id;
  END;
  ```
- **Example:**
  ```sql
  CALL update_department(1, 'Engineering');
  ```
- **Use Cases:** Reusable update logic, encapsulation.

## See

### [Stored Procedures](../Performance/Stored%20Procedures.md)
