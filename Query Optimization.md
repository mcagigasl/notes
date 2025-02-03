Despite modern database frameworks having ways to optimize query performance, it is still necessary to optimize query clauses.

Some query optimization techniques:

- Use `UNION ALL` instead of `UNION` if there are no duplicated records.
- Use the appropriate type of join for each query, avoiding unnecessary records.
- Don't use `SELECT *`; instead, select the columns you need.
- Always, when possible, filter your data early.