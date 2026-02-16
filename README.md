<p align="center">
  <img src="https://www.especial.gr/wp-content/uploads/2019/03/panepisthmio-dut-attikhs.png" alt="UNIWA" width="150"/>
</p>

<p align="center">
  <strong>UNIVERSITY OF WEST ATTICA</strong><br>
  SCHOOL OF ENGINEERING<br>
  DEPARTMENT OF COMPUTER ENGINEERING AND INFORMATICS
</p>

---

<p align="center">
  <strong>Databases I</strong>
</p>

<h1 align="center">
  Subqueries in SQL Language
</h1>

<p align="center">
  <strong>Vasileios Evangelos Athanasiou</strong><br>
  Student ID: 19390005
</p>

<p align="center">
  <a href="https://github.com/Ath21" target="_blank">GitHub</a> ·
  <a href="https://www.linkedin.com/in/vasilis-athanasiou-7036b53a4/" target="_blank">LinkedIn</a>
</p>

<p align="center">
  Supervisor: Periklis Andritsos, Professor
</p>
<p align="center">
  <a href="https://ice.uniwa.gr/en/emd_person/periklis-andritsos/" target="_blank">UNIWA Profile</a> ·
  <a href="https://www.linkedin.com/in/periklisandritsos/" target="_blank">LinkedIn</a>
</p>

<p align="center">
  Co-supervisor: Anastasios Tsolakidis, Assistant Professor<br>
</p>

<p align="center">
  <a href="https://alis.uniwa.gr/en/profile/anastasios-tsolakidis" target="_blank">UNIWA Profile</a> ·
  <a href="https://www.linkedin.com/in/tasos-tsolakidis-35493930/" target="_blank">LinkedIn</a>
</p>

<p align="center">
  Athens, June 2023
</p>

---

# Project Overview

The project demonstrates the design and manipulation of a relational database that models a company’s personnel structure, departments, and project assignments.

---

## Table of Contents


| Section | Folder / File | Description |
|------:|---------------|-------------|
| 1 | `assign/` | Assignment material |
| 1.1 | `assign/assignment_02.pdf` | Assignment description (English) |
| 1.2 | `assign/εργασία_02.pdf` | Assignment description (Greek) |
| 2 | `docs/` | Theoretical documentation |
| 2.1 | `docs/SQL-Queries.pdf` | SQL queries theory and examples (English) |
| 2.2 | `docs/SQL-Ερωτήματα.pdf` | SQL queries theory and examples (Greek) |
| 3 | `src/` | SQL source code |
| 3.1 | `src/new_personnel.sql` | SQL script for personnel database queries |
| 4 | `README.md` | Repository overview and instructions |

---


## Database Schema

The database, named **`new_personnel`**, consists of four primary tables:

| Table  | Description                                              | Primary Key              |
|-------:|----------------------------------------------------------|--------------------------|
| DEPT   | Department details (Name, Location)                       | DEPTNO                   |
| EMP    | Employee records (Name, Job, Salary, Hire Date)           | EMPNO                    |
| PROJ   | Project descriptions                                     | PROJ_CODE                |
| ASSIGN | Relationship between Employees and Projects (Time spent) | (EMPNO, PROJ_CODE)       |

---

## Key SQL Operations

### 1. Data Initialization
The SQL scripts handle the complete setup of the database environment, including:

- Creation of the `new_personnel` database  
- Definition of all tables with **PRIMARY KEY** and **FOREIGN KEY** constraints  
- Population of sample data for departments such as:
  - Accounting (Athens)
  - Sales (London)
  - Research (Athens)

---

### 2. Complex Query Examples

The documentation includes several practical and advanced SQL exercises:

- **Financial Reporting**  
  Calculation of monthly employee earnings *(Salary + Commission)* and formatting results with currency symbols.

- **Service Calculation**  
  Use of `DATEDIFF` to compute years of service and filtering employees with more than **20 years** of experience.

- **Advanced Filtering**  
  Use of `SUBSTRING` and `BETWEEN` to identify employees hired on specific days of the month.

- **Correlated Subqueries**  
  Identification of employees who earn the **highest salary within their department**.

---

## Usage Summary

This document serves as a complete **laboratory report**, demonstrating proficiency in:

- **Data Definition Language (DDL)**  
  `CREATE`, `DROP`, and enforcement of table constraints  

- **Data Manipulation Language (DML)**  
  `INSERT` statements for populating database records  

- **Data Query Language (DQL)**  
  Advanced `SELECT` statements using:
  - `IFNULL`
  - `CONCAT`
  - `FORMAT`
  - Nested and correlated subqueries  

---

# Installation & Setup Guide

This repository contains a **relational database creation and SQL query project** developed for the **Databases I (Database Management)** course at the **University of West Attica (UNIWA)**.  
It demonstrates database creation, schema definition, data insertion, and advanced SQL querying.

---

## Prerequisites

Before using this project, ensure you have the following installed:

### 1. Database Management System (DBMS)
- **MySQL** (recommended)
- Compatible alternatives:
  - MariaDB
  - PostgreSQL *(minor syntax adjustments may be required)*

### 2. SQL Client / Interface
Any SQL client capable of executing `.sql` scripts:
- MySQL Workbench *(recommended)*
- phpMyAdmin
- DBeaver
- Command-line MySQL client

Make sure your SQL client is properly connected to your database server.

---

## Installation

### 1. Clone the Repository

Open a terminal/command prompt and run:

```bash
git clone https://github.com/Data-Bases-1/SQL-Queries.git
```

#### Alternative (Without Git)

- Open the repository URL in your browser
- Click Code → Download ZIP
- Extract the ZIP file to a local directory

---

## Database Setup
### 2. Locate the SQL Script
Navigate to:
```bash
src/new_personnel.sql
```
This file contains:
- Database creation statements
- Table definitions (`DEPT`, `EMP`, `PROJ`, `ASSIGN`)
- Primary and foreign key constraints
- Sample data insertion
- Example SQL queries

### 3. Execute the SQL Script
#### Option A: Using MySQL Workbench / GUI Client
1. Open your SQL client
2. Create a new SQL tab
3. Open or paste the contents of new_personnel.sql
4. Execute the script (Run)

#### Option B: Using MySQL Command Line
```bash
mysql -u your_username -p
```
Then:
```bash
SOURCE path/to/new_personnel.sql;
```
---

## Verification
After successful execution, verify the setup:
### Check Database
```sql
SHOW DATABASES;
USE new_personnel;
```

### Check Tables
```sql
SHOW TABLES;
```
Expected tables:
- `DEPT`
- `EMP`
- `PROJ`
- `ASSIGN`

---

## Inspect Table Structure
```sql
DESCRIBE DEPT;
DESCRIBE EMP;
DESCRIBE PROJ;
DESCRIBE ASSIGN;
```

---

## Validate Sample Data
```sql
SELECT * FROM DEPT;
SELECT * FROM EMP;
SELECT * FROM PROJ;
SELECT * FROM ASSIGN;
```

---

## Open the Documentation
1. Navigate to the `docs/` directory
2. Open the report corresponding to your preferred language:
    - English: `SQL-Queries.pdf`
    - Greek: `SQL-Ερωτήματα.pdf`