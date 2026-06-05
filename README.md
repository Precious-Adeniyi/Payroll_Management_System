# 💼 Payroll Management System – Python & MySQL

## Overview
A desktop payroll management application built with Python 
and Tkinter, connected to a MySQL database. The system handles 
employee payroll calculations, record management, and data storage.

## Features
- Employee record management (Add, Update, Delete, Display)
- Automatic payroll calculations:
  - Tax (30% of Gross Pay)
  - Pension (2%)
  - Student Loan (1.2%)
  - NI Payment (1.1%)
  - Gross Pay and Net Pay
- Built-in calculator
- View Payroll tab with scrollable records table
- Notebook tab for payroll notes
- MySQL database integration

## Tools & Technologies
- Python
- Tkinter (GUI)
- pymysql (MySQL connection)
- MySQL Database

## How to Run
1. Install dependencies:
```bash
   pip install pymysql
```
2. Set up MySQL and create the database:
```sql
   CREATE DATABASE payment;
   USE payment;
   CREATE TABLE payment (
       ref VARCHAR(50), firstname VARCHAR(100),
       address VARCHAR(200), cityweighting FLOAT,
       basicsalary FLOAT, overtime FLOAT,
       grosspay VARCHAR(50), tax VARCHAR(50),
       pension VARCHAR(50), nipayment VARCHAR(50),
       deductions VARCHAR(50), postcode VARCHAR(20),
       gender VARCHAR(10), payday VARCHAR(20),
       taxperiod VARCHAR(20), taxcode VARCHAR(50),
       ninumber VARCHAR(50), netpay VARCHAR(50)
   );
```
3. Run the application:
```bash
   python payroll.py
```

## Screenshots
![Payroll System](Payroll_System/payroll.png)
