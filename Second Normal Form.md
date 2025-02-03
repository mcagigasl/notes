---
aliases:
  - 2NF
---

The 2NF is intended to avoid columns to don't contain relations or composite values. To accomplish it the following must to be true:
* Must satisfy [[First Normal Form|1NF]]
* If [[Primary Key]] is one column, 2FN is satisfied
* f there is a composite primary key, then each non-key column must be dependent on **all** the keys