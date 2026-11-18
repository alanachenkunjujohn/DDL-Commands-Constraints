# DDL-Commands-Constraints
This repository contains the SQL scripts and documentation focusing on **Data Definition Language (DDL)** commands and **database integrity constraints** using an Employee Management database schema.

## 📌 Project Overview

The objective of this assignment is to design, modify, and enforce data integrity rules on a relational database named `employee` consisting of three interconnected tables:
* `departments`
* `location`
* `employees`

## 🗂️ Repository Structure

* `DDL&CONSTRAINTS.sql` – Complete SQL script containing both Part 1 (DDL Commands) and Part 2 (Schema Recreation with Constraints).
* `MySQL Documentation` – Step-by-step documentation detailing the workflow, logic, and verification steps used to complete the assignment.
* `README.md` – Project overview and setup instructions.

## 🛠️ Key Concepts Covered

### Part 1: DDL Commands
* **`CREATE`**: Database and table creation with appropriate data types (`INT`, `VARCHAR`, `ENUM`, `DATE`, `DECIMAL`).
* **`ALTER`**: Adding columns (`email`), modifying column lengths (`designation`), dropping columns (`age`), and renaming columns (`hire_date` to `date_of_joining`).
* **`RENAME`**: Renaming tables (`departments` to `Departments_Info`, `location` to `Locations`).
* **`TRUNCATE`**: Removing all records from a table while preserving its structure.
* **`DROP`**: Deleting tables and databases safely.

### Part 2: Database Constraints
* **`PRIMARY KEY` & `AUTO_INCREMENT`**: Uniquely identifying departments, employees, and auto-generating sequential location IDs.
* **`NOT NULL` & `UNIQUE`**: Preventing missing or duplicate department names, locations, and employee names.
* **`ENUM` & `CHECK`**: Restricting `gender` values to `'M'` or `'F'` and enforcing a minimum employee `age` of 18.
* **`DEFAULT`**: Automatically assigning the current system date (`CURRENT_DATE`) to `hire_date` when omitted.
* **`FOREIGN KEY`**: Establishing referential integrity between `employees`, `departments`, and `location`.

