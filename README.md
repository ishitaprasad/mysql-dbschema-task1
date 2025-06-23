# mysql-dbschema-task1
Task 1 of SQL developer internship: setup a database and create a schema. Contains five tables for a retail management system.

# Retail Management System Database
This project contains the SQL schema and ER diagram for a simplified Retail Management System. It demonstrates how to model customers, products, categories, suppliers, and orders using SQL with appropriate relationships and sample data. 

# Contents:

1. schema.sql: SQL script to create tables and insert sample data using MySQL Workbench.
2. retail-er-diagram.png : Visual ER diagram showing entity relationships.
3. table-screenshots.png : Screenshots of the tables used in this database.
4. README.md : Project overview and usage guide.

##  Schema Overview

The database includes the following entities:

1. Customer – stores customer details. (CUSTID- primary key, name, email, phone address)
2. Category – product categories. (CATID- primary key, catgeory name)
3. Supplier – supplier contact info. (SUPID- primary key, email, name)
4. Product – product info, linked to category and supplier. (PRODID- primary key, name, price, stock, category, supplier) {CATID, SUPID FK)
5. Orders – a flat order table combining order details and items. (ORDERID & PRODID- composite key, CUSTID, orderdate, qty, amount) (PRODID, CUSTID FK)

Relationships are managed via primary and foreign keys. Each order row links a customer to a product with quantity and amount.


