[[Pandas DataFrame|DataFrames]] and [[Pandas Series|Series]] are able to call  [[Matplotlib]] [[plotting]] methods, which simplifies notation. For example, matplotlib.pyplot.hist() can be called by dataFrame.hist()

To create the plot:
```
series.plot(kind)
dataFrame.plot(kind)
series.hist()
```

To visualize the plot
```
matplotlib.show()
```
## Bars

Reveals relationship between categorical and numerical variables. Usually used with series with [[Explicit Indexing]]
```
series.plot(kind='bars')
```

## [[Line Plots]]

```
dataFrame.plot(x=x_column, y=y_column, kind='line')
```
## [[Scatter Plots ]]


```
dataFrame.plot(x=,y=,kind='scatter)
```
## [[Histogram]]

```
	series.hist(alpha, bins)
	dataFrame.hist(columnn, alpha, bins)
```

## [[Boxplot]]
