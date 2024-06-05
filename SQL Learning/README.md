# Getting Start

To Getting start with this learning path, you could use the fallowing tools:

- [Docker](https://www.docker.com/)
- [MS SQL Server](https://hub.docker.com/_/microsoft-mssql-server)
- [Azure Data Studio](https://docs.microsoft.com/en-us/sql/azure-data-studio/download?view=sql-server-ver15)
- [VS Code](https://code.visualstudio.com/)

Or whatever relational database you prefer like.

- [PostgreSQL](https://www.postgresql.org/)
- [MySQL](https://www.mysql.com/)
- [SQLite](https://www.sqlite.org/index.html)

Also to practice I recommend use an data warehouse like:

- [AdventureWorks](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms)
- [Northwind](https://github.com/anasmorahhib/Northwind-datawarehouse/blob/master/northwind.sql)
- [WideWorldImporters](https://learn.microsoft.com/en-us/sql/samples/wide-world-importers-install-configure?view=sql-server-ver16&tabs=ssms)

## Docker command to run MS SQL Server:

```bash
docker run --platform linux/amd64 \
   -e "ACCEPT_EULA=Y"\
   -e "MSSQL_SA_PASSWORD=<Your Strong password>" \
   -p 1433:1433 --name mssql --hostname mssql \
   -d \
   mcr.microsoft.com/mssql/server:2022-latest
```

The platform flag is used to specify the platform to run the container on. This is necessary when running on Mac.

## Docker command to run PostgreSQL:

```bash
docker run \
   -e POSTGRES_USER=postgres \
   -e POSTGRES_PASSWORD=<Your Strong password> \
   -p 5432:5432 --name pgsql --hostname pgsql \
   -d \
   postgres:alpine
```

## Docker command to run MySQL:

```bash
docker run \
   -e MYSQL_ROOT_PASSWORD=<Your Strong password> \
   -p 3306:3306 --name mysql --hostname mysql \
   -d \
   mysql:latest
```

## Docker command to run SQLite:

```bash
docker run \
   -p 1433:1433 --name sqlite --hostname sqlite \
   -d \
   sqlite:latest
```

## Table of Contents

### [Insert Statement](./Insert%20Statement.md)

### [Select Statement](./Select%20Statement.md)

### [Update Statement](./Update%20Statement.md)

### [Delete Statement](./Delete%20Statement.md)

### [Columns](./Columns.md)

## Technical questions

Here we have some technical questions that you can use to practice your SQL skills.

### **Basic**
### **SELECT Queries**

1. Retrieve the first and last names of all employees.
2. Find all products that have a list price greater than $1000.
3. Retrieve sales orders where the order date is in the year 2023.
4. Find the names and emails of all customers living in 'New York'.
5. Join the FactInternetSales table with the DimProduct table to retrieve product names and their total sales amounts.
6. Get the sales order numbers and the corresponding customer names.
7. Find the total sales amount for each product category.
8. Retrieve the average sales amount per order, grouped by year.
9. Retrieve the top 5 customers by total sales amount.
10. Find the product names and their average review scores.
11. Find all sales orders that were placed in the last month.
12. Find all employees who were hired in the year 2020.
13. Get the number of products in each product subcategory.
14. Retrieve the names of customers who placed more than 10 orders.
15. Find the total sales amount and average sales amount per order for each customer.

### **INSERT Queries**

16. Add a new product to the DimProduct table.
17. Insert a new employee into the DimEmployee table.
18. Insert multiple new rows into the DimCustomer table in one statement.
19. Add a new sales order to the FactInternetSales table.
20. Insert data into a temporary table from an existing table.
21. Insert the top 3 products by sales amount into a new table called TopSellingProducts.
22. Add a new row to the DimProductSubcategory table.
23. Use the INSERT INTO ... SELECT statement to insert data from one table into another.
24. Insert a new department into the DimDepartment table.
25. Insert a new customer with a default value for the email address.

### **UPDATE Queries**

26. Update the list price of a product with a specific ProductKey.
27. Update the email address of a customer with a specific CustomerKey.
28. Update the sales amount of all orders in the FactInternetSales table by increasing it by 10%.
29. Update the color of all products in a specific subcategory.
30. Update the address of a specific employee in the DimEmployee table.
31. Set the safety stock level of all products to 100 in the DimProduct table.
32. Update the job title of an employee with a specific EmployeeKey.
33. Update multiple columns in the DimCustomer table for a specific customer.
34. Reset the list price of all products to their original values if they are currently higher than $1000.
35. Update the reorder point of products in the 'Bikes' category by adding 10 to the current value.

### **DELETE Queries**

36. Delete a product from the DimProduct table with a specific ProductKey.
37. Delete all sales orders in the FactInternetSales table that were placed before the year 2020.
38. Delete a customer from the DimCustomer table with a specific CustomerKey.
39. Delete all products with a zero list price.
40. Delete all employees who were hired before the year 2000.
41. Delete duplicate rows from the DimProductSubcategory table.
42. Delete all sales orders with a total due less than $10.
43. Delete rows from a table based on a condition in another table.
44. Delete a specific department from the DimDepartment table.
45. Delete all inactive customers from the DimCustomer table.

### **Aggregate Functions**

46. Calculate the average sales amount per order in the FactInternetSales table.
47. Find the minimum and maximum sales amount for each product category.
48. Count the number of products in each product subcategory.
49. Find the total sales amount for each year.
50. Calculate the sum of the safety stock levels for all products in the DimProduct table.

---

These tasks cover a wide range of SQL operations and will help you practice and demonstrate your SQL expertise using the AdventureWorksDW database.

### **Advanced**


### **Complex SELECT Queries with Joins**

1. Retrieve the first and last names of employees along with their department names.
2. Find the total sales amount for each product category, including only orders placed in the last year.
3. Retrieve product names, subcategory names, and the corresponding total sales amounts.
4. Find the names and email addresses of customers who have purchased 'Mountain Bikes'.
5. Join the FactInternetSales, DimProduct, and DimCustomer tables to find the total sales amount for each customer.
6. Retrieve the first and last names of employees who report to a specific manager.
7. Find the top 5 products by sales amount for each product subcategory.
8. Retrieve the product names, category names, and their average list prices.
9. Find the names and sales amounts of the top 10 customers by total sales amount.
10. Retrieve the order numbers, customer names, and the names of the products they purchased.

### **Advanced INSERT Queries**

11. Insert multiple new products into the DimProduct table based on a SELECT statement from another table.
12. Add new employees to the DimEmployee table, setting default values for their hire dates.
13. Insert new sales orders into the FactInternetSales table, ensuring that the order numbers are unique.
14. Insert data into a temporary table from a complex SELECT statement involving multiple joins.
15. Add multiple new departments to the DimDepartment table, ensuring no duplicates.
16. Insert rows into the DimCustomer table based on customer data in a staging table.
17. Add new products to the DimProduct table, using a subquery to determine the correct subcategory.
18. Insert sales order data into the FactInternetSales table, ensuring referential integrity.
19. Add rows to the DimEmployee table, setting a default department for all new employees.
20. Insert customer data into the DimCustomer table, using a SELECT statement with joins to clean the data.

### **Complex UPDATE Queries**

21. Update the list prices of products based on their subcategory average list prices.
22. Increase the salaries of employees in the Sales department by 5%.
23. Update the email addresses of customers who have not placed an order in the last year to a default value.
24. Adjust the reorder points of products based on their sales performance over the last year.
25. Update the job titles of employees who have been with the company for more than 10 years.
26. Set the safety stock levels of products in the 'Bikes' category based on their sales volumes.
27. Update the contact information of customers who have placed more than 5 orders.
28. Increase the list prices of products in the 'Accessories' category by 10%.
29. Update the department of employees who report to a specific manager.
30. Adjust the standard costs of products based on their most recent purchase prices.

### **Complex DELETE Queries**

31. Delete all sales orders that were placed before the year 2000.
32. Remove all products from the DimProduct table that have never been sold.
33. Delete customer records from the DimCustomer table that have invalid email addresses.
34. Remove employees from the DimEmployee table who have left the company.
35. Delete all duplicate rows from the DimProductSubcategory table.
36. Remove sales orders from the FactInternetSales table that have a total due of less than $5.
37. Delete customer records from the DimCustomer table who have not placed an order in the last 5 years.
38. Remove all inactive departments from the DimDepartment table.
39. Delete product records from the DimProduct table that have a list price of zero.
40. Remove employees from the DimEmployee table who belong to departments that no longer exist.

### **Stored Procedures and Views**

41. Create a stored procedure to retrieve customer details by email address.
42. Write a stored procedure to update the list price of a product based on its ProductKey.
43. Create a view to display the total sales amount for each product category.
44. Write a stored procedure to insert a new sales order into the FactInternetSales table.
45. Create a view to show the average sales amount per order for each customer.
46. Write a stored procedure to delete a customer based on their CustomerKey.

47. Create a view to display the total sales amount for each customer by year.
48. Write a stored procedure to update customer email addresses based on a list of CustomerKeys.
49. Create a view to show the total and average list prices of products by subcategory.
50. Write a stored procedure to insert new products into the DimProduct table, ensuring no duplicates.

### **Advanced Queries with Filters and Joins**

51. Retrieve the names of products along with their total sales amount, but only for products with sales above $10,000.
52. Find the employees who have worked in more than one department.
53. Retrieve the names of customers who have placed orders in multiple years.
54. Find the total sales amount for each product, excluding sales from the 'Accessories' category.
55. Retrieve the top 10 products by total sales amount, excluding products that have not been sold in the last year.
56. Find the names and email addresses of customers who have made purchases above a specific amount in the last year.
57. Retrieve the total sales amount for each customer, including only orders placed in the last six months.
58. Find the employees who have received a promotion in the last five years.
59. Retrieve the names of products and their total sales amount, grouped by their subcategories.
60. Find the average sales amount per order for customers who have placed more than 20 orders.

### **Combining Aggregations and Joins**

61. Retrieve the total and average sales amounts for each product, grouped by product category.
62. Find the total number of products sold for each product subcategory, including only products that have been reviewed.
63. Retrieve the names of customers and the total sales amount for each, but only include customers who have made more than three purchases.
64. Find the total sales amount for each product, grouped by month and year.
65. Retrieve the average list price of products, grouped by product subcategory and category.
66. Find the total sales amount for each customer, grouped by the year they made the purchase.
67. Retrieve the names of employees and the total sales amount for each, grouped by the departments they have worked in.
68. Find the total and average sales amounts for each product, grouped by the customers who purchased them.
69. Retrieve the total number of sales orders and the total sales amount, grouped by the year and month of the order date.
70. Find the total sales amount for each product category, grouped by the regions where the products were sold.

### **Complex Subqueries and Common Table Expressions (CTEs)**

71. Write a query to find the products with sales amounts above the average sales amount for their category.
72. Use a subquery to find the customers who have spent more than the average amount across all customers.
73. Create a CTE to find the top 5 employees by total sales amount and retrieve their details.
74. Write a query using a subquery to find the products that have never been sold.
75. Use a CTE to find the total sales amount for each product category and retrieve categories with total sales above $50,000.
76. Write a query using a subquery to find the customers who have not placed an order in the last year.
77. Create a CTE to find the employees with more than 10 years of service and retrieve their department details.
78. Write a query using a subquery to find the total sales amount for the top 3 products in each category.
79. Use a CTE to find the total and average sales amounts for each customer and retrieve customers with average sales above $1000.
80. Write a query using a subquery to find the products that have been reviewed more than 5 times.

### **Combining Stored Procedures and Transactions**

81. Create a stored procedure to insert a new customer and their initial sales order in a single transaction.
82. Write a stored procedure to update product prices and log the changes in a history table.
83. Create a stored procedure to delete a sales order and update the stock levels of the associated products in a single transaction.
84. Write a stored procedure to insert multiple new employees and their department assignments in a single transaction.
85. Create a stored procedure to transfer an employee to a different department and update their records in a single transaction.
86. Write a stored procedure to insert a new product and update the product count in the related category table in a single transaction.
87. Create a stored procedure to delete a customer and their associated sales orders in a single transaction.
88. Write a stored procedure to update the reorder point of products and log the changes in a history table.
89. Create a stored procedure to archive old sales orders and delete them from the active table in a single transaction.
90. Write a stored procedure to insert new sales data and update related customer and product information in a single transaction.

### **Advanced Data Management Tasks**

91. Add a new column `LastOrderDate` to the DimCustomer table and update it with the date of the most recent order for each customer.
92. Rename the `PhoneNumber` column to `ContactNumber` in the DimEmployee table.
93. Delete the `MiddleName` column from the DimCustomer table.
94. Modify the data type of the `ListPrice` column in the DimProduct table to DECIMAL(18,2).
95. Add a new column `ReviewCount` to the DimProduct table and update it with the number of reviews for each product.
96. Rename the `Email` column to `EmailAddress` in the DimCustomer table.
97. Delete the `Suffix` column from the DimEmployee table.
98. Modify the data type of the `StandardCost` column in the DimProduct table to DECIMAL(18,2).
99. Add a new column `OrderCount` to the DimCustomer table and update it with the total number of orders for each customer.
100. Rename the `Title` column to `JobTitle` in the DimEmployee table.
---

These tasks will challenge your ability to work with complex SQL operations and enhance your understanding of advanced SQL concepts using the AdventureWorksDW database.