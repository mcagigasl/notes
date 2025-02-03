---
aliases:
  - Percentiles
---

Quantiles are cut points dividing the range of a probability [[Probability Distribution]] into continuous intervals with equal probabilities, or dividing the observatinos of [[Data|data]] in the same way.

With [[NumPy]] we can calculate quantiles from a serie, with the `np.quantile methd`

The 0.5 quantile is the median
```
np.quantile(serie,0.5)
```

We also can calculate [[quartiles]]
```
np.quantile(serie,np.linspace(0, 1, 5))
```
