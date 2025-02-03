Snowflake is a cloud-based [[Data Warehouse|data warehouse]] that utilizes a [[Columnar Databases|columnar]] data storage model. Uses [[Snowflake SQL]] to perform queries. 

## Architecture

Snowflake's architecture is a hybrid of [[Shared-disk Architecture]] and [[Shared-nothing Architecture]] architecture:

+ Uses a central data repository por persisted data
+ Processes queries using [[Massiively Parallel Processing|MPP]] compute clusters, where each node in the cluster stores a portion of the entire data.

### Layers
Snowflake architecture consists on three layers


![[Pasted image 20250121175815.png]]

#### Database Storage

When data is loaded into Snowflake, Snowflake reorganizes that data into its internal optimized, compressed, columnar format. Snowflake stores this optimized data in cloud storage. The data objects stored by Snowflake are not directly visible nor accessible by customers; they are only accessible through SQL query operations run using Snowflake.
#### Query Processing 

Query execution is performed in the processing layer. Snowflake processes queries using “virtual warehouses”. Each virtual warehouse is an MPP compute cluster composed of multiple compute nodes allocated by Snowflake from a cloud provider.
#### Cloud Services 

Services managed in this layer include:

+ Authentication
+ Infrastructure management
+ Metadata management
+ Query parsing and optimization
+ Access control

