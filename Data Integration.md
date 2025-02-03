---
tags:
  - jobcv
---

[[Data]] Integration is the proces to integrate different data sources into a Unified Data Model.  This Unified model should be [[Business Driven]] e.g what combination of data will be useful for the business.

![[Pasted image 20250114102941.png]]


## Data Integration Tool 

The Data Integration Tool must be **flexible, reliable and scalable**. ///An example of integrations tools: [[Snowflake]] (an agnostic [[Data Warehouse]]), [[Google BigQuery]] or [[Amazon Redshift]]
## Sources 

Sources can be, differents [[Database Management Systems]] and the **cadence** of updating depends on the type of the source data.

## Transform

Because the unified data have a unique [[Database Management Systems]] , an [[ETL]] is necessary to update the unified data model with the source data.

Automated Testing is important to maintain data consistency.

## Governance

For [[Data Governance]] purposes, stablish the lineage of the data is important which means that the data stored in the unified data model must be backtracked to its original data source. 
