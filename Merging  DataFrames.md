[[Pandas DataFrame|Dataframes]] can be joined like [[SQL]] joins. 

## By Column

```
DataFrame.merge(right, on=column, how='inner')
```

The `on` argument only works if both DataFrames has the same column name. For merging different columns names:

```
DataFrame.merge(right, right_on, left_on , how='inner')
```

### [[Inner Join]]

```
DataFrame.merge(right, on, how='inner')
```

### [[Left Join]] and Right Join

```
DataFrame.merge(right|left, on, how='left')
```

### Outer Join

```
DataFrame.merge(right, on, how='outer')
```

### [[Self Join]]

```
DataFrame.merge(DataFrame, right_on, left_on ,)
```

### [[Semi Join]]

For semi joins, first we need to merge both DataFrames, and then exclude from the filter the left dataframe by the values contained in the merged one.

```
mergedDataFrame = leftDataFrame.merge(rightDataFrame, on=key)
semiJoinDataFrame = leftDataFrame[leftDataFrame['key'].isin(mergedDataFrame['key'])
```

### [[Anti Join]]

For anti joins, the strategy is similar as semi joins, but with two differentes: a left join strategy, and we need to keep trak of what columns of the merged DataFrame belongs to the left, to the right or to both. We use the *indicator* argument for this purpose.
```
mergedDataFrame = leftDataFrame.merge(rightDataFrame, on=key, how='left', indicator=True)
keyList = mergedDataFrame[mergedDataFrame['_merged'] == 'left_only]
antiJoinDataFrame = leftDataFrame[leftDataFrame[key].isin(keyList)]

```
## By Index

### Single Index 

The merge method adjust to accept index names or column names, so the syntax is the same as joining data by column:

```
DataFrame.merge(right, on=index, how='inner')
```

### MultiIndex
```
DataFrame.merge(right, on=[index_1,...,index_n], how='inner')
```

## By Index and Column 

For merging two tables (or one table with itself) by index and column, `right_index` or `left_index` are needed to define if the resultant DataFrame must contain the original indexes or not.

## Ordered merges 

If we want to preserve dataframes order, we need to use the `pd.merge_ordered` method. This method orders the resultant dataframe according to the `on` column(s), even if the original dataframes are not sorted. 

```
pd.merge_ordered(df1, df2, on='key', how, fill_method)
```

In addition, allows for handling missing values with the `fill_method` argument.

### Asof method
```
pd.merge_asoft(df1, df2, on='key')
```
+ Left method 
+ Stands for "as of "
+ Searches the nearest value in the "on" clause 