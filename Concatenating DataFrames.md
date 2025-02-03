[[Pandas DataFrame|DataFrames]] cane be concatenated horizontally and vertically:

![[Pasted image 20250117102812.png|500]]

## Syntax

```
pd.concat([d1,...,dn], axis=0)
```

The axis parameter controls if the concatenation is by row(0) or by column(1)
### Index Dropping

Because concatenated DataFrames can have same index, we can drop he original indexes by:

```
pd.concat([d1,...,dn], ignore_index = true)
```

### Multi Index
It is possible to have [[Explicit Indexing]] in the resultant table associating the original tables with keys, for that we need to ignore original indexes too:

```
pd.concat([d1,...,dn], ignore_index = true, keys=['key1',...,'keyn'])
```

### Multiple Columns 

If we concatenate tables with different column names, NaN values will be assigned to not matched columns. To ignore not comun columns we can perform an [[Inner Join]]

```
pd.concat([d1,...,dn],join='inner')
```