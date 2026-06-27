# 📚 Book Shop Management System

## Overview

The Book Shop Management System is a Python and MySQL-based application designed to manage bookstore operations efficiently. The system provides features for inventory management, book sales, stock monitoring, user authentication, and sales analysis through a menu-driven interface.

This project helps bookstore owners maintain accurate records of books, track sales, manage stock availability, and generate sales reports.

---

## Features

### 🔐 User Authentication

* User Registration
* Secure Login System
* Multiple User Support

### 📦 Inventory Management

* Add New Books to Stock
* View Available Stock
* Update Existing Stock
* Automatic Book Number Generation

### 🛒 Sales Management

* Sell Books
* Generate Purchase Records
* Update Available Stock Automatically
* Track Monthly Sales

### 📊 Sales Analytics

* Monthly Sales Visualization
* Bar Chart Reports using Matplotlib
* Sales Tracking by Book

### 🗄 Database Management

* MySQL Database Integration
* Automated Table Creation
* Data Persistence
* Foreign Key Relationships

---

## Technology Stack

| Technology                  | Purpose                 |
| --------------------------- | ----------------------- |
| Python                      | Application Development |
| MySQL                       | Database Management     |
| PyMySQL / MySQL Connector   | Database Connectivity   |
| Matplotlib                  | Sales Visualization     |
| Object-Oriented Programming | Code Structure          |

---

## Project Structure

```
Book-Shop-Management-System/
│
├── Main.py
│   ├── Main Menu
│   ├── Login & Registration
│   └── Navigation Controller
│
├── Book.py
│   ├── Inventory Management
│   ├── Book Sales
│   ├── User Authentication
│   ├── Stock Updates
│   └── Sales Analytics
│
├── Tables_in_mysql.py
│   ├── Database Creation
│   ├── Table Creation
│   └── Initial Setup
│
└── README.md
```

---

## Database Schema

### Database Name

```sql
book_shop
```

### Table: stock

| Column          | Type                 |
| --------------- | -------------------- |
| Book_No         | BIGINT (Primary Key) |
| Book_Name       | VARCHAR(255)         |
| Author          | VARCHAR(255)         |
| Publisher       | VARCHAR(255)         |
| Cost_per_Book   | FLOAT                |
| Available_Stock | BIGINT               |
| qty_purchased   | BIGINT               |
| purchased_on    | DATE                 |

### Table: users

| Column   | Type         |
| -------- | ------------ |
| username | VARCHAR(255) |
| password | VARCHAR(255) |

### Table: purchased

| Column       | Type   |
| ------------ | ------ |
| Book_No      | BIGINT |
| purchased_on | DATE   |

---

## Installation

### Step 1: Install Python

Download Python from:

https://www.python.org/downloads/

### Step 2: Install MySQL

Download MySQL Server:

https://www.mysql.com/downloads/

### Step 3: Install Required Libraries

```bash
pip install pymysql
pip install mysql-connector-python
pip install matplotlib
```

Or install all together:

```bash
pip install pymysql mysql-connector-python matplotlib
```

---

## Database Setup

Run the database initialization script:

```bash
python Tables_in_mysql.py
```

This will automatically:

* Create the `book_shop` database
* Create required tables
* Create indexes
* Configure relationships

---

## Running the Application

Start the application using:

```bash
python Main.py
```

---

## Application Workflow

### Main Menu

```
1. Register
2. Login
3. Exit
```

### Inventory Management

```
1. Add New Stock
2. View Stock
3. Update Stock
4. Exit
```

### Sales Management

```
1. Sell a Book
2. View Monthly Sales
3. Exit
```

---

## Key Functionalities

### Add New Stock

* Enter book details
* Store inventory records
* Generate unique book numbers

### View Stock

* Display all books
* Show available quantities
* Monitor inventory levels

### Sell Books

* Record customer purchases
* Reduce stock automatically
* Generate purchase receipts

### Sales Analysis

* Monthly sales report generation
* Graphical visualization using Matplotlib
* Book-wise sales tracking

---

## Future Enhancements

* GUI using Tkinter
* Barcode Scanner Integration
* Customer Management Module
* Invoice PDF Generation
* Search and Filter Books
* Online Book Ordering
* Admin Dashboard
* GST Billing Support
* Export Reports to Excel

---

## Academic Information

**Project Title:** Book Shop Management System

**Category:** Database Management System (DBMS)

**Language:** Python

**Database:** MySQL

**Type:** Console-Based Application

---

## Developed By

**Aditya Prakash Purohit**

B.Tech Student

Python Developer | Database Management Enthusiast

---

## License

This project is developed for educational and academic purposes.

You are free to use, modify, and enhance this project for learning and research.
