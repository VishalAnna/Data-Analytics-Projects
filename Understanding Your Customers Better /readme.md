
# Sales Database

This repository contains SQL scripts to create a database for managing sales data, including sales orders, customer information, product details, and delivery regions. The database schema is designed to efficiently store and manage sales-related data.

## Table Structure

### Sales Orders (SALES.PUBLIC.SALES_ORDERS)
- `ORDERNUMBER`: Unique identifier for the sales order (VARCHAR)
- `ORDERDATE`: Date of the sales order (DATE)
- `CUSTOMER_NAME_INDEX`: Customer index as a primary key (NUMBER)
- `CHANNEL`: Sales channel (VARCHAR)
- `WAREHOUSE_CODE`: Warehouse code (VARCHAR)
- `DELIVERY_REGION_INDEX`: Index referencing delivery region (NUMBER)
- `PRODUCT_DESCRIPTION_INDEX`: Index referencing product description (NUMBER)
- `ORDER_QUANTITY`: Quantity of products ordered (NUMBER)
- `UNIT_PRICE`: Unit price of the product (NUMBER)
- `TOTAL_REVENUE`: Total revenue from the sales order (NUMBER)
- `TOTAL_UNIT_COST`: Total unit cost for the sales order (NUMBER)

### Customers (customers)
- `Customer_Index`: Unique identifier for customers (NUMBER)
- `Customer_Names`: Names of customers (VARCHAR)

### Regions (regions)
- `Index`: Unique identifier for regions (NUMBER)
- `City`: City name (VARCHAR)
- `Country`: Country name (VARCHAR)

### Products (products)
- `Index`: Unique identifier for products (NUMBER)
- `Product_Name`: Name of the product (VARCHAR)

## Data Loading

Data can be loaded into these tables using the provided SQL scripts. The dataset includes customer information, product details, sales orders, and delivery region information. The data is loaded from CSV files using a predefined file format.

## Master Table (VN_sales)

A master table named `VN_sales` is created by joining the sales orders table with customer, product, and region tables. This master table contains comprehensive information about sales transactions, including customer names, product names, city, country, and full addresses.

## Usage

You can use this database to perform various data analytics tasks, generate reports, and gain insights into sales data. The schema is designed to support efficient querying and reporting for sales-related activities.

Feel free to explore the provided SQL scripts and customize the database as needed for your specific data analytics requirements.
