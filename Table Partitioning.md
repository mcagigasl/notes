[[Table]] Partitioning is the technique to split a table into a several part. This technique is meant to reduce the space of a single table in memory and optimize querys.


## Vertical Partitioning

Vertical partitioning splits up a column(s) of a table into a several ones. This could be useful to split data which is not fetched habitually, such as a long description.
## Horizontal Partitioning 

Horizontal partitioning splits up a table horizontally, for example from a certain timestamp. 

### Syntax

```
CREATE TABLE film_partitioned (

film_id INT,

title TEXT NOT NULL,

release_year TEXT

)

PARTITION BY LIST (release_year);

-- Create the partitions for 2019, 2018, and 2017

CREATE TABLE film_2019

PARTITION OF film_partitioned FOR VALUES IN ('2019')
```

### Pros
* Indices of heavily-used partition fits in memory
* Move to specific medium: slower vs faster
* Used for both [[Online Analytical Processing|OLAP]] and [[Online Transaction Processing|OLTP]]

### Cons
* Partitioning a table can be complicated
* Some constraints can not be set