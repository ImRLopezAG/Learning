- **Explanation:** Stored procedures are prepared SQL codes that can be saved and reused.
- **Syntax:**
  ```sql
  CREATE PROCEDURE insert_employee (
    IN first_name VARCHAR(50),
    IN last_name VARCHAR(50),
    IN department VARCHAR(50)
  )
  BEGIN
    INSERT INTO employees (first_name, last_name, department)
    VALUES (first_name, last_name, department);
  END;
  ```
- **Example:**
  ```sql
  CALL insert_employee('Jane', 'Smith', 'Marketing');
  ```
- **Use Cases:** Reusable insert logic, encapsulation.

## See

### [Stored Procedures](../Performance/Stored%20Procedures.md)
