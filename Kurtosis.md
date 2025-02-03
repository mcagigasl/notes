**Kurtosis** measures the **tailedness** of a [[Probability Distribution]], which is related to the presence of [[outliers]] but does not directly count them.

$$K = \frac{\frac{1}{n} \sum_{i=1}^{n} (X_i - \mu)^4}{\left(\frac{1}{n} \sum_{i=1}^{n} (X_i - \mu)^2 \right)^2}$$ Where 
- $Xi$​ = Each individual data point
- $\mu$ = Population mean
- $n$ = Total number of observations
- The numerator measures **[[fourth central moment]]** (how extreme the tails are).
- The denominator normalizes by **[variance squared]** to standardize kurtosis.


- **High kurtosis (>3, "leptokurtic")**: More extreme outliers, meaning the distribution has heavy tails.
- **Low kurtosis (<3, "platykurtic")**: Fewer extreme outliers, meaning the distribution has lighter tails.
- **Normal kurtosis (≈3, "mesokurtic")**: Similar to a normal distribution, with a typical number of outliers.

![[Pasted image 20250131104825.png]]