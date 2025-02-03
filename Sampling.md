In a [[data]] context, sampling refers to a technique to randomly subset a dataset. Sampling is useful for reducing computational costs, improving efficiency, and enabling [[statistical inference]] when dealing with large datasets or even study a case sampling some values instead of analysing the whole dataset.

### Common sampling techniques

- **Random Sampling** – Each data point has an equal chance of being selected.
- **Stratified Sampling** – The dataset is divided into distinct groups (strata), and samples are taken proportionally from each.
- **Systematic Sampling** – Every _n_-th data point is selected from an ordered dataset.
- **Cluster Sampling** – The dataset is divided into clusters, and entire clusters are randomly selected.
- **Reservoir Sampling** – Used for streaming data, where a fixed-size sample is maintained dynamically.

### [[Pandas DataFrame|DataFrames]] sampling

We an sample a DataFrame with the `sample` method
```
dataFrme.sample(n, replace=False)
```

Replace, allows or disallows sampling of the same row more than once.