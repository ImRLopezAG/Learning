### **Explanation:**
Aggregate functions perform a calculation on a set of values and return a single value. Common aggregate functions include `COUNT()`, `SUM()`, `AVG()`, `MIN()`, and `MAX()`.

### **Syntax:**
```sql
SELECT aggregate_function(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT AVG(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Calculating the average salary of employees in the Sales department.

---

## **1. COUNT()**

### **Explanation:**
The `COUNT()` function returns the number of rows that match a specified condition.

### **Syntax:**
```sql
SELECT COUNT(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT COUNT(employee_id)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Counting the number of employees in the Sales department.

---

## **2. SUM()**

### **Explanation:**
The `SUM()` function returns the total sum of a numeric column.

### **Syntax:**
```sql
SELECT SUM(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT SUM(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Calculating the total salary expense for the Sales department.

---

## **3. AVG()**

### **Explanation:**
The `AVG()` function returns the average value of a numeric column.

### **Syntax:**
```sql
SELECT AVG(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT AVG(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Calculating the average salary of employees in the Sales department.

---

## **4. MIN()**

### **Explanation:**
The `MIN()` function returns the smallest value in a specified column.

### **Syntax:**
```sql
SELECT MIN(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT MIN(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Finding the lowest salary in the Sales department.

---

## **5. MAX()**

### **Explanation:**
The `MAX()` function returns the largest value in a specified column.

### **Syntax:**
```sql
SELECT MAX(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT MAX(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Finding the highest salary in the Sales department.

---

## **6. GROUP BY**

### **Explanation:**
The `GROUP BY` statement is used with aggregate functions to group the result set by one or more columns.

### **Syntax:**
```sql
SELECT column1, aggregate_function(column2)
FROM table_name
WHERE condition
GROUP BY column1;
```

### **Example:**
```sql
SELECT department, AVG(salary)
FROM employees
GROUP BY department;
```

### **Use Case:**
Calculating the average salary for each department.

---

## **7. HAVING**

### **Explanation:**
The `HAVING` clause was added to SQL because the `WHERE` keyword could not be used with aggregate functions. It is used to filter records that work on summarized `GROUP BY` results.

### **Syntax:**
```sql
SELECT column1, aggregate_function(column2)
FROM table_name
GROUP BY column1
HAVING aggregate_function(column2) condition;
```

### **Example:**
```sql
SELECT department, AVG(salary)
FROM employees
GROUP BY department
HAVING AVG(salary) > 50000;
```

### **Use Case:**
Finding departments where the average salary is greater than $50,000.

---

## **8. VARIANCE()**

### **Explanation:**
The `VARIANCE()` function returns the statistical variance of all values in a specified column.

### **Syntax:**
```sql
SELECT VARIANCE(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT VARIANCE(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Calculating the variance in salaries within the Sales department.

---

## **9. STDDEV()**

### **Explanation:**
The `STDDEV()` function returns the standard deviation of all values in a specified column.

### **Syntax:**
```sql
SELECT STDDEV(column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT STDDEV(salary)
FROM employees
WHERE department = 'Sales';
```

### **Use Case:**
Calculating the standard deviation of salaries within the Sales department.

---

## **10. COUNT DISTINCT**

### **Explanation:**
The `COUNT(DISTINCT column)` function returns the number of distinct (unique) values in a specified column.

### **Syntax:**
```sql
SELECT COUNT(DISTINCT column)
FROM table_name
WHERE condition;
```

### **Example:**
```sql
SELECT COUNT(DISTINCT department)
FROM employees;
```

### **Use Case:**
Counting the number of unique departments in the employees table.

---

## **Combining Aggregate Functions**

### **Explanation:**
You can combine multiple aggregate functions in a single query to get different summaries of your data.

### **Example:**
```sql
SELECT 
    department, 
    COUNT(employee_id) AS total_employees, 
    AVG(salary) AS average_salary, 
    MIN(salary) AS min_salary, 
    MAX(salary) AS max_salary
FROM employees
GROUP BY department;
```

### **Use Case:**
Getting a comprehensive summary of employee statistics for each department.
