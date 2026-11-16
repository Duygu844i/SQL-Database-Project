# SQL & Relational Database Design Project

**Author:** Duygu Hasanli  
**DBMS Used:** SQLite (DB Browser for SQLite)  

## 📌 Overview
This repository contains the complete SQL implementation, analytical business scenario solutions, and Entity-Relationship Diagrams (ERDs) developed for the **SQL & Relational Database Design** practical assignment.

---

## 📂 Repository Contents

| File Name | Description |
| :--- | :--- |
| `SalesDB_Solutions.sql` | Complete SQLite script containing schema creation (`CREATE TABLE`), sample data population (`INSERT INTO`), foundational queries (`B01–B10`), and 48 analytical queries across six business scenarios (`1.1–6.10`). |
| `SQL Assignment.docx` | Compiled analytical report featuring query output tables, required technical justifications (filtering logic, `LEFT JOIN` vs. `INNER JOIN` behavior, `WHERE` clause safety), and ERD relationship explanations. |
| `ERD_Project_A.pdf` | Entity-Relationship Diagram for the **Sales Management Database** (`Customers`, `Products`, `Employees`, `Orders`), including primary/foreign keys, cardinality, and self-referencing manager hierarchy. |
| `ERD_Project_B.pdf` | Entity-Relationship Diagram for the **University Course Registration System** (`Students`, `Instructors`, `Courses`, `Enrollments`), resolving many-to-many relationships and enforcing unique enrollment constraints. |

---

## 📊 Key Modules Covered

### 1. Foundational SQL (`B01–B10`)
* Data retrieval, filtering (`WHERE`, `IN`, `BETWEEN`, `LIKE`), sorting (`ORDER BY`), distinct selection, inner joins, aggregations (`GROUP BY`), and safe DML operations (`INSERT`, `UPDATE`, `DELETE`).

### 2. Business Scenario Analysis (`1.1–6.10`)
* **Scenario 1 — Customer Loyalty & Sales Analysis:** Customer segmentation, inactive account detection via `LEFT JOIN`, and top revenue ranking.
* **Scenario 2 — Order & Delivery Investigation:** Date-difference calculations (`julianday`), pending shipment tracking, and safe record updates.
* **Scenario 3 — Products & Employee Performance:** Inventory pricing analysis, unsold product detection, and `UNION` directory merging.
* **Scenario 4 — Targeted Campaign Planning:** Multi-table joins, cross-category intersection (`INTERSECT`), and cross-sell segmentation (`EXCEPT`).
* **Scenario 5 — Fulfilment Exception Desk:** Data integrity audits (inconsistent shipping dates, missing addresses) and workload balancing.
* **Scenario 6 — Sales Team Review & Retention:** Organizational hierarchy mapping (`SELF JOIN`), manager team summaries, and period-over-period retention (`October` vs. `November 2026`).

### 3. Relational Database Modeling (ERDs)
* **Project A:** Normalized 4-table sales schema with `1:N` optional relationships and self-referencing employee supervision.
* **Project B:** Academic registration schema decomposing an `M:N` student-course relationship via an associative `Enrollments` entity with a composite `(StudentID, CourseID)` unique constraint.

---

## 🚀 How to Run
1. Open **DB Browser for SQLite** (or any SQLite-compatible environment).
2. Create a new database and navigate to the **Execute SQL** tab.
3. Load and run `SalesDB_Solutions.sql` to build the tables, populate records, and execute any query block.
