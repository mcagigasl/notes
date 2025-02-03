A time series is a series of data points **indexed** in time order. It is plotted frequently using a [[Run Chart]]

With [[Pandas]] if we have a dataset including discrete data and date columns, it would be useful to convert the columns into indexes via [[Explicit Indexing]]. [[Date Offset|Date offsets]] could be very useful to create index and manipulate them. 

The method `dataFrame.index.to_period()` is very useful to group a time indexed dataframe.

