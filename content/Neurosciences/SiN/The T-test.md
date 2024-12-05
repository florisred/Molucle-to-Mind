# T-test
## What can you answer with this test
- Do the *means* of *two groups* differ significantly
	- Also about SD, not only about means
	- a higher SD will mean more overlap, so that means less statistically significant
- Unsystematic variation is the variation not due to your experimental setup
	- Systematic variation is about the mean
## How does it work?
 ![[Pasted image 20240917113543.png|300]] and ![[Pasted image 20240917114249.png|200]]
- observed difference between means (systemaic variation) - expected difference under H0
	- divided by unsystematic variation SE
## Assumptions
- Variances of the two groups are the same
	- You can test this with the *Levene Test*
		- If it is significant, the variances are significantly different 
- Data are normally distributed
- measurement level is at least *interval*
- Data points must be independent!! --> will be discussed more next week
## Effect sizes
![[Pasted image 20240917113749.png|100]]
## T-test as a regression model
- two groups, code one as 1 and one as 0.
	- *Intercept*(a) is mean of group 0, 
	- *the slope* (b) is the difference between them in means. 
- b is the parameter of interest when you want to test for significant