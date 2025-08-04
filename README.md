# Elevate-Labs-Task-1

# E-commerce Database Schema

## Overview
This project involves designing a relational database schema for an **E-commerce** domain. It models core entities such as Customers, Products, Orders, Order Items, and Categories, and defines the relationships among them.

## Entities and Relationships
- **Category:** Represents product categories (e.g., Electronics, Clothing)
- **Product:** Items available for purchase, each belonging to a category.
- **Customer:** Buyers who place orders.
- **Order:** Purchases made by customers.
- **Order_Item:** Represents products within an order, including quantity and price.

The relationships include:
- Each Product belongs to one Category.
- Each Order is placed by one Customer.
- Each Order contains multiple Order Items.
- Each Order Item references one Product.

## Tables and Columns

- **Category**
  - `category_id` (Primary Key)
  - `name`

- **Product**
  - `product_id` (Primary Key)
  - `name`
  - `price`
  - `category_id` (Foreign Key to Category)

- **Customer**
  - `customer_id` (Primary Key)
  - `first_name`
  - `last_name`
  - `email` (Unique)

- **Order**
  - `order_id` (Primary Key)
  - `order_date`
  - `customer_id` (Foreign Key to Customer)

- **Order_Item**
  - `order_item_id` (Primary Key)
  - `order_id` (Foreign Key to Order)
  - `product_id` (Foreign Key to Product)
  - `quantity`
  - `price`


##  Files Included

| File Name           | Description                                    |
|---------------------|------------------------------------------------|
| `task-1_schema.sql`| SQL script to create database and all tables  |
| `task-1_ERdiagram1.drawio.png`    | Entity-Relationship (ER) diagram of the schema (Created without Code) |
| `task-1_ERdiagram2.dbdiagram.png`    | Entity-Relationship (ER) diagram of the schema (Created with Code) |
| `README.md`         | Project overview and usage instructions        |

---

##  How to Use

1. Open **MySQL Workbench**
2. Connect to your MySQL server
3. Run the SQL script `task-1_schema.sql` to create the schema and tables
4. Use `task-1_ERdiagram2.dbdiagram.png` to understand the schema structure visually
5. Also Use `task-1_ERdiagram1.drawio.png` to understand the schema structure visually

##  Concepts Applied

- SQL DDL: `CREATE TABLE`, `PRIMARY KEY`, `FOREIGN KEY`
- Use of `AUTO_INCREMENT`
- ER Diagram Design

##  Author

**Mohammed Arman Mohammed Aslam Jogle**  
SQL Developer Intern  
4th August 2025
