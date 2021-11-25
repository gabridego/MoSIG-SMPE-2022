# SMPE - Lecture 6 25/11/2021

## More comments on parallel quicksort algorithm
- How confident can we be about an algorithm being better than others? How general are conclusions? Results depend on used machine and number of runs.
Strong bias on used machine (**pseudoreplication**, different from replication), can only draw conclusion on local machine, not on all world.
- Optimization impacts on results, line may not cross anymore.
- What can impact on the results? (Fishbone diagram):
	- number of repetitions
	- number of threads and CPU
	- algorithm
	- memory
	- kernel version
	- library version
	- pinning (check threads are not all going to the same CPU)
- Cannot observe experiment without perturbating it. A profiler can analyze it from the outside.

## Comments on Fitt's law exercise
- Many things have impact:
	- distance and width (parameters of the problem)
	- device
	- qualities and behavior of practitioner
	- instructions given to practitioner
	- elapsed time since experiment started (practice and fatigue)
- Ideally, device would understand if practitioner is distracted or tired
- Very likely that law does not hold if width is too small

## Statistics
Different notions of intervals (confidence, credibility, fluctuation, ...), different meanings but sometimes are computed in the same way. Intuitively,
the more experiments we make the closest we get to the true value. Tradeoff between precision and cost, but we can still be unlucky in the results we obtain.

The more experiment is controlled, the lower the variance, but bias is introduced.

### Central limit theorem
Does not assume any particular data distribution, just that mean and variance is defined. We can use sample variance, not true variance. If an upper bound to
the true variance is known, it should be used.

For most distribution, convergence in term of area to a gaussian after 30 repetitions. With less than 30, Student's t-test, but assumes normal distributions.

Things should be as independent as possible, use randomization (flipping a coin).

### Abnormal measurements
How to handle outliers? The definition of outlier depend on the context. Data can be safely removed if we know something went wrong during the experiment and
that data point does not represent the real behavior. Otherwise, it's cherrypicking. Only drop if there is a good reason to do it.

Sample mean is very sensitive to outliers.
