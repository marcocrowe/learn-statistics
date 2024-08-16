
# Work

**Step 1: Calculate the Regression Line**  
We first need to find the regression line of $Y$ on $X$. The equation of the regression line is:

$Y = \beta_0 + \beta_1 X$  

where $\beta_0$ is the intercept and $\beta_1$ is the slope.

Calculate the Slope ($\beta_1$) and Intercept ($\beta_0$)

1. **Means of X and Y:**
   $\bar{X} = \dfrac{7 + 19 + 33 + 42}{4} = \frac{101}{4} = 25.25
   $  
   $\bar{Y} = \dfrac{6 + 10 + 14 + 23}{4} = \frac{53}{4} = 13.25
   $

2. **Calculate the slope ($\beta_1$):**
   $
   \beta_1 = \frac{\sum (X_i - \bar{X})(Y_i - \bar{Y})}{\sum (X_i - \bar{X})^2}
   $

   Compute the necessary sums:
   $
   \sum (X_i - \bar{X})(Y_i - \bar{Y}) = (7 - 25.25)(6 - 13.25) + (19 - 25.25)(10 - 13.25) + (33 - 25.25)(14 - 13.25) + (42 - 25.25)(23 - 13.25)
   $
   $
   = (-18.25)(-7.25) + (-6.25)(-3.25) + (7.75)(0.75) + (16.75)(9.75)
   $
   $
   = 132.5625 + 20.3125 + 5.8125 + 163.3125 = 321.0
   $
   $
   \sum (X_i - \bar{X})^2 = (7 - 25.25)^2 + (19 - 25.25)^2 + (33 - 25.25)^2 + (42 - 25.25)^2
   $
   $
   = (-18.25)^2 + (-6.25)^2 + (7.75)^2 + (16.75)^2
   $
   $
   = 332.5625 + 39.0625 + 60.0625 + 280.5625 = 712.25
   $
   $
   \beta_1 = \frac{321.0}{712.25} \approx 0.451
   $

3. **Calculate the intercept ($\beta_0$):**
$\beta_0 = \bar{Y} - \beta_1 \bar{X}$  
$\beta_0 = 13.25 - 0.451 \times 25.25 \approx$  
$13.25 - 11.40 = 1.85$

So the regression line equation is approximately:
$
Y = 1.85 + 0.451 X
$

**Step 2: Calculate $R^2$ (Coefficient of Determination)

1. **Total Sum of Squares (SST):**

| $Y$  | $\overline{Y}$ | $(Y - \overline{Y})$ | $(Y - \overline{Y})^2$ |
|----|----------------|----------------------|------------------------|
| 6  | 13.25          | -7.25                | 52.5625                |
| 10 | 13.25          | -3.25                | 10.5625                |
| 14 | 13.25          | 0.75                 | 0.5625                 |
| 23 | 13.25          | 9.75                 | 94.0625                |
| | | **SST** | **157.75** |


   $
   SST = \sum (Y_i - \bar{Y})^2
   $
   $
   = (6 - 13.25)^2 + (10 - 13.25)^2 + (14 - 13.25)^2 + (23 - 13.25)^2
   $
   $
   = 52.5625 + 10.5625 + 0.5625 + 94.0625 = 157.75
   $

1. **Residual Sum of Squares (SSE):**

| $\hat{Y}$  | $\Beta_0$ + $\Beta_1 X *$ | $(Y - \hat{Y})$ | $(Y - \hat{Y})^2$ |
|-----------|-------------------------|----------------:|------------------:|
| 5.007     | 1.85 + 0.451 * 7        | 0.993           | 0.986             |
| 10.419    | 1.85 + 0.451 * 19       | -0.419          | 0.173             |
| 16.733    | 1.85 + 0.451 * 33       | -2.733          | 7.353             |
| 20.792    | 1.85 + 0.451 * 42       | 2.208           | 4.930             |
| | | **SSE** | **13.442** |


1. **Calculate $R^2$:**
   $R^2 = 1 - \dfrac{SSE}{SST}$  

   $R^2 = 1 - \dfrac{13.442}{157.75} \approx 1 - 0.085 = 0.915$

**Interpretation
- **$R^2 = 0.915$** indicates that approximately 91.5% of the variability in $Y$ can be explained by the variability in $X$ through the linear regression model.
- This high $R^2$ value suggests a strong linear relationship between $X$ and $Y$. The regression model does a good job of explaining the variability in the dependent variable $Y$.
