# DBMS-project
# Employee and Department Database Project

## 📌 Project Description
This project is a database management system created using MySQL in XAMPP. It contains two tables: EMPLOYEE and DEPARTMENT. The project demonstrates the use of SQL commands such as table creation with constraints, data insertion, updating records, and retrieving information using queries.

The main objective of this project is to understand relational databases, primary keys, foreign keys, and SQL operations like SELECT, UPDATE, and ORDER BY.

## 🗄️ Tables Used

### 1. DEPARTMENT Table
Stores department information.

Columns:
- DEPTNO (Primary Key)
- DNAME (Department Name)

### 2. EMPLOYEE Table
Stores employee details.

Columns:
- EMPNO (Primary Key)
- ENAME (Employee Name)
- JOB
- MGR (Manager ID)
- HIREDATE
- SAL (Salary)
- COMM (Commission)
- DEPTNO (Foreign Key referencing DEPARTMENT)

## 🚀 Features
- Create tables with constraints (Primary Key & Foreign Key)
- Insert employee and department records
- Update salary with increment conditions
- Calculate annual salary and allowances
- Display employees based on conditions
- Perform sorting and filtering operations

## 🛠️ Technologies Used
- MySQL
- XAMPP
- SQL

## ▶️ How to Run the Project
1. Install XAMPP on your system.
2. Start Apache and MySQL from the XAMPP Control Panel.
3. Open phpMyAdmin in your browser.
4. Create a new database.
5. Run the SQL queries provided in the project to create tables and insert data.

## 📊 Example Queries Implemented
- Display employee annual salary.
- Update salary by percentage increment.
- Calculate HRA, DA, PF and total salary.
- Retrieve employees based on salary conditions.
- Sort employees by highest salary.

## 🎯 Learning Outcomes
- Understanding relational database design
- Working with SQL constraints
- Writing SELECT and UPDATE queries
- Performing calculations using SQL
- Managing data in MySQL

## 👨‍💻 Author
Vishal Mansuriya
Amar Singh Yadav
IILM University Greater Noida
