# 👟 Online Shoe Store Database Application
---

# 🛒 Project Overview

This project designs and implements a **robust database application** for an **online shoe store**, managing:

- 👥 Customer Management
- 📦 Inventory Tracking
- 🧾 Order Processing
- 🧑‍💼 Employee Management
- 🚚 Shipping Logistics

---

# 🎯 Project Objectives

1. **Database Design**
   - Create ER Schema Diagram (Conceptual Model)
   - Transform to 3NF Relational Model
   - Identify Entities, Attributes, Relationships, Constraints

2. **SQL Script Development**
   - Write DDL scripts for tables, relationships, constraints
   - Develop DML scripts for sample data insertion

3. **Database Implementation**
   - Execute scripts to build schema
   - Populate database with mock data

4. **Query Development & Testing**
   - Develop 12+ queries: joins, aggregates, subqueries, ORDER BY, HAVING
   - Test for performance and accuracy

5. **Documentation**
   - ER diagrams, relational models, schema documentation
   
---

# 🗺️ Conceptual Model (ER Schema Diagram)

### Entities & Attributes

- **Customers**: CustomerID (PK), FirstName, LastName, Email, Phone
- **Inventory**: ItemID (PK), Brand, Model, Size, Price, QuantityInStock
- **Orders**: OrderID (PK), CustomerID (FK), EmployeeID (FK), ShippingID (FK), OrderDate
- **Employees**: EmployeeID (PK), FirstName, LastName, Position
- **Shipping**: ShippingID (PK), ShipDate, DeliveryStatus

### Relationships

- Customers ➡️ Orders (1-to-Many)
- Orders ➡️ Inventory (1-to-Many)
- Orders ➡️ Employees (Many-to-1)
- Orders ➡️ Shipping (Many-to-1)

![image](https://github.com/user-attachments/assets/3be3f8e3-2480-4618-8ee1-104880831e8a)

---

# 🛠️ Relational Model in 3NF

| Table | Attributes |
| :--- | :--- |
| **Customers** | CustomerID (PK), FirstName, LastName, Email, Phone |
| **Employees** | EmployeeID (PK), FirstName, LastName, Position |
| **Inventory** | ItemID (PK), Brand, Model, Size, Price, QuantityInStock |
| **Shipping** | ShippingID (PK), ShipDate, DeliveryStatus |
| **Orders** | OrderID (PK), CustomerID (FK), EmployeeID (FK), ShippingID (FK), OrderDate |

- ✅ Reduces redundancy
- ✅ Ensures referential integrity
- ✅ Supports scalable business operations

---

# 💻 Implementation Details

### 📂 Schema Creation - `LPorter_cis556_schema.sql`

```sql
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    Email VARCHAR(100),
    Phone VARCHAR(20)
);

-- Other tables for Inventory, Orders, Employees, Shipping (see full scripts)
```

### 🗂️ Data Insertion - `LPorter_cis556_data.sql`

- Mock data generated via [Mockaroo](https://mockaroo.com/)

```sql
INSERT INTO Customers (CustomerID, FirstName, LastName, Email, Phone)
VALUES (1, 'Marylee', 'Brands', 'mbrands0@taobao.com', '410-982-2326');

-- More sample data for Inventory, Employees, Shipping, Orders
```
---

# 📈 Query Development

Developed 12 SQL Queries to test:

- 🔹 Single Table Queries
- 🔹 Multi-Table Joins
- 🔹 Aggregate Functions (SUM, AVG)
- 🔹 Subqueries
- 🔹 `ORDER BY`, `HAVING` clauses
---

# 📋 Conclusion

This project successfully delivers:

- ✅ Normalized Database Structure (3NF)
- ✅ Full DDL + DML SQL Scripts
- ✅ Sample Data Insertion
- ✅ Working Queries with tested results
- ✅ Project Documentation

---

# ✨ Tech Stack

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=sqlite&logoColor=white)
![Mockaroo](https://img.shields.io/badge/Mockaroo-FF6D00?style=for-the-badge&logo=data&logoColor=white)

---

# 📑 Files Included

- `LPorter_cis556_schema.sql` — Database Schema Creation Scripts
- `LPorter_cis556_data.sql` — Mock Data Insertion Scripts
- Screenshots — (ERD, Schema, Sample Queries) located in .docx file

---
# 🙌 Connect with Me!

🔗 [LinkedIn](https://www.linkedin.com/in/lashelleporter)  |  📧 [shellep@umich.edu](mailto:shellep@umich.edu)  |  🌎 Rockford, MI

---

🚀 **Project Completed by LaShelle Porter** — December 2023
