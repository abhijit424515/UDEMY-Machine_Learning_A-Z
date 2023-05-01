# Machine Learning

## Guidelines
- Always separate data into training set and test set

## Pre-processing
### Feature scaling
- Normalization $(X - X_{min})/(X_{max} - X_{min})$
- Standardization $(X - X_{min})/\sigma$

## Regression
### Simple Linear Regression
For a given set of points in 2D, find an optimal line $\hat{y} = b_0 + b_1x$ that can best predict y, given x.
The **best** point will depend upon application, so the error function may vary.
Most common error function: $\sum{(y_i-\hat{y_{i}})^2}$

### Simple Linear Regression
For a given set of points in n-dimensions, find an optimal line $\hat{y} = b_0 + b_1x_1 + ... b_nx_n$ that can best predict y, given $\bar{x} = (x_1,x_2,...,x_n)$.
The **best** point will depend upon application, so the error function may vary.
Most common error function: $\sum{(y_i-\hat{y_{i}})^2}$

## R-Squared
$$
SS_{res} = \sum{(y - y_i)^2} \qquad SS_{tot} = \sum{(y - y_{avg})^2} \\
R^2 = 1 - \frac{SS_{res}}{SS_{tot}}
$$

Rule of thumb for values of R^2:
- 1.0 --> Too perfect (sus)
- 0.9 --> very good
- < 0.7 --> not great
- < 0.4 --> terrible

## Adjusted R-Squared