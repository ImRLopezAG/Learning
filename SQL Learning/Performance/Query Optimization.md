### **Explanation:**
Optimizing queries involves rewriting them to run more efficiently. This can include restructuring queries, using appropriate joins, and avoiding unnecessary computations.

### **Strategies:**
- **Use EXPLAIN:** Analyze the execution plan of your queries.
  ```sql
  EXPLAIN SELECT * FROM employees WHERE department = 'Sales';
  ```
- **Avoid SELECT *:** Specify only the columns you need.
  ```sql
  SELECT first_name, last_name FROM employees WHERE department = 'Sales';
  ```
- **Use Proper Joins:** Choose the correct type of join based on your data and query requirements.
- **Limit Rows Returned:** Use `LIMIT` to restrict the number of rows returned.
  ```sql
  SELECT first_name, last_name FROM employees LIMIT 10;
  ```
