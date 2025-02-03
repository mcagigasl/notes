---
aliases:
  - DBMS
---
DBMS stands for Database Management System, which, according with Connolly and Begg a DBMS is a "*software system that enables users to define, create, maintain and control access a  [[database]]*."  

A DBMS manages three aspects:
* [[Database Schema]]
* Database's logical structure
* Databases's engine
* 

### Key Orientations of DBMS:

1. **[[OLTP]] (Online Transaction Processing)**:
    
    - Focuses on managing day-to-day transactional data.
    - Typically used for applications that require high-speed processing of numerous small transactions (e.g., banking, e-commerce, order processing).
    - Characteristics include high concurrency, fast query responses, and frequent inserts/updates/deletes.
    - DBMS systems like **MySQL**, **PostgreSQL**, and **Oracle** are often used for OLTP workloads.
    - 
2. **[[OLAP]] (Online Analytical Processing)**:
    
    - Designed for analytical queries on large volumes of data.
    - Focuses on decision-making, reporting, and data analysis rather than real-time transaction processing.
    - OLAP systems typically involve complex queries, aggregation, and multidimensional data views (e.g., business intelligence systems, data warehousing).
    - DBMS systems used for OLAP include **Amazon Redshift**, **Google BigQuery**, and **Snowflake**.
      
3. **[[HTAP]] (Hybrid Transactional/Analytical Processing)**:
    
    - A newer class of databases designed to handle both OLTP and OLAP workloads within the same system.
    - This approach enables organizations to process real-time transactional data while simultaneously performing analytical queries without needing to replicate or move data between systems.
    - Some DBMS like **SAP HANA**, **MemSQL (now SingleStore)**, and **CockroachDB** support HTAP workloads.
      
4. **[[Non Relational Databases Systems|NoSQL DBMS]] Databases**:
    
    - NoSQL systems (like **MongoDB**, **Cassandra**, and **Couchbase**) are optimized for non-relational data models (e.g., document, key-value, column-family, graph), and they often excel at handling high volumes of unstructured or semi-structured data.
    - These databases can be used for both transactional (OLTP) and analytical (OLAP) purposes, depending on the specific use case.
    
1. **[[Distributed Databases]]**:
    
    - Many modern DBMS systems are distributed, and they can be designed to support both OLTP and OLAP workloads across a network of machines (e.g., **Apache Cassandra**, **Google Spanner**, **CockroachDB**).
    - These systems allow scalability, fault tolerance, and high availability, making them suitable for large-scale enterprise applications.

### Examples of DBMS Supporting Different Orientations:

- **OLTP**: Traditional relational databases like **MySQL**, **PostgreSQL**, **Oracle Database**, **SQL Server**.
- **OLAP**: Data warehousing solutions like **Google BigQuery**, **Amazon Redshift**, **Microsoft Azure Synapse**.
- **HTAP**: Platforms like **SAP HANA**, **SingleStore**, **CockroachDB**.

