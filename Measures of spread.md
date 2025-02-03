Measures of spread describes how [[data]] observations are apart or close together.  There are few different measures of spread.

## Variance

Variance is the distance from each data point to the data's [[Measures of center|mean]]. In probability theory, variance is the expected value of the squared deviation from the mean of a [[Random Variable]].

The higher the variance, more spread-out are the data.
![[Pasted image 20250128112736.png|500]]


## Standard deviation and absolute deviation
### Standard deviation (SD)

Square root of variance.
+ Same unit as data
+ Sensitive to outliers because of squaring:
+ Useful in normally distributed data
+ If data follows a normal distribution, ~68% of the values fall within 1 SD of the mean.
### Mean absolute deviation (MAD)

Mean absolute deviation takes the absolute value of the distances to the mean, and then takes the mean of those differences.
+ Same unit as data 
+ More robust to extreme values such as outliers 

#### Standard deviation vs Mean absolute deviation

![[Pasted image 20250128115048.png|500]]

If the data is normally distributed (or close to normal)
    
- SD is preferred because it effectively captures the spread.
- SD is directly related to variance, making it useful in many statistical models and inferential statistics.
- If data follows a normal distribution, ~68% of the values fall within 1 SD of the mean.
    
 If the data has [[outliers]] or is skewed
    
- MAD is preferred because it is more robust to extreme values.
- MAD is based on the median, which is less affected by large deviations than the mean.
- Even a single large outlier can significantly inflate SD, while MAD remains stable.
## Interquartile range 
The interquartile range is the distance between the 0.25 and the 0.75 ($Q_3 - Q_1$
) [[Quantiles|percentile]], which is also the height of the box in a boxplot.
