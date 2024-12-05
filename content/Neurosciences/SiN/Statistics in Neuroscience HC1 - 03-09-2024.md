# Today
- Brief review of basiscs statistics
- First statistical analysis: Testing differences in ratios with Xsquared test
- Introduction to R
# Brief review of basics of statistics
## Statistical Models
- Aim is to develop a model that *describes the data well* (fits the observed values with little error) and makes *accurate predictions* about new data points
	- Described by this formula: **Outcome<sub>i</sub> = model + error<sub>i</sub>**
## Empirical research cycle
### Goal of this course:
- Choice of appropriate statistical test given your hypotheses, and the nature of your data.
	- How can one *generate falsifiable hypotheses* and *test them properly*, and in doing so gain knowledge about the world
### 1. Start with a question
- Prompted by observations about the world
- The research question you formulate defines the scope of the investiogation
### 2. Generate a *Theory*
- Organized statement about relationships between things
- Makes predictions about future observations
- Serves as a framework for your statistical model
### 3. Formulate a *Hypothesis*
- Step 1: Make statements that are *specific* and *falsifiable*
	- In science, you don't prove your theory, but you disprove the alternative
	- Use a *Null Hypothesis*: H<sub>0</sub> (negation, no effect)
		- e.g. Males and females do not differ in height (𝜇𝑚𝑎𝑙𝑒 = 𝜇𝑓𝑒𝑚𝑎𝑙𝑒)
		- “This gene has no association with depression” (𝛽 = 0)
	- Also an *Alternative Hypothesis*: H<sub>i</sub> or H<sub>A</sub>
		- 2-sided hypothesis:
			- “Males and females differ in height”  --> 𝜇𝑚𝑎𝑙𝑒 ≠ 𝜇𝑓𝑒𝑚𝑎𝑙𝑒
			- “The gene is associated with depression” --> 𝛽 ≠ 0
		- 1-sided hypothesis ( Directional, but should be used cautiously)
			- “Males are taller than females” --> 𝜇𝑚𝑎𝑙𝑒 > 𝜇𝑓𝑒𝑚𝑎𝑙𝑒
			- The gene decreases liability for depression" -->𝛽 < 0
- Step 2: Determine what the data should look like if H<sub>0</sub> is true
	- Means are equal: Observations sampled from same distribution
		 ![[Pasted image 20240903112249.png|200]]
	- Means are not equal: use statistical testing
		![[Pasted image 20240903112357.png|200]]
### 4. Collect Data to test the Hypothesis
#### 4A
- Data collected from a study will either
	- confirm the predictions & increase confidence in the theory
	- Not confirm the prediction and decrease confidence
- Strength of conclusions rest on the study design and sample representativeness
- Not single set of data will prove or disprove a theory
	- Always use replication in multiple samples
#### 4B Explore your data!
- Not officially part of the scientific method, but very important step 
- Descriptive statistics give you important information about your variables, especially for error-checking (mistakes happen easily and often)
	- Use graphs or frequency distrb. to see trends and problems
### 5. Testing your Hypotheses
- Test if there is a *Significant* association between two or more variables
	- Significance is arbitrary, but we generally use p < 0.5 
- Inference generalizes the findings within the sample back to the population as a whole
	- Is your sample representative???
## Sampling
- Population versus sample – if we could collect ALL data, we wouldn’t need inferential statistics!
![[Pasted image 20240903113222.png|300]]
## Statistical Inference
- When analyzing data in a sample, you get a parameter estimate and a measure of sampling variability (Standard Error)
- Test statistics incorporate these two into a standardized ratio of systemic to unsystematic variance, as appropriate for the type of variables analyzed
- Test statistics follow known distributions, which can be used to determine wether the observed statistic is within the typical range or outside of it
	- Fluctuations due to between-sample variability or systematic difference due to a real effect.
	- The tests follow for example the normal distribution
	- specific distribution depends on degrees of freedom in the model (df)
## Types of statistical tests
![[Pasted image 20240903113821.png]]
## P-value
- Chance of observing the data assuming that H<sub>0</sub> is true
- if p < α:
	- Test results too unlikely under H<sub>0</sub> 
	- Reject H<sub>0</sub> in favor of H<sub>a</sub> 
- if P > α:
	- Our results are likely under H<sub>0</sub> 
	- Don't reject H<sub>0</sub> in favor of H<sub>a</sub>
- Default for most tests is 2-sided
	- You wanted 1-sided? Divide the 2-sided p-value by 2!

- Drawing Conclusions
	- Think critically and report your results + interpretation accurately!
	- Draw a conclusion about your research question
	-  …but is it the correct conclusion?
	-  …and are your results meaningful?
## Types of error
![[Pasted image 20240903114906.png|300]]
## Common assumptions
Most tests we use are parametric, meaning that they assume the parameter sampling distribution (typically, but not necessarily, also the variable itself) is normal
### Parametric tests
- Observations are independent
- Data are measured at interval/ratio level
- *Testable assumptions*:
	- Data are normally distributed
	- If multiple groups: Equal variance (homogeneity of variance)
### Non-parametric tests
- Observations are independent
- *underlying continuous distribution*
## Testing for normality (just the slide)
![[Pasted image 20240903115255.png]]
## Effect size measures
### Pearson's r:
- Lies between 0 and 1
- ![[Pasted image 20240903115938.png|50]]
	- r=.10: small (1 % variance explained)
	- r=.30: medium (9 % variance explained)
	- r=.50: large (25 % variance explained)
### Cohen's d:
- Lies theoretically between 0 and ≈ |2.5|
	- d=.2: small (15 % not overlapping)
	- d=.5: medium (33 % not overlapping)
	- d=.8: large (47 % not overlapping)
	- ![[Pasted image 20240903120232.png|200]]

## How to report study results
1. Research question and hypotheses
2. Describe design and sample characteristics --> representativeness
3. N (for each subgroup)
4. Descriptive statistics (for each subgroup)
	- Mean, SD, skew, kurtosis [[Pre-processing (features)#Shape statistics| ((some extra info on this)) ]]
5. Tests of assumptions (for each subgroup)
	- SW (with df and p value), which tests for normality
6. test statistic (df), p, confidence interval
7. effect size
8. conclusion --> research question answer


# Chi-square test (χ<sup>2</sup>)
## Contingency table 
- Frequencies observed for levels of nominal and ordinal in a contingency table![[Pasted image 20240903120828.png|200]]
- These proportions are not identical, but are they significantly different?
	- χ<sup>2</sup>- test
- Assumption: sample is randomly taken from population assumed under H<sub>0</sub>.
## Example  χ<sup>2</sup>- test
- Research question: Do boys and girls differ with respect to hair color?
- Theory: hair color genes on X chromosomes --> difference
- Hypothesis:
	- H0: Boys and girls _do not differ_ in the proportions with each hair color
	- HA: Boys and girls _differ_ in the proportions with each hair color
- Statistical model:
	- Hair color<sub>i</sub> = most likely hair color (blond) + error _(null model)_
	- Hair color<sub>i</sub> = predicted hair color based on sex + error _(alternative model)_
- Expected frequencies:
	- What proportion of the sample is blond? -> 28/47 = 0.60
	- So if there are no sex effects on hair color, what proportion of boys should be blond? 0.60
	- Given that we have 22 boys in our sample, what number of them should be blond (under H0)? 0.60 * 22 = 13.11![[Pasted image 20240903121420.png|200]]![[Pasted image 20240903121540.png|200]]
	![[Pasted image 20240903121624.png]]
	- Then, lookup in  χ<sup>2</sup> table with value df --> not significant 
	- Chi-square test can only be 1-sided, as you test the squared difference between obs and exp. This cannot be smaller than 0, so you can only test 1-sidedly.
# Introduction to R
## What is R?
- Programming language
- Open-source
- Really good for data science
## What can R do?
- Clean data
- Summarizing variables
- Recording or combining variables
- Tables and figures
- Statistical analyses and hyptheosis testing
- LOTS of custom applications
## How does R do things?
- Objects
	- Different types (classes) of objects
		-  numeric (1, 42, -99) - string (“male”, “female”) - factor (0=control, 1=treatment)
	- 1-D (vectors), 2-D (matrices, data.frames), or multi-dimensional (lists)
	- Assign value(s) to objects:
		- objectName <- 74
	- Multiple values are stored in elements, which can be indexed:
		- objectName[rowNumber, columnNumber]
- Functions
	- Small bits of code that perform an action on objects
- Packages
	- Larger sets of code that store functions
	- allow any user to make and share new functions
	- Install packages before first use and then load when you start a new session to make functions available.
## Console
-  Interactive window for running commands
- Display results
- View and export tables and figures
## Syntax window
- Keeps a permanent record of commands
- send commands to console
- add comments for documentation (#)
- requires proper vocabulary and grammar (commands and syntax)
