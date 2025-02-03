The continuous uniform [[Probability Distribution]] is a probability distribution that describes an experiment where the outcome is equally likely to occur anywhere within a given interval $[a,b]$. That is, any subinterval of equal length within $[a,b]$ has the same probability of containing the outcome. The [[Probability Density Function]] (PDF) is constant over this interval and zero outside it.

## Probability density function

![[Pasted image 20250129124331.png|500]]
$$ f(x) = \begin{cases} \frac{1}{b - a}, & a \leq x \leq b \\ 0, & \text{otherwise} \end{cases}$$
## [[Cumulative distribution function]]
![[Pasted image 20250129124404.png|]]
$$F(x) = \begin{cases} 0, & x < a \\ \frac{x - a}{b - a}, & a \leq x \leq b \\ 1, & x > b \end{cases}$$