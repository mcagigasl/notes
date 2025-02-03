A fact table is the central table in a [[dimensional model]] that contains quantitative data (often called measures) that can be analysed. Fact tables typically store numerical values that represent business metrics (e.g., sales, revenue, quantity)

Example: A "Sales" fact table might include fields like SalesAmount, QuantitySold, and DiscountApplied, along with foreign keys linking to dimensions like time, products, and customers.

## Characteristics

- Stores measurable, numeric data (e.g., sales, revenue, profit).
- Contains [[Foreign Key]] that reference related [[Dimension Table]].
- Can have large volumes of data, as it typically records every transactional event.