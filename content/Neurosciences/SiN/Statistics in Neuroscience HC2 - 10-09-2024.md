# Quick things
- You *SHOULD WATCH ALL THE VIDEOS / READ THE BOOK IN ADVANCE*
- Assignment things:
	- Went well, but keep track of what you are testing
	- If you have to redo it, you will be emailed about it
	- report with 2 decimals throughout the report, uless you want to make a specific point.
## Testing for normality
- Kolmogorov-Smirnov test: H0 of no difference between cumulative frantion of any theoritical distribution and observed data 
## 1.2
- extreme behavior -> regular population will have floor effect.
### Central limit theorem
- CLT is about sampling theory, not the observed data
1. Draw a sample N>30 from the opulation
2. calculate the mean or SD in that sample
3. repeat this many times
4. determine SD and Means of samples
5. These are normally distributed

# Correlation & regression
## Positive & Negative correlation
- Positive: one score goes up, the other too, 
	- Ranges from 1 - 0
- Negative: One score goes up, the other goes down
	- ranges from 0 to -1
- 1 and -1 is a very strong correlation, 0 is the least strong
## Pearson correlation
- Calculation by hand:
	1. Calculate means
	2. calculate deviation of each score from men
	3. Calculate standard deviation
	4. Calculate the co-variance -> scale dependent
	5. Calculate correlation --> not scale dependent
		- To do this, you divide by standard deviation
## Spearmans Rho
- Rank scores, sometimes results in *confidence intervals*

## Regression
- Checks if there is a (significant) relation between two different scores
- b<sub>0</sub> is the intercept
	- what one score is when the other is 0 
- b<sub>1</sub> is the slope
	- the amount of change per unit in other score

### Means model
- Without any other predictor, the mean is the best predictor for the next value
- just a straight line, which you have deviations from
### Regression model
- Including predictor, now has a *slope*
- The question is if this has lower *residuals*, thus describes the data better
	- The difference between predictions and observations
- R outputs the F-statistic
### F-statistic
- Based on sums of squares
	- Calculate total sum of squares
	- compares the fit of the model without the predictor
	- Ratio of what is explained by the model vs what is not explained by the model
- What does a large f mean? the model predicts more than is not predicted by the model
- SS<sub>T</sub> total sum of squares -> sum of error assuming b<sub>1</sub> = 0
- SS<sub>R</sub> = residual sum of squares --> minimized by regression line
- SS<sub>M</sub> = model sum of squares -> improvement regression model b1 is not 0
- F = SS<sub>M</sub> / SS<sub>R</sub>
- R<sup>2</sup> = SS<sub>M</sub> / <sub>T</sub>
### Hypothesis testing
- Generally we are not interested in the significance of the intercept
- We are interested in the significance of b<sub>1</sub>
- Correlation: *standardized, symmetrical*
- Regression: *not standardized, not symmetrical*
- they do have different steps 
	- regression has a predictor and dependent
	- 