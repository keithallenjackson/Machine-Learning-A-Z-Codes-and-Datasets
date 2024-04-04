 
## Feature scaling
**Normalization**

$X' = \frac{X - X{min}}{X{max} - X{min}}$

**Standardization**

$X' = \frac{X - \mu}{\sigma}$

$\mu$ is average

$\sigma$ is std deviation

## Linear Regression

Assumptions of Linear Regression

1. Linearity (linear relationship between Y and each X)
2. Homoscedasticity (equal variance)
3. Multivariate Normality (normality of error distribution)
4. Independence (of observations. Includes "no autocorrelation")
5. Lack of multicollinearity (predictors are not correlated with each other)
6. The Outlier check (this is not an assumption, but an "extra")


### Simple Linear Regression
$\hat{y} = b_0 + b_1X_1$

$\hat{y}$ is the dependent vairable

$b_0$ is the y-intercept (constant)

$X_1$ is the independent variable

$b_1$ is the slope coefficient

_How to find the best linear regression_: **Ordinary Least Squares**

$y_i$ (actual data point), $\hat{y_i}$ (point on linear regression line from at same x-axis point), $\epsilon_i$ is called the residual with the equation: $\epsilon_i = y_i - \hat{y_i}$

$b_0$, $b_1$ such that: $SUM(y_i - \hat{y_i})^2$ is minimized

### Multiple Linear Regression

$\hat{y} = b_0 + b_1X_1+b_2X_2 + ... + b_nX_n$

$\hat{y}$ is the dependent variable

$b_0$ is the y-intercept constant

$b_n$ slope coefficient for each $X_1$ independent variable

**Dummy Variables**

Used when doing linear regression and one of the independent variables is categorical (like State or City). 

**Dummy Variable Trap**

When creating dummy variables from categorical independent variables, always omit 1 of the category dummy variables.

$D_2 = 1 - D_1$

### Polynomial Linear Regression

$y = b_0 + b_1x_1 + b_2x_1^2 + ... + b_nx_1^n$

**Why _Linear_ when having powers?**

What makes a model linear is not the $x$ values and the operations done on it, but rather the coefficients ($b$ values). The $b$ values do not have any powers applied to them.

## Support Vector Regression (SVR)
