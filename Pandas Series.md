A [[Pandas]] Series is an extension of [[NumPy Arrays]] (is built on top of it) with some extra features, like indexing, handling of missing values (NaN).  [[Pandas DataFrame]] columns are, indeed Pandas Series. A easy way to access it is: `dataFrame.colum_name 

## Aggregation
`Series.aggregate([f1,...,fn])`allows to execute several methods against a series.

## String
`Series.str` allows to access String methods

## Plot

Series can be plotted along with [[Matplotlib]] package with the method .plot
`Series.plot`
