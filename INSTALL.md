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

# INSTALL

## Subqueries in SQL Language

This repository contains a **relational database creation and SQL query project** developed for the **Databases I (Database Management)** course at the **University of West Attica (UNIWA)**.  
It demonstrates database creation, schema definition, data insertion, and advanced SQL querying.

---

## 1. Prerequisites

Before using this project, ensure you have the following installed:

### 1.1 Database Management System (DBMS)

- **MySQL** (recommended)
- Compatible alternatives:
  - MariaDB
  - PostgreSQL _(minor syntax adjustments may be required)_

### 1.2 SQL Client / Interface

Any SQL client capable of executing `.sql` scripts:

- MySQL Workbench _(recommended)_
- phpMyAdmin
- DBeaver
- Command-line MySQL client

Make sure your SQL client is properly connected to your database server.

---

## 2. Installation

### 2.1 Clone the Repository

Open a terminal/command prompt and run:

```bash
git clone https://github.com/Data-Bases-1/SQL-Queries.git
```

### 2.2 Alternative (Without Git)

- Open the repository URL in your browser
- Click Code → Download ZIP
- Extract the ZIP file to a local directory

---

## 3. Database Setup

### 3.1 Locate the SQL Script

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

### 3.2 Execute the SQL Script

#### 3.2.1 Option A: Using MySQL Workbench / GUI Client

1. Open your SQL client
2. Create a new SQL tab
3. Open or paste the contents of new_personnel.sql
4. Execute the script (Run)

#### 3.2.2 Option B: Using MySQL Command Line

```bash
mysql -u your_username -p
```

Then:

```bash
SOURCE path/to/new_personnel.sql;
```

---

## 4. Verification

After successful execution, verify the setup:

### 4.1 Check Database

```sql
SHOW DATABASES;
USE new_personnel;
```

### 4.2 Check Tables

```sql
SHOW TABLES;
```

Expected tables:

- `DEPT`
- `EMP`
- `PROJ`
- `ASSIGN`

---

## 5. Inspect Table Structure

```sql
DESCRIBE DEPT;
DESCRIBE EMP;
DESCRIBE PROJ;
DESCRIBE ASSIGN;
```

---

## 6. Validate Sample Data

```sql
SELECT * FROM DEPT;
SELECT * FROM EMP;
SELECT * FROM PROJ;
SELECT * FROM ASSIGN;
```

---

## 7. Open the Documentation

1. Navigate to the `docs/` directory
2. Open the report corresponding to your preferred language:
   - English: `SQL-Queries.pdf`
   - Greek: `SQL-Ερωτήματα.pdf`
