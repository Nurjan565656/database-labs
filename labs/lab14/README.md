# Lab 14
# Joining Tables Lab

## Description
This project focuses on SQL JOIN operations in PostgreSQL. The main purpose is to understand how data stored in different tables can be combined using related columns and foreign key relationships.

## Database Structure
The database contains five tables:

- `customers` – stores customer information, including names and email addresses.
- `orders` – contains customer orders, their dates, and total amounts.
- `products` – stores product names and prices.
- `order_items` – connects orders with products and stores the quantity of each product.
- `employees` – contains employee information and manager relationships.

## Topics Covered

### 1. INNER JOIN
Returns only records that have matching values in both tables. It is useful when we need to display related information, such as customers who have placed orders.

### 2. LEFT JOIN
Returns all records from the left table and matching records from the right table. If there is no match, the columns from the right table contain `NULL`. This is useful for finding customers who have not placed any orders.

### 3. RIGHT JOIN
Returns all records from the right table and matching records from the left table. It helps display all orders, even when matching customer information is missing.

### 4. FULL OUTER JOIN
Combines the results of LEFT JOIN and RIGHT JOIN. It returns all records from both tables, including unmatched records, with `NULL` values where no relationship exists.

### 5. CROSS JOIN
Combines every row from the first table with every row from the second table. This creates a Cartesian product and is useful when we need all possible combinations of records.

### 6. Multiple Table JOINs
Allows us to combine data from more than two tables in one query. For example, we can connect customers, orders, order items, and products to see which products each customer purchased.

### 7. SELF JOIN
A SELF JOIN joins a table with itself. It is useful for working with hierarchical relationships, such as connecting employees with their managers through the `manager_id` column.

### 8. JOIN with Conditions
Additional conditions can be used with JOIN operations. The `WHERE` clause allows us to filter the combined results, for example, by order date or order amount.

### 9. Relationship Types
The database demonstrates how tables can be connected through relationships. Customers and orders represent a one-to-many relationship, while orders and products have a many-to-many relationship through the `order_items` junction table.

## Conclusion
This lab demonstrates how SQL JOIN operations help combine related data from multiple tables. It also provides practice with foreign keys, table aliases, filtering conditions, and different types of relationships in a relational database.
