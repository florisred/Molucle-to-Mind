## Nested data in neuroscience
- The t-test, anova, etc, all hinge on the idea that the data you collect is independent
	- However, in Neuroscience you often have data from multiple doctors and multiple individuals
		- We can call this *clustered data*
	- When multiple observations are all from one doctor / individual, and other observations from another, this assumption is violated!
## Measure of dependency: ICC
- *Intra-cluster Correlation*
	- A measure of how much of the variation in the sample is due to measuring multiple clusters
	- Proportion of systematic variance of the total variance
	- Proportion variation in the dependent variable that is attributable to the clustering
- *High ICC* -> variation in data due to the clustering of the data
- *Low ICC* -> variation in data not due to the clustering of the data
### Effective sample size
- This is the minimum sample size for it to be effective $$\displaystyle{\displaylines{Neff = \frac{ Ntotal}{1+(n-1)*ICC}}}$$
- If it is lower than this, you too often conclude that the effect is significant
### Handeling dependency
- Three ways:
	1. If you have a balanced test, you can do a *pooled t-test*
	2. Take a random observation from each cluster
		- 1 + 2 will render observations independent, such that standard techniques can be applied
		- However, information and thus power is lost. 
	3. Multi-level analysis
		- Uses all available information and is thus most powerful
### Multi-level analysis
- regular regression:
	- y<sub>i</sub>=  b<sub>0</sub> + b<sub>1</sub>G<sub>i</sub> + error<sub>i</sub>
- Multi level:
	- y<sub>j</sub>=  b<sub>0j</sub> + b<sub>1</sub>G<sub>j</sub> + error<sub>j</sub>
	- b<sub>0j</sub> = b<sub>0</sub> + u<sub>0j</sub>
- So it is very similar, only the Intercept is different. 
	- We call this a *random intercept* -> not actually random, but different for each cluster. 
