ETL stands for **Extract, Transform, Load**. In In ETL, data is transformed before loading into storage - usually to follow the storage's schema, as is the case with [[Data Warehouse]]

In an ETL process, the data is transformed during the move and it uses a separate systems to process the data.

![[Pasted image 20241203184932.png]]

#### Pros
+ Lower storage [[costs]]
+ Easiest [[Personal Indentifiable Information|PII]] compliance: the original data is transformed in transit, so we can use this to anonymize PII and avoid the PII to be loaded into the data warehouse.
#### Cons
+ Transformation errors requires new data pulls
+ Costs of separate system to process data

### Purposes
+ Clean Data
+ Maximize querys after ETL process