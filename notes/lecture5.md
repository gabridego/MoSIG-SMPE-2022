# SMPE - Lecture 5 18/11/2021

## Comments on Challenger exercise
- How confident can we be on predicted probability of failure? What if new observations are added? Confidence intervals can be plotted, but different results can be obtaines. R and Python behave differently.
- It is not straightforward to run the same code on different machines, need installation/import.
- Statistics does not tell everything about reality. It assumes a model, but may not apply in reality.

## Comments on quicksort exercise
- Theoretical complexity of quicksort is nlogn, we should expect the line to follow it.
- For linear regression, in R geom_smooth().
- The program should not be doing what it is supposed to do... and may not be optimally compiled (-o 0)
- Always check what we are measuring, does it make sense? Is it what we expect?
- Experiments should be executed in the same conditions. For example, still using the machine during execution?
- A lot of aspects impact measurement, experiments should be isolated.
- Different machines perform differently, all parameters should be listed and organized (**fishbone diagram**).
- Experiments can be randomized in order of execution, in order to lower the effect of perturbations.

## Considerations on performance measurement
- Several metrics used in different fields, not always directly measurable. Different requirements, not always satisfied.
