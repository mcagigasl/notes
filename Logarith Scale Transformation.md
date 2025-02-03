Logarithmic transformations are useful when [[data]] spans several orders of magnitude or has [[skewed distributions]]

## Use Cases
### Dealing with Skewed Data (Normalization)

- If your data has a long right tail (e.g., salaries, population sizes, stock prices), taking the logarithm makes it more normally distributed.
- This improves statistical analysis, making models like linear regression work better.
- Example: Income distribution—most people earn low to moderate wages, but a few earn extremely high salaries.

###  Enhancing Visualization of Large Ranges

- When data covers many orders of magnitude, a log scale compresses large values and expands small ones.
- This makes patterns easier to see.
- Example: Earthquake magnitudes (Richter scale) or astronomical distances.

###  Reducing Variance in Machine Learning Models

- Some ML algorithms (e.g., linear regression, neural networks) perform poorly when numerical values vary drastically.
- Log transformations help stabilize variance (homoscedasticity) and improve model performance.
- Example: Predicting house prices—a small house price might be $100K, while a luxury mansion might be $10M.

### Multiplicative Relationships to Additive Ones

- Many natural phenomena follow power-law or exponential relationships (e.g., bacterial growth, economic trends).
- A log transformation turns multiplication into addition, making it easier to model.
- Example: Exponential growth in pandemics—instead of analyzing cases as 100, 1,000, 10,000, a log scale shows a linear trend.

### Feature Engineering for Machine Learning

- Log transformations can make features more informative for ML models.
- Useful when a feature's absolute differences matter less than its relative changes.
- Example: Financial data—log returns are often used instead of raw price changes.