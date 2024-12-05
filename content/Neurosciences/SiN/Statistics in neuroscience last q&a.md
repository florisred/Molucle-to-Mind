## Will we have to know how to interpret the g*power program?
 - No, just conceptual questions on power
## Z-score or cohen's d?
- Whenever we use parametric tests, we probably get z-scores
	- Then its better to report them
- Cohen's d if not
## When do we calculate the effect size & when do we record it?
- If you are writing a paper, then I think its really good practice to report the effect size
	- Often, it is not reported -> but it should be!
- Can also score you some extra on your poster if you report them -> you can still update your poster if you want to take advantage but youve already uploaded!
## How do we interpret z-scores?
- If we look at the normal distribution, a z-score of 1 means one standard deviation outside of the mean. 
## Helmert's contrast, how to interpret?
- A helmert contrast is used when you have *4 groups*
	- Two *sigle manipulations*, one group where they are *combined*
- The helmer contrasts specifically test whether a *combination of two* is different than a single manipulation -> does the combination do anything
Lets say you have the following observations:
- **Co**ntrol, **Dr**ug, **Th**erapy, (**D**+**T**) - a combined condition
- 1st test: **Co** v.s. D + T + (D+T)
- 2nd test:  (**D**+**T**) v.s. **D**+**T** (to se if there are any differences from combining them in a condition, or just adding the means together) 
	- You are specifically testing whether the combination of the two does more than just combining the mean of the two conditions
- 3rd test: **D** v.s. **T**
## When are contrasts used?
- When you have an ANOVA test, multiple groups you want to compare the mean of
- The significance of the ANOVA test means that any of the means are different in lump, contrasts can help you see where and how the difference comes
## I cannot get a grip on dummy coding, what should we know about it?
- Made the exam like 5 weeks ago, so she cannot remember what is in there
- But, you have to know *WHY* you use dummy coding in regression
	- Because R will see it as a linear trend, (group 1 is smaller than group 2) 
		- So you have to factorize it
	- If you want to put it in a regression model, you make one group your 'baseline' group, and compare all the other groups to it
- You only dummy code for categorical (nominal) variables
## We were testing the significance of a variance, that was one sided (as it cannot be negative), but later we tested the significance of a predictor, what kind of test is that?
- A predictor can both be negative and positive -> two sided chi-square test
## In the assignment we had the example of a wild type vs a knock out mice, two groups, but within each group multiple mice and multiple measurements of neurons. What is the cluster level we are looking at?
- So, so, this is  a god question because in neuroscience we often have multiple levels , (neurons in mice), but uou could also have more levels (vesicles in different neurons in different mice)
	- We only tested two levels, but there are ways to do more levels -> not necessary for exam
		- Can be done by adding a random term or by adding a covariate
## Why do we do the p divided by 2? 
- If we are testing a variance term, it cannot be negative -> it is one sided. To adjust for this, you have to divide the p by two
## How problematic are the correlations between predictors? I dont know how to answer that question
- The level of problematicness is expressed by the VIF
	- VIF = 1: no problem
	- VIF = 5: seriously problematic
- If the VIF is low, there is no problem with multicollinearity
## When you plot data, can you see based on the graph whether the vif is high?
- no, but you can see if they are highly correlated
	- If you make a scatterplot, and it kinda looks like a line, that is *bad*
## I still do not understand the significance of the chi-square test
- Which one?
	- *thats what im confused about, you use them many times and it seems confusing*
- Well, the chi-square test is a general type of test (like f test, both used in ANOVA and Regression)
	- Chi-square test is used to *compare fit of different models*, and a *cross-tab test*

## Is the practice exam on canvas representative
- Yes, very comparable in contents & length
- 20 mc questions
	- Are there interaction effects, which test to use, report the right data from the R output, etc. 
- 6 open questions with subquestions
	- Always gonna be one on power, repeated measures anova, etc. 
- The *decision tree for all the tests* will be provided int the test
## Repeated measures anova is always one sided right?
- You answer three questions:
	- Is there a difference over time?
	- Is there a difference between groups?
	- Is there an interaction effect?
## The research question at the beginning of the variable is one-sided, but you have a two-sided test:
- You divide the p-value by two
- Only do a 1-sided test if it is logically impossible for the values to turn the other way around
	- You cannot age backwardly, After knocking down a gene that expression cannot go up
