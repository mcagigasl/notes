The **relational model** is the most widely used [[Data Model]], especially for **traditional relational databases** (e.g., **MySQL**, **PostgreSQL**, **Oracle**, **SQL Server**). It organizes data into **tables** (also called **relations**) consisting of rows (records) and columns (attributes). The data model is based on **set theory**, and it uses **keys** (primary and foreign keys) to ensure relationships between different tables.

## Key Features

* **Structured Data** (for RDBMS) stored in tables or collections (for NoSQL).
* **Transactional**: Often optimized for online transaction processing ([[OLTP]]), meaning they handle day-to-day operations of businesses (e.g., storing customer records, orders).
* **[[ACID]]** Compliance (Atomicity, Consistency, Isolation, Durability): Ensures reliable transactions.
* Typically use [[SQL]] (Structured Query Language) for querying data.
* **[[Database Normalization]]**: the process of organizing data to reduce redundancy and dependency by dividing large tables into smaller ones and ensuring relationships between them are logically sound.

