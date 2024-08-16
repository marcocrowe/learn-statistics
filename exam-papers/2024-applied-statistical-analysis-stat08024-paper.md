
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

#### Answer 1.C

#### Question 1.C.1 (3 Marks)

What percentage of the boxes have cereal weighing over 500g?

#### Answer 1.C.1

#### Question 1.C.2 (3 Marks)

If n = 5 boxes are selected at random compute $Pr(\overline{X} \leq 499.5)$.

#### Answer 1.C.2

To solve the questions, we'll use the properties of the normal distribution.

1. **Determine the probability:**

   Since the distribution of weights is $N(500, 2.1)$, we want to find $P(X > 500)$.

   We can standardize this to the standard normal distribution:
   \[
   Z = \frac{X - \mu}{\sigma}
   \]
   where $X$ is the weight of a box, \(\mu = 500\), and \(\sigma = \sqrt{2.1}\).

   For $X = 500$:
   \[
   Z = \frac{500 - 500}{\sqrt{2.1}} = \frac{0}{\sqrt{2.1}} = 0
   \]

   The standard normal variable $Z$ for $X = 500$ is 0. 

   The probability that $X$ is greater than 500 grams is:
   \[
   P(X > 500) = P(Z > 0)
   \]

2. **Use the standard normal distribution:**

   In the standard normal distribution, $P(Z > 0)$ is 0.5, because the normal distribution is symmetric around 0.

   Therefore:
   \[
   P(X > 500) = 0.5
   \]

3. **Convert to percentage:**

   \[
   \text{Percentage} = 0.5 \times 100\% = 50\%
   \]

   **Answer 1.C.1:** 50% of the boxes have cereal weighing over 500g.

### Question 1.C.2

**If $n = 5$ boxes are selected at random, compute $Pr(\overline{X} \leq 499.5)$.**

1. **Determine the distribution of the sample mean:**

   The sample mean \(\overline{X}\) for \(n\) boxes follows a normal distribution:
   \[
   \overline{X} \sim N\left(\mu, \frac{\sigma^2}{n}\right)
   \]

   Given \(\mu = 500\), \(\sigma^2 = 2.1\), and \(n = 5\):
   \[
   \overline{X} \sim N\left(500, \frac{2.1}{5}\right)
   \]

   The variance of \(\overline{X}\) is \(\frac{2.1}{5}\) and the standard deviation is \(\sqrt{\frac{2.1}{5}}\).

   \[
   \sigma_{\overline{X}} = \sqrt{\frac{2.1}{5}} \approx \sqrt{0.42} \approx 0.648
   \]

2. **Standardize the sample mean:**

   We need to find:
   \[
   P(\overline{X} \leq 499.5)
   \]

   Standardize this to the standard normal distribution:
   \[
   Z = \frac{\overline{X} - \mu}{\sigma_{\overline{X}}}
   \]

   For \(\overline{X} = 499.5\):
   \[
   Z = \frac{499.5 - 500}{0.648} \approx \frac{-0.5}{0.648} \approx -0.771
   \]

3. **Use the standard normal distribution:**

   Find the probability $P(Z \leq -0.771)$ using the standard normal distribution table or a calculator:

   \[
   P(Z \leq -0.771) \approx 0.220
   \]

   **Answer 1.C.2:** $Pr(\overline{X} \leq 499.5) \approx 0.220$ or 22.0%.

### Question 1.D (5 Marks)

$A \sim t_{11}. \text {Given }\Gamma(5.5)=52.34$, calculate $f(a=1)$.

### Answer 1.D

Sure, let's format the calculations correctly and ensure the steps are clear for the PDF calculation of the t-distribution at \(a = 1\) with 11 degrees of freedom.

### Calculation of the PDF for \(A \sim t_{11}\) at \(a = 1\)

The probability density function (PDF) of the t-distribution with \(\nu\) degrees of freedom is given by:

\[
f(a) = \frac{\Gamma\left(\frac{\nu + 1}{2}\right)}{\sqrt{\nu \pi} \Gamma\left(\frac{\nu}{2}\right)} \left(1 + \frac{a^2}{\nu}\right)^{-\frac{\nu + 1}{2}}
\]

Given:
- Degrees of freedom \(\nu = 11\)
- We need to calculate \(f(a = 1)\)

### Step 1: Substitute into the formula

The PDF at \(a = 1\) is:

\[
f(1) = \frac{\Gamma\left(\frac{11 + 1}{2}\right)}{\sqrt{11 \pi} \Gamma\left(\frac{11}{2}\right)} \left(1 + \frac{1^2}{11}\right)^{-\frac{11 + 1}{2}}
\]

Simplify to:

\[
f(1) = \frac{\Gamma(6)}{\sqrt{11 \pi} \Gamma(5.5)} \left(\frac{12}{11}\right)^{-6}
\]

### Step 2: Use the provided values

We are given:
- \(\Gamma(5.5) = 52.34\)
- $\Gamma(x) = (x-1)!$ for integer x
- \(\Gamma(6) = 5! = 120\)

### Step 3: Compute the value

1. **Calculate \(\sqrt{11 \pi}\)**

   \[
   \sqrt{11 \pi} = \sqrt{11 \times 3.1416} \approx \sqrt{34.5576} \approx 5.879
   \]

2. **Calculate \(\left(\frac{12}{11}\right)^{-6}\)**

   \[
   \frac{12}{11} \approx 1.0909
   \]
   \[
   \left(\frac{12}{11}\right)^{-6} \approx \left(1.0909\right)^{-6} \approx 0.665
   \]

3. **Substitute into the PDF formula**

   \[
   f(1) = \frac{120}{5.879 \times 52.34} \times 0.665
   \]

   Calculate the denominator:

   \[
   5.879 \times 52.34 \approx 307.47
   \]

   Then:

   \[
   \frac{120}{307.47} \approx 0.389
   \]
   \[
   f(1) = 0.389 \times 0.665 \approx 0.259
   \]

$$\boxed{f(1) \approx 0.259}$$

### Question 1.E (5 Marks)

Consider the following joint distribution:

| p(x,y) | x=0  | x=1  | x=2  |
|--------|------|------|------|
| y=1    | 0.1  | `?`  | 0.25 |
| y=2    | 0.05 | 0.15 | 0.25 |

Complete the table and calculate $p(x=1), p(y=1)$

### Answer 1.E

To complete the joint distribution table and calculate the marginal probabilities \( p(x=1) \) and \( p(y=1) \), follow these steps:

1. **Complete the Joint Distribution Table**

   Given the joint distribution:

   | p(x,y) | 0    | 1    | 2    |
   |--------|------|------|------|
   | 0      | 0.1  | ?    | 0.25 |
   | 1      | 0.05 | 0.15 | 0.25 |

   The sum of all joint probabilities should be 1:

   \[
   \text{Sum} = 0.1 + ? + 0.25 + 0.05 + 0.15 + 0.25
   \]

   First, calculate the sum of known values:

   \[
   0.1 + 0.25 + 0.05 + 0.15 + 0.25 = 0.8
   \]

   So, the sum of the unknown value \( ? \) should be:

   \[
   1 - 0.8 = 0.2
   \]

   Since the joint distribution table should sum to 1, and we have:

   \[
   0.1 + ? + 0.25 + 0.05 + 0.15 + 0.25 = 1
   \]

   The value of \( ? \) is:

   \[
   ? = 0.2
   \]

   | p(x,y) | x=0  | x=1  | x=2  |          |
   |--------|------|------|------|----------|
   | y=1    | 0.1  | `x`  | 0.25 | `y`      |
   | y=2    | 0.05 | 0.15 | 0.25 | 0.45     |
   |        | 0.15 | `z`  | 0.5  | **1.00** |

$y+0.45=1 \therefore y=0.55$  
$0.15+z+0.5=1 \therefore z=0.35$

   | p(x,y) | x=0  | x=1      | x=2  |          |
   |--------|------|----------|------|----------|
   | y=1    | 0.1  | `x`      | 0.25 | **0.55** |
   | y=2    | 0.05 | 0.15     | 0.25 | 0.45     |
   |        | 0.15 | **0.35** | 0.5  | **1.00** |

$x + 0.15 = 0.35 \therefore x = 0.2$  

Alternatively,  
$0.1+x+0.25 = 0.55 \therefore x = 0.2$  

   Thus, the completed table is:

   | p(x,y) | x=0  | x=1  | x=2  |      |
   |--------|------|------|------|------|
   | y=1    | 0.1  | 0.2  | 0.25 | 0.55 |
   | y=2    | 0.05 | 0.15 | 0.25 | 0.45 |
   |        | 0.15 | 0.35 | 0.5  | 1.00 |

1. **Calculate Marginal Probabilities**

   - **For \( p(x=1) \):**

     \[
     p(x=1) = p(x=1, y=0) + p(x=1, y=1) + p(x=1, y=2)
     \]

     Substituting the values:

     \[
     p(x=1) = 0.05 + 0.15 + 0.25 = 0.45
     \]

   - **For \( p(y=1) \):**

     \[
     p(y=1) = p(x=0, y=1) + p(x=1, y=1)
     \]

     Substituting the values:

     \[
     p(y=1) = 0.2 + 0.15 = 0.35
     \]

### Summary

- The completed joint distribution table is:

  | p(x,y) | 0    | 1    | 2    |
  |--------|------|------|------|
  | 0      | 0.1  | 0.2  | 0.25 |
  | 1      | 0.05 | 0.15 | 0.25 |

- The marginal probabilities are:

  - \( p(x=1) = 0.45 \)
  - \( p(y=1) = 0.35 \)

## Question 2

### Question 2.A (5 Marks)

Given $n_1 = 110, x_1 = 65$ and $n_2 = 120, x_2= 70$, calculate a 90% confidence interval for the difference in the two proportions. Using the confidence interval, comment on the population proportions.

#### Answer 2.A

To calculate a 90% confidence interval for the difference in two proportions, we follow these steps:

**Step 1: Define the Sample Proportions**  

Given:

- \( n_1 = 110 \) and \( x_1 = 65 \) for the first sample
- \( n_2 = 120 \) and \( x_2 = 70 \) for the second sample

The sample proportions are:

$\hat{p}_1 = \frac{x_1}{n_1} = \frac{65}{110} \approx 0.5909$  
$\hat{p}_2 = \frac{x_2}{n_2} = \frac{70}{120} \approx 0.5833$  
Confidence level:

$$(\hat{p}_1 - \hat{p}_2) \pm z_{\alpha/2} \times \sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}$$

$(\hat{p}_1 - \hat{p}_2) \approx 0.5909 - 0.5833 = 0.0076$  

The standard error (SE) for the difference between two proportions is:

$\text{SE} = \sqrt{\frac{\hat{p}_1 (1 - \hat{p}_1)}{n_1} + \frac{\hat{p}_2 (1 - \hat{p}_2)}{n_2}}$  

Plugging in the values:
$\text{SE} = \sqrt{\frac{0.5909 \times (1 - 0.5909)}{110} + \frac{0.5833 \times (1 - 0.5833)}{120}}$  
$\text{SE} = \sqrt{\frac{0.5909 \times 0.4091}{110} + \frac{0.5833 \times 0.4167}{120}}$  
$\text{SE} = \sqrt{\frac{0.2418}{110} + \frac{0.2421}{120}}$  
$\text{SE} = \sqrt{0.002198 + 0.002017}$  
$\text{SE} \approx \sqrt{0.004215} \approx 0.0649$  

**Step 4: Determine the Critical Value**

For a 90% confidence interval, the critical value ($z_{\alpha/2}$) is approximately 1.645. given from the standard normal distribution table.

**Step 5: Calculate the Confidence Interval
The confidence interval is given by:

$(\hat{p}_1 - \hat{p}_2) \pm z_{\alpha/2} \times \text{SE}$  
$0.0076 \pm 1.645 \times 0.0649$  
$0.0076 \pm 0.1061$  

So the 90% confidence interval is:
$0.0076 - 0.1061 \approx -0.0985$  
$0.0076 + 0.1061 \approx 0.1137$  

**Final Confidence Interval**  
$$\boxed{(-0.0985, 0.1137)}$$

The 90% confidence interval for the difference in the two proportions is from -0.0985 to 0.1137.

**Comment on the Population Proportions:**

- The interval includes 0, which suggests that there is no significant difference between the two population proportions at the 90% confidence level.
- This means we cannot conclusively state that one proportion is different from the other based on this interval. The proportions are not significantly different in a statistically significant way, considering the given confidence level.


### Question 2.B (5 Marks)

Calculate and interpret the R2 value from the following sample data:
X= {7,19,33,42}; Y={6,10,14,23}.

Q2. (c)

Given E[X]=0.88, E[X2]=1.12, E[Y]=0.92,E[Y2]=1.14,E[XY]= 0.55, calculate the
(5 Marks)

(5 Marks)

correlation between X and Y.

Q2. (d)

A race track is open to the public for both motorcycle and car use. The lap times (minutes) of
motorcycles is XM ~ N(u=3.4,o=1.4). The lap times of cars is Xc~N(p=3.6,o=0.78).

(i)
a group of ten motorcyclists.
(ii) Calculate the probability that a motorcycle is faster than a car.

Calculate the probability that the average lap time is between 3 and 4 minutes for
(4 Marks)

(6 Marks)

(End of Question 2)

## Paper Details

STAT08024 - Applied Statistical Analysis
Summer Examinations 2023/2024


(TOTAL MARKS: 25)

QUESTION 3

Q3. (a)

Briefly describe the terms ANOVA and family-wise error rate in the context of ANOVA.
(4 Marks)

(i)

Q3. (b)

X~Exp(A)with E[X]=1/A and Var[X]=1/X2.
State the ox value.
(ii) Explain how the value from part (i) above was obtained.

Q3. (c)

Let p be the fraction of engineers who do not understand basic statistical concepts. In
the past this has been high; p = 0.73. A new program has been implemented to im-
prove the engineers' knowledge and it is expected that p would decrease from 0.73. To test
Ho: p ≥ 0.73, H1: p<0.73, 300 engineers in the new program were tested, and 208 did not
comprehend basic statistical concepts. At the 5% significance level, can Ho be rejected in
(5 Marks)

(3 Marks)
(3 Marks)

Attendance
Amount Bet

117
2.07

128
2.80

122
3.14

119
2.26

131
3.40

125
2.93

120
2.66

130
3.33

127
3.54

(i)
(ii)

(iii)

favour of H1?

Q3. (d)

The attendance (hundreds) at a racetrack (x), and the amount (€x106) that was gambled
(y), on n = 10 selected days are given in the following table:

135
3.89

Given the following statistics: Xxi = 1254, Lyi =30.02, Xx2 = 157558
Ly? = 93.0652, Xxiyi = 3791.09, E x?y? = [REDACTED]

Calculate the sample correlation coefficient.

Determine the linear regression equation.

Provide an interpretation of the equation obtained in part (ii) above.

(3 Marks)

(3 Marks)

(4 Marks)
#
QUESTION 4

Q4. (a)

In the context of regression analysis, briefly explain the meaning of the terms: SSE, SSR,
SST.

Q4. (b)

In a two-tailed hypothesis test with a significance level of 5%, a researcher obtains a test
statistic value of z = -2.2. Determine the p-value, and explain what this value means in
relation to Ho.

Q4. (c)

A scientist is interested in assessing the relationship between two variables V1 (independent)
and V2 (dependent) and takes n = 10 sample values from a lab experiment. Given r ~- 0.96:
(i)
(ii)

(TOTAL MARKS: 25)

(3 Marks)

(4 Marks)

Sketch a scatterplot to visualise the overall pattern of the lab results. (2 Marks)
Comment on the causal relationship between V1 and V2.

(3 Marks)

Q4. (d)

It is known that 5% of manufactured components are defective. Samples of size n = 800
are drawn from the process in order to determine the proportion of defects. Determine the
proportion of samples that are likely to contain more than 6% defects.
Note: X~Bin(n,p), E[X]=np,Var[X]=np(1-p),p=X/n.

Q4. (e)

95% of X values lie in the range p±1.96 -=. Rewrite this statement in terms of a probability
equation and rearrange the equation to obtain an interval estimate for p.

(5 Marks)

σ

(8 Marks)

