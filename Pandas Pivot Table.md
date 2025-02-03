A [[Pandas]] [[Pivot Table]] is the way pandas has to create Pivot Tables from a [[Pandas DataFrame]]. A Pivot Table is a [[Pandas DataFrame|DataFrame]] with [[Explicit Indexing]]

The rows are indexed by the index attribute, values are the values to aggregate, columns are the keys to group by and the aggfunction is the aggregated function to apply. By default the aggfunction is mean()

```
	pandas.pivotTable(index, values, columns, aggfunction)
```

I