A **data warehouse** (DW) is a specialized repository designed for storing large volumes of **structured** data from multiple sources, optimized for **analytical processing** ([[OLAP]]) rather than transactional processing ([[OLTP]]).

## Key Characteristics

- **Data Structure**: Primarily stores **structured data**. The data is organized into tables, often with a schema that is designed for fast querying and analysis.
- **Storage Format**: Data is typically transformed (via **ETL** — Extract, Transform, Load) into a clean, organized format before being loaded into the warehouse.
- **Data Processing**: Optimized for **analytical queries** (OLAP), often aggregating and summarizing large datasets. Unlike traditional databases, which are used for transactional data (OLTP), data warehouses support reporting, business intelligence, and data analytics.
- **Querying**: Primarily uses **SQL** (Structured Query Language) for querying. It’s optimized for complex, long-running queries that aggregate data over time (e.g., monthly sales reports).
- **Performance**: Designed to handle large volumes of read queries rather than frequent updates or transactions. Data is often indexed for fast querying.
- **ACID Compliance**: Typically, data warehouses don’t emphasize **transactional integrity** but focus more on **data consistency** and availability for analytical purposes.

## **Use Cases**

- **Business Intelligence (BI)**, **reporting**, **data analysis**, and **decision-making**.
- Storing **historical data** for long-term analysis (e.g., sales performance, customer behavior over time).

## **Warehouse solutions**

- **[[Amazon Redshift]]**, **[[Google BigQuery]]**, **[[Snowflake]]**, **[[Microsoft Azure Synapse Analytics]]**, **[[Teradata]]**.