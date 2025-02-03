ELT stands for **Extract, Load, Transform**. In ELT, the data is stored in its native form in a storage solution like [[Data Lake]] or a [[Data Warehouse|data warehouse]]. Portions of data are transformed for different purposes, from building a data warehouse to doing deep learning. All the transformation happens on the data warehouse (or the storage solution).

ELT processes have grown due, in part to the growth of cloud data warehouses.

 
![[Pasted image 20241203185311.png]]
#### Pros
+ No separate system to process data 
+ Transformations can be rerun without impacting source systems
+ Works well for near real-time requirements

#### Cons 
+ Increase storage [[costs]] due to raw data
+ Compliance with [[Personal Indentifiable Information|PII]] is complicated


