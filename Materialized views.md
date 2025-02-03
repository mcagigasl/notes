Materialized views stores the content of a view query in disk. There are useful for querys taking long time for execute. 

To create a materialized view:
`CREATE MATERIALIZED my_view VIEW as...`

To refresh a materialized view:
`REFRESH MATERIALIZED VIEW my_view`

## Dependencies 

Sometimes materialized views depends on other materialized views, and refreshing views becomes non-trivial. There are several tools to managing dependencies such as:
* [[Directed Acyclic Graphs]]
* [[Pipeline scheduler tools]] such as [[Apache Airflow]] or [[Luigi]]*