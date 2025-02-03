The Kinball model, is a [[Data WareHouse Architecture|data warehouse architecture]]  approach in which [[Data Mart|data marts]] are first formed based on business requirements. This approach refers a data warehouse as **a copy o transaction data specifical architecture for query and analysis***. Follows the [[Star Schema]] so the data follows a [[Denormalized Schema | denormalized schema]]

![[Pasted image 20250116130928.png]]

## Advantages
* Quickly completing the first stage of data warehousing design process
* Because the denormalized structure, the majority of data operators can quickly understand it.
* Simply creation of new data marts
## Disadvantages

* It is difficult to modify the [[dimensional model]] to accommodate any change in business requirements.
* Redundant data, so irregularities can occur.
* Incorporating large amounts of legacy data is complex.
* ETL processing time because denormalization


## Kimball's 4-step model

Kimball's 4-step model is aimed to create [[Data Mart|Data Marts]] following the [[dimensional model]], following the steps bellow: 

* **Step 1**:  Select the [[organizacional process]]
* **Step 2**: Declare the grain 
* **Step 3**: Identify the dimensions
* **Step 4**: Identify the facts 
