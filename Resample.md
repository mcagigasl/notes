Resample is a method to convert [[Pandas Series]] or [[Pandas DataFrame|DataFrames]] datetime-like [[Explicit Indexing|index]]. The object must to have a datetime index, and this index will be modified according to an [[Date Offset]] rule. 

It works like a [[Grouping DataFrames|groupby]] method, because the resultant object will be grouped by the offset. Therefore, an aggregated function must be used. 

