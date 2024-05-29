### **Explanation:**
Database management systems use statistics to create query execution plans. Keeping these statistics up to date ensures the optimizer makes accurate decisions.

### **Commands:**
- **ANALYZE:** Collects statistics about the contents of tables.
  ```sql
  ANALYZE TABLE employees;
  ```
- **OPTIMIZE:** Reorganizes the table and updates statistics.
  ```sql
  OPTIMIZE TABLE employees;
  ```

### **Best Practices:**
- Regularly analyze and optimize tables, especially after large updates or inserts.
- Automate the process using maintenance scripts.
