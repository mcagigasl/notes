---
aliases:
  - DataFrames
tags:
  - Pandas
---
A [[Pandas]] DataFrame is a Pandas Data Structure representing a bi-dimensional array with columns and rows. It can be thought as a [[SQL Table]]. Each column is a [[Pandas Series]]. 

Each DataFrame could be manipulated as a SQL Table, for example

`SELECT  Sum(quantity) from expenses GROUP BY employee 

is the same as 

`dataFrame.groupby('employee').expenses.sum() 

DataFrame records are nameds *observations* and indexes *labels*

### Methods 

Returns the fist n rows``dataFrame.head(n)
Column information``dataFrame.info()
Rows and columns ``dataFrame.shape
Fet stadistics``dataFrame.describe()
Subs dataFrames `dataFrame[[]]

### Methods for Categorical Data

``dataFrame.drop_duplicates([])
``dataFrame.value_counts(normalize=False)
## Missing Values

A missing value, in a DataFrame is treated as a NaN. There are several ways to manage missing values:

*  A boolean dataFrame
```
dataFrame.isna()
```

* In combination with `dataFrame.any()` we can obtain a serie, indexed by columns with the columns containing missing values
```
dataFrame.isna().any()
```

* It's possible to drop observations with missing values or even replace missing values:
```
dataFrame.dropna()
dataFrame.fillna(value)
```