Decide what kind of [[data storage]] we want has a deep impact on [[database performance]]. Data is written in continuous chunks. In row oriented databases, each chunk contains a row containing all of its columns values as a tuple. In the other hand, in column oriented databases each chunk contains all values in each row belonging to a certain column. 

## Row stores


![[Pasted image 20250120183232.png|500]]
+ Typically [[Online Transaction Processing|OLTP]]
+ Partitioned horizontally
+ Stores all row's values together, as a tuple
+ Write data quickly 
+ Indexing can drastically improve query time
## Column stores

![[Pasted image 20250120183356.png|500]]

+ Typically [[OLAP]]
+ Partitioned vertically 
+ Stores multiples row's column values together 
+ Reads are efficient
+ Columns have uniform types
+ Column compression works well, speeding up reads.