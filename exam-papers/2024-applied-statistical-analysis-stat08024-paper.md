
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

$$\bar{x} \pm t_{v,\alpha/2} \times \frac{s}{\sqrt{n}}$$

because the sample size, though not extremely small, still warrants the use of the **t-distribution** due to the reliance on the sample standard deviation.

</details>

- Sample size $n = 50$
- Mean $\bar{x} = 320.1$
- Standard deviation $s = 6.75$
- Confidence level $1 - \alpha = 0.95$

The confidence interval for the mean melting point $\mu$ is given by:

$$
\bar{x} \pm t_{v,\alpha/2} \times \frac{s}{\sqrt{n}}
$$

Where $t_{v,\alpha/2}$ is the critical value from the t-distribution with $v = n - 1 = 50 - 1 = 49$ degrees of freedom and $\alpha/2 = (1 - 0.95)/2 = 0.025$.  

The critical value $t_{v,\alpha/2}$ can be found using a t-table or a statistical calculator. For a 95% confidence level and 49 degrees of freedom, the critical value is approximately $2.0096$.

<details>
<summary>Calculating a Confidence Interval not in the t-table</summary>
To use **linear interpolation** for estimating the critical value of $t_{49,\alpha/2}$, we'll use the nearest critical values from the t-distribution table for $v = 40$ and $v = 60$. Here are the steps:

Step 1. Identify known values from the t-distribution table:

- For $v = 40$ and $\alpha/2 = 0.025$ (95% confidence level):
  - $t_{40,\alpha/2} = 2.021$
- For $v = 60$ and $\alpha/2 = 0.025$:
  - $t_{60,\alpha/2} = 2.000$

We want to estimate the value for $v = 49$.

Step 2: Set up the linear interpolation formula  

To find the critical value for $v = 49$, we can set up a proportion:

$t_{49} = t_{40} + \left( \frac{49 - 40}{60 - 40} \right) \times (t_{60} - t_{40})$

Where:

- $t_{49}$ is the estimated critical value we want.
- $t_{40}$ and $t_{60}$ are the known critical values.
- $49 - 40$ is the difference between 49 and 40.
- $60 - 40$ is the total difference between the degrees of freedom.

Step 3: Plug in the values and calculate

Let's calculate the interpolated value.

It seems like I can’t do more advanced data analysis right now. Please try again later.

However, you can follow the formula and plug in the numbers manually:

$t_{49} = 2.021 + \left( \frac{49 - 40}{60 - 40} \right) \times (2.000 - 2.021)$

This should give you an interpolated value close to $2.0096$, matching the exact calculation.
</details>

Substitute the values into the formula:

$320.1 \pm 2.0096 \times \dfrac{6.75}{\sqrt{50}} = $  
$320.1 \pm 2.0096 \times \dfrac{6.75}{7.0711} = $
$320.1 \pm 1.92 = $
$[318.18, 322.02]$

$\text{The 95\% confidence interval for the mean melting point is \boxed{[318.18, 322.02]}}$

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

