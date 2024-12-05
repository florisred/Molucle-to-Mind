# Missed the first one
# GWAS -> DRUG
## Why?
- silly question, seems quite obvious
- drugs are good
- It takes a lot of money to develop and get approved new drugs
	- Worse for CNS disorders, often found by chance
	- Very difficult to have a systematic approach to finding drugs
- We *need more drugs* -> yes
	- 20%-30% of schizophrenia patients do not respond to medications
## Drug repurposing
- Finding new uses for already approved drugs
- You already know the safety profile
- Con: doesn't make as much money
	- Thats a terrible con, i hate the fact that this is even a consideration
	- we have nothing to lose but our chains, rise up, proletariat!
- Example 1: Viagra
	- Was originally approved for high blood pressure
- Example 2: Aspirin
## How to go from GWAS to novel treatments?
- many ways
- Examine drugs targeting significant loci
	- Was done in Crohn's disease
	- But, there are many different loci, and even the genes have like 200 possibilities
	- Makes it very hard to predict what the drug will do
- Two other approaches
	- Drug gene-set anlysis
	- signature matching
## Drug gene-set analaysis
- Genetically informed drug repurposing method
- Identifies drugs that are known to target genes associated with your phenotype
- Affordable to identify candidate drugs
- Quick and customizable
- MAGMA review: post-GWAS analysis
- You create drug-gene sets, and perform competitive analysis to see which drugs would likely affect disease
	- You can also create drug groups, to prioritize drugs
	- To look for potential drugs that are not approved yet to make it more enticing for big pharnma
- Limitations:
	- Can exacerbate disease symptoms because there is no directionality
	- Limited by knowledge of known drugs - gene interactions
		- Can bias results (into drugs we have researched more)
## Signature matching
- Try to account for limitations in drug gene-set analysis
- Requirements:
	- Disease signature
		- Some gene or protein expression associated with disease stae
	- Drug signature
- Select drugs that counteract 
- Question: can you also 

# Applying GWAS on MRI
## Imaging-genetics
- New field, to be shaped by you and me!!!
## Why would you do this?
- Behavioral traits or neuropsychiatric conditions are often
	- Heterogeneous
	- Highly polygenic
	- Prone to gene-environment correlation
- What if we study phenotypes that are more homogeneous, less polygenic, and closer to biology
- That is why we use *endophenotypes*! (discussed before)
	- Closer to biology
	- Less complex than a disorder
	- In causality before disorder
	- Has to fulfill certain criteria
## How do you do this?
- Scan a lot of people and genotype them and run a GWAS
	- Challenge: GWAS require large sample sizes
	- But, MRI is very expensive, so where you gonna find the data?
- Cannot go from voxel to GWAS
	- But, you can go from voxel to a singular number for example prefrontal cortex from structural, different networks from fMRI, or white matter tracts from DTI
	- IDEA: finding the most important markers for a specific trait
		- Like my feature reduction thesis, but applied to gene-imaging
## Genetic architecture
- how can we describe the genetic architecture of a trait?
	- Heritability
	- Polygenicity
	- Discoverability
	- Pleiotropy