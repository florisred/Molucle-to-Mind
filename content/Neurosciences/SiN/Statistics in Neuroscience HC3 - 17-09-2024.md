# [[The T-test]]

# Anova
- When you want to compare more than two means
## One-way ANOVA
 - First you have the means model --> compare every single observation to the overall mean
 - Secondly there is a model where the means of the different groups are taken into account
	 - You hope that the residuals will be lower like this.
### Formula one-way anova
![[Pasted image 20240917115727.png|200]] with ![[Pasted image 20240917115617.png|400]]
### Post-hoc contrasts
- Its very common to run a selection of *hypothesis driven tests* after the test instead of all *pairwise comparisons*
- There are several different ones:
#### Simple contrasts:
- You only compare the control group vs all the subgroups individually
#### Repeated contrasts
- Compare 1-2, 2-3, 3-4 but not any others
#### Helmer contrast
- Compares each level with subsequent levels
![[Pasted image 20240917120550.png]]
![[Pasted image 20241014232914.png]]
## Two-way ANOVA
- Compares multiple means, When you manipulated one or multiple independent variables
- Has multiple (now two) different predictors for the dependent variable
### interpretation of two-way anova
#### Main effect
- 