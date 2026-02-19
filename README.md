<p align="center">
  <img src="https://www.especial.gr/wp-content/uploads/2019/03/panepisthmio-dut-attikhs.png" alt="UNIWA" width="150"/>
</p>

<p align="center">
  <strong>UNIVERSITY OF WEST ATTICA</strong><br>
  SCHOOL OF ENGINEERING<br>
  DEPARTMENT OF COMPUTER ENGINEERING AND INFORMATICS
</p>

<p align="center">
  <a href="https://www.uniwa.gr" target="_blank">University of West Attica</a> ·
  <a href="https://ice.uniwa.gr" target="_blank">Department of Computer Engineering and Informatics</a>
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

<hr>

<p align="center">
  <strong>Supervision</strong>
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

---

<p align="center">
  Athens, June 2023
</p>

---

<p align="center">
  <img src="https://linuxiac.com/wp-content/uploads/2021/05/mysql-create-database-workbench.png" width="250"/>
</p>

---

# README

## Subqueries in SQL Language

The project demonstrates the design and manipulation of a relational database that models a company’s personnel structure, departments, and project assignments.

---

## Table of Contents

| Section | Folder / File              | Description                               |
| ------: | -------------------------- | ----------------------------------------- |
|       1 | `assign/`                  | Assignment material                       |
|     1.1 | `assign/assignment_02.pdf` | Assignment description (English)          |
|     1.2 | `assign/εργασία_02.pdf`    | Assignment description (Greek)            |
|       2 | `docs/`                    | Theoretical documentation                 |
|     2.1 | `docs/SQL-Queries.pdf`     | SQL queries theory and examples (English) |
|     2.2 | `docs/SQL-Ερωτήματα.pdf`   | SQL queries theory and examples (Greek)   |
|       3 | `src/`                     | SQL source code                           |
|     3.1 | `src/new_personnel.sql`    | SQL script for personnel database queries |
|       4 | `README.md`                | Project documentation                     |
|       5 | `INSTALL.md`               | Usage instructions                        |

---

## 1. Database Schema

The database, named **`new_personnel`**, consists of four primary tables:

|  Table | Description                                              | Primary Key        |
| -----: | -------------------------------------------------------- | ------------------ |
|   DEPT | Department details (Name, Location)                      | DEPTNO             |
|    EMP | Employee records (Name, Job, Salary, Hire Date)          | EMPNO              |
|   PROJ | Project descriptions                                     | PROJ_CODE          |
| ASSIGN | Relationship between Employees and Projects (Time spent) | (EMPNO, PROJ_CODE) |

---

## 2. Key SQL Operations

### 2.1 Data Initialization

The SQL scripts handle the complete setup of the database environment, including:

- Creation of the `new_personnel` database
- Definition of all tables with **PRIMARY KEY** and **FOREIGN KEY** constraints
- Population of sample data for departments such as:
  - Accounting (Athens)
  - Sales (London)
  - Research (Athens)

---

## 3. Complex Query Examples

The documentation includes several practical and advanced SQL exercises:

- **Financial Reporting**  
  Calculation of monthly employee earnings _(Salary + Commission)_ and formatting results with currency symbols.

- **Service Calculation**  
  Use of `DATEDIFF` to compute years of service and filtering employees with more than **20 years** of experience.

- **Advanced Filtering**  
  Use of `SUBSTRING` and `BETWEEN` to identify employees hired on specific days of the month.

- **Correlated Subqueries**  
  Identification of employees who earn the **highest salary within their department**.

---

## 4. Usage Summary

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
