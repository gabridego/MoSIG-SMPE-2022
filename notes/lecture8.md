# SMPE - Lecture 8 09/12/2021

## Analysis of variance
Formulas are on the [slides](https://github.com/alegrand/SMPE/blob/master/sessions/2021_10_Grenoble/08_anova.pdf).

We consider the case of balanced experiment design, data are balanced with respect to all predictor modalities.

- One factor ANOVA: test if predictors have impact on response
- Two factor ANOVA: a predictor may have an impact if in interaction with another one. Interaction variables are added to the expression.
Different significance test for different predictors and for interaction variables.

## Recap of previous lectures
Possible pitfalls: unbalanced experiment design, missing observations for some combinations of parameters when working with experimental observations
(results obtained grouping observations can be consequence on methods using for grouping), collinearity, biased data (measurements depend on where they
are sample from).

Common wrong hypothesis: linearity, normal residuals for ANOVA, noisy factors (the more observations, the more confident you are, but conclusions are still
wrong), building model and adding variables at will (adapting model on fixed dataset, overfitting of conclusions, building hypothesis on the fly breaks the
results, hacking), spurious correlations.
