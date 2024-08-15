
# Applied Statistical Analysis - (STAT08024) - 2024 - Summer  Paper

## Question 1

### Question 1.A

A researcher wants to know if the Irish public are in support of a new government policy. He believes that less than 30% of the public support it and wishes to carry out a survey to test this hypothesis. From a list of individuals living in his area he draws a random sample of 80 individuals and finds that 23 are in favour.

#### Question 1.A.1 (1 Mark)

What is the population?

#### Answer 1.A.1

The population is the Irish public.

#### Question 1.A.2 (1 Mark)

Identify any potential bias.

#### Answer 1.A.2

The researcher has drawn a sample from a list of individuals living in his area. This may introduce bias as the sample may not be representative of the Irish public.  A better approach would be to use a random sample of the Irish public, i.e. a few people from each county (area).

#### Question 1.A.3 (2 Marks)

Identify the parameter and statistic - give the symbol and value for both.

#### Answer 1.A.3

- **Parameter (Population Proportion)**: The parameter is the true proportion of the Irish public who support the new government policy.
  - **Symbol**: $p$
  - **Value**: Unknown, but the researcher hypothesizes it to be $p_0 = 0.30$ (30%).

- **Statistic (Sample Proportion)**: The statistic is the proportion of the sampled individuals who support the new government policy.
  - **Symbol**: $\hat{p}$
  - **Value**: $\hat{p} = 0.2875$ (28.75%).

### Question 1.B (5 Marks)

The melting points (C) of n=50 alloy filaments is investigated yielding T= 320.1 and
s = 6.75. Calculate a 95% confidence interval for the mean melting point p.

#### Answer 1.B

<details>
<summary>Choosing a Distribution</summary>

To determine whether to use the **t-distribution** or the **z-distribution** for calculating the confidence interval, you need to consider two factors:

1. **Sample Size**:
   - For **large sample sizes** (typically $n \geq 30$), the **z-distribution** (normal distribution) is usually used to calculate the confidence interval, because the Central Limit Theorem ensures that the sample mean will be normally distributed.
   - For **small sample sizes** (typically $n < 30$), the **t-distribution** is used because the t-distribution accounts for the additional uncertainty that comes with estimating the population standard deviation $\sigma$ using the sample standard deviation $s$.

2. **Use of Sample Standard Deviation**:

   - When the population standard deviation $\sigma$ is **unknown** and the sample size is relatively small, the **t-distribution** is more appropriate because it adjusts for the additional variability that comes with estimating $\sigma$ using $s$.
   - Even for **larger samples** (like $n = 50$), if you are using the sample standard deviation $s$ instead of the population standard deviation $\sigma$, the **t-distribution** is still the more accurate approach.

Why use the t-distribution in this case?  

In your problem:

- The **sample size $n = 50$** is relatively large, but the population standard deviation $\sigma$ is **unknown** (you are given the sample standard deviation $s = 6.75$).
- Since you are using the **sample standard deviation $s$**, it is safer to use the **t-distribution** rather than the z-distribution.

Thus, you would calculate the confidence interval using the formula:

$$\bar{x} \pm t_{\alpha/2} \times \frac{s}{\sqrt{n}}$$

because the sample size, though not extremely small, still warrants the use of the **t-distribution** due to the reliance on the sample standard deviation.

</details>

- Sample size $n = 50$
- Mean $\bar{x} = 320.1$
- Standard deviation $s = 6.75$
- Confidence level $1 - \alpha = 0.95$

The confidence interval for the mean melting point $\mu$ is given by:

$$
\bar{x} \pm t_{\alpha/2} \times \frac{s}{\sqrt{n}}
$$

Where $t_{\alpha/2}$ is the critical value for the t-distribution with $n-1$ degrees of freedom and $\alpha/2$ significance level.

### Question 1.C (5 Marks)

A cereal manufacturer packages cereal in boxes with a 500g label weight. Suppose that the
actual distribution of weights is $N(\mu = 500, \sigma^2 = 2.1)$.

#### Question 1.C.1 (3 Marks)

What percentage of the boxes have cereal weighing over 500g?

#### Question 1.C.2 (3 Marks)

If n = 5 boxes are selected at random compute $Pr(\overline{X} \leq 499.5)$.

### Question 1.D (5 Marks)

$A \sim t_{11}. \text {Given }\Gamma(5.5)=52.34$, calculate $f(a=1)$.

### Question 1.E (5 Marks)

Consider the following joint distribution:

| p(x,y) | 0 | 1 | 2 |
|--------|---|---|---|
| 0      | 0.1 | ? | 0.25|
| 1      | 0.15 | 0.15 | 0.25|


## Paper Details

STAT08024 - Applied Statistical Analysis
Summer Examinations 2023/2024

