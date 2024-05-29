### **Explanation:**
Indexes are used to speed up the retrieval of data from a database table by creating a data structure that allows for faster searching.

### **Syntax:**
```sql
CREATE INDEX index_name
ON table_name (column1, column2, ...);
```

### **Example:**
```sql
CREATE INDEX idx_department
ON employees (department);
```

### **Use Case:**
Improving the performance of queries that filter by the `department` column.