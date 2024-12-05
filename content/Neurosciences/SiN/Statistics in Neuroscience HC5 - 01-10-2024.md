## Lessons from the assignment
- When the mauchly test is violated, look at the table with weird degrees of freedom --> this is the *adjusted* score!
- ALWAYS REPORT ALL DESCRIPTIVE STATISTICS
	- Median when working with ranked scores
- always report two decimals p value, not do <, but 3.2e-15 for example

## Multiple regression
- Increasing the number of predictors
	- So predict *weight* with *height*, *age*, and *heartrate*, not just *height*, for example.
- The concept is very much the same as simple regression
- The *betas* are not comparable, as they differ in scale. 
	- You need *normalized beta-values* for that or *z-scores*
- Betas can be interpreted as the change in outcome with 1 unit change in one predictor while keeping the others at 0. 
- Why? 
	- Joint effect pf multiple predictors
	- Control for confounders / covariates
	- Study effect of new predictor over and above known predictors
- Whenever you do interaction research, *scaling* is very important
	- First make z-scores of your predictors!
### Multi-colinearity
- If you have multiple predictors and they are highly correlated, you cannot estimate the betas
	- Solution: *VIF* --> Variance Inflation Factor, a measure of redundancy
	- VIF = 1 --> al lis good
	- VIF > 5: Very correlated, not good
	- VIF > 10: remove!!!
### Dummy coding


### multiple testing
 - 