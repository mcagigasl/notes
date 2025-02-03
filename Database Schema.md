A **database schema** refers to the structure that defines how data is organized within a [[database]]. It specifies the **tables**, their **columns**, the **types of data** that can be stored in those columns, as well as the **relationships** between different tables. In essence, a schema provides a blueprint for how the database is designed.

A schema can include:

1. **[[Tables]]**: A collection of data organized in rows and columns.
2. **[[Database View|Views]]**: Virtual tables that provide a specific view of the data.
3. **[[Vault Index|Indexes]]**: Structures that improve query performance.
4. **Relationships**: Definitions of how tables are related, such as throughs [[Primary Key|primary keys]] and **[[Foreign Key|foreign keys]]**.
5. **[[Constraints]]**: Rules for data integrity, like **NOT NULL**, **UNIQUE**, and **CHECK** constraints.

There are two primary types of database schemas:

- **Physical Schema**: Refers to the physical storage of the data (e.g., file systems, disk storage).
- **Logical Schema**: Refers to the design of the database in terms of the organization of tables, relationships, and constraints, without considering how the data is stored.

### Example:

For a simple **employee database**, the schema might define:

- An `Employee` table with columns like `EmployeeID`, `Name`, `Department`, and `Salary`.
- A `Department` table with `DepartmentID` and `DepartmentName`.
- A relationship between the `Employee` and `Department` tables via a foreign key on `DepartmentID`.

### Summary:

A **database schema** provides the structural design and relationships of a database. It's a critical component for ensuring that data is stored efficiently and can be queried in meaningful ways.

(A) What are primary and foreign keys in relational databases?  
(B) How do indexes improve database query performance?  
(C) What is normalization in database design?