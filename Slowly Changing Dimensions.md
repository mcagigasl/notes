In data engineering, **changing [[dimension|dimensions]]** primarily refers to how changes in **dimension attributes** (like customer data, product information, etc.) are handled in a data warehouse or database, ensuring that historical changes are either preserved, overwritten, or managed in a way that supports accurate reporting and analytics.

Dimensional changing only affects dimensional tables. The values of the metrics captured on [[Fact Table|fact tables]] should stay the same over time.

There are several strategies for change dimensions:

## Type I

Updates rows with the new value. This is suitable when historical data is not necessary.

### Pros
+ Easy implementation
+ Reduces storage requirements (no new columns or table needed)
### Cons
+ Historical changes are lost.

## Type II

Adds column(s) with timestamps to track changes, preserving both new and old values. This is suitable when we want to maintain historical changes across time.
### Pros

+ Preserves full historical changes
+ Ideal for trend analysis and reporting
### Cons
+ More storage needed than Type II 
+ Complex queries 
## Type III

The dimension table stores both, the new and old attributes (like previous_address and current_address). Useful when we want to kept a limited history.
### Pros
+ Simpler to implement than Type II
+ Less storage than Type II
### Cons

- Limited historical tracking—only the most recent change is available.
- Not suitable for complex historical analysis.
## Type IV 

Creates dimensional tables for historical data, like a snapshot. Useful when we want the full history keeping the dimension table light. 

### Pros

- Keeps the main dimension table small and optimized for querying.
- Allows for full historical tracking in a dedicated table.

### Cons

- More complex to query (you may need to join the current and historical tables).
- Requires additional storage for the historical table.
