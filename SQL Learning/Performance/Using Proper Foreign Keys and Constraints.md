### **Explanation:**
Foreign keys and constraints enforce data integrity and can improve query performance by allowing the database optimizer to better understand relationships between tables.

### **Syntax:**
```sql
ALTER TABLE employees
ADD CONSTRAINT fk_department
FOREIGN KEY (department_id) REFERENCES departments(department_id);
```

### **Best Practices:**
- Define foreign keys to enforce referential integrity.
- Use constraints to ensure data validity (e.g., `CHECK`, `UNIQUE`).

---

By focusing on these performance-enhancing techniques, you can significantly improve the efficiency and responsiveness of your SQL queries and database operations. Understanding and applying these concepts will help you manage large datasets more effectively and ensure your applications run smoothly.