A **dimension table** contains descriptive, textual, or categorical information that provides context to the facts stored in the fact table. Each dimension table is typically linked to the [[Fact Table]] by a [[foreign key]].

 **Example**: A "Time" dimension table might include attributes like `Day`, `Month`, `Quarter`, `Year`, and `Weekday`. A "Product" dimension table might include `ProductName`, `Category`, `Brand`, and `Supplier`.
 
## Characteristics:

- Contains **descriptive attributes** (e.g., product names, customer locations, time periods).
- **[[Surrogate keys]]** are often used to uniquely identify dimension records (e.g., `ProductID`, `TimeID`).
- Smaller in size compared to [[Fact Table]], and data is often more static.
- **Denormalized structure** (for better query performance) compared to normalized transactional models.