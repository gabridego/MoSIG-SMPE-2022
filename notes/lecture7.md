# SMPE - Lecture 7 02/12/2021

## Linear modeling
Formulas are on the [slides](https://github.com/alegrand/SMPE/blob/master/sessions/2021_10_Grenoble/07_linear_regression.pdf).

- Data have different types, we work with quantitative data.
- Regression helps to extract information from data, as relations between variables.
- "Eyeball" method: draw line that pass through maximum possible number of points.
- Minimize distance in term of projections of points on the line, but several metrics are available.
- In classical linear regression, least squares are minimized.

Linear regression relation is satisfied for each data point. We look for beta parameters that minimize squared distance of data points from the line (Ordinary Least Squares estimator).

Good estimators are unbiased and with minimal variance. Residual variance is an unbiased estimator of the true variance.

ANOVA (analysis of variance) considers response variation explained and not explained by the fitted model (SST = SSM + SSE). Model evaluated with coefficient of determination
R^2 = SSM / SST, between 0 and 1: 1 if all information is included in the model, 0 if the model explains nothing. However, R^2 close to 1 does not mean that data are well
summarised. In this case analysis must be carried out looking for shapes in the data.

Significance of parameters must then be tested, to verify that they contribute to the model.

p-value: how likely it is that null hypothesis is verified.
