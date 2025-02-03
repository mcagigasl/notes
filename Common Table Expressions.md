---
aliases:
  - CTEs
---
Common Table Expressions (CTEs) are [[SQL]] constructs used to define auxiliary queries within a larger query. They are intended to simplify complex queries and improve readability. Depending on the SQL engine, CTEs may be executed either inline or materialized, which can, in some cases, aid in query optimization.

```postgresql
WITH cte_name AS ()
```
