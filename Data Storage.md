Data storage refers to the process of saving and preserving data in a way that allows it to be accessed, managed, and used when needed. There are three differents types of Data Storage: [[Database Management Systems]] or traditional databases, [[Data Warehouse]] and [[Data Lake]]. 

## **Key Differences:**

| Feature                 | **Traditional Databases** (DBMS)                              | **Data Lakes**                                          | **Data Warehouses**                                   |
| ----------------------- | ------------------------------------------------------------- | ------------------------------------------------------- | ----------------------------------------------------- |
| **Data Structure**      | Structured (tables, rows, columns) or semi-structured (NoSQL) | Raw, unstructured, semi-structured, and structured      | Structured (tables, columns, rows)                    |
| **Data Type**           | Primarily structured data                                     | Raw, unstructured (e.g., text, images, videos)          | Structured, cleaned data                              |
| **Use Case**            | Transactional processing (OLTP), daily operations             | Big data analytics, machine learning, data science      | Analytical queries (OLAP), business intelligence      |
| **Data Transformation** | Minimal transformation (normalization, indexing)              | Raw data, minimal or no transformation                  | Data is cleaned, transformed (ETL process)            |
| **Performance**         | Optimized for fast transactions (read/write)                  | Optimized for large-scale analytics and processing      | Optimized for complex analytical queries (read-heavy) |
| **Scalability**         | Typically scale vertically (single server)                    | Scales horizontally, cost-effective for massive amounts | Scales horizontally, but more costly than data lakes  |
| **Data Integrity**      | ACID compliance (transactional)                               | Not ACID-compliant; focus is on raw data storage        | Focuses on **data consistency** for analysis          |
| **Query Type**          | Fast transactional queries (OLTP)                             | Big data processing (e.g., Hadoop, Spark)               | Complex analytical queries (OLAP)                     |

### Summary:

- **Traditional Databases**: Used for **day-to-day transactional** operations with structured data. They focus on **[[ACID]] compliance** and are optimized for fast **read/write operations**.
- **Data Lakes**: Store large volumes of **raw, unstructured**, and **semi-structured data**, typically used for **big data analytics**, machine learning, and advanced processing. Data is stored in its raw format until it's processed and analyzed.
- **Data Warehouses**: Specialized for **analytical queries** and **business intelligence**, typically storing **cleaned and structured data** from multiple sources, optimized for reporting and decision-making.

Each of these solutions serves a distinct purpose in the data ecosystem, with **traditional databases** focusing on operational efficiency, **data lakes** focusing on storing diverse and unprocessed data for advanced analysis, and **data warehouses** focusing on delivering insights from structured data for business intelligence.
