We can group [[Pandas DataFrame|DataFrames]] similarly to [[SQL]]:
```
SELECT  Sum(quantity) from expenses GROUP BY employee 
```

is the same as 

```
dataFrame.groupby('employee').expenses.sum() 
```

The result of a grouping is not a DataFrame, but a DataFrameGroupBy object, with the group column as index. If we group by several columns, the result will be a multi index DataFrameGroupBy.

To obtain a DataFrame, not a DataFrameGroupBy, we need to execute aggregated functions, with the **agg** method

## Aggregated functions 

### Syntax 

```
dataFrameGroupBy.agg(func)
```

The **func** argument accepts different types:

* function
* str: a string function name
* list: list of functions and/or function names
* dict:  a dictionary with the syntax {columns:function}
* None
