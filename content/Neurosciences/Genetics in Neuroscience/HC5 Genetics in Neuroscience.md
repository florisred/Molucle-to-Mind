## Convergent effects of different types
- Different types of evidence of the same genes 
- ![[Pasted image 20241126154446.png]]
## Why do we want to look for convergence?
- Is it biologically meaningful?
## Testing for functional clustering of SNP associations
- Gene-set analysis with sets of genes as unit of analysis
	- Targeted gene-sets/pathways
- You look at the joint association of all SNPs
- Pros
	- Reduce multiple testing by prioritizing genes in biological pathways or in groups of functionally related genes
	- Increases statistical power
	- Deals with genetic heterogeneity
	- Provides biological insight
- Cons:
	- Garbage in, garbage out
		- Crucial to select reliable sets of genes!
	- 
## Gene-based analysis
- If a single SNP is not significant, but many SNPs toward a single gene *are*, then you can do a gene-based analysis
	- You no longer really get the analysis of single SNPs, but a more aggregated score
	- Requires a lower P-value
	- But also results in a lower p-value
- Pros:
	- Reduce multiple testing (from 2,5 million SNPs to 20k genes)
	- Accoutns for heterogenity in gene
	- Immediate gene-level interpretation
- Cons:
	- Disregards regulatory information when using standard gene mapping (you can alleviate this with eQTL information)
	- still a lot of tests
## How to define gene sets?
- Protein interaction networks
	- Using Y2H or co-immunoprecipitation
- Can also use co-expression networks
- Can use cell type specificity analysis
	- See if the genes are actually expressed in the cells
## Self-contained vs competitive tests
- Null hypotheses:
	- Self-contained: The genes in the gene-set are not associated with the trait
	- Competitive: The genes in the gene-set are not more strongly associated with the trait than the genes not in the gene-set
- For self-contained methods, rates increase with heritability, whereas they are constant for competitive methods
	- This is because you account for it with competitive tests
- Competitive tests define which combinations are biologically most interpretable
- When we have a larger gene size, we will include more SNPs in our gene sets, which can artificially inflate effect sizes
	- Different methods respond differently to this
## Issues of interpretation in gene-set analyses
- GSA tests for *accumulation of effects* within genes within the sets, could be due to:
	- Direct effect: the set itself in involved
	- Confounding: The set itself is not involved, but many genes in the et overlap with another *causal* set 
	- Interaction: The set is partially involved, the effect specific to a subset defined by another gene set
### Marginal vs conditional analysis
- Marginal: average of all p-values of every gene in a set
- Conditional: association is the effect of a specific sub/superset corrected for another sub/superset, allowing you to more specifically see the effect of a specific subset
### Interactional analysis
- 2 sets, with both a part overlapping with each other.
	- If the parts (and only the part) that overlaps with both is very significant, it would suggest an interaction effect
## Interpret GWAS risk loci
- Step 1:
	- Annotate all GWS SNPs in risk loci, with as much biological information as we have
- Step 2:
	- Map annotated SNps to genes, using positional, eQTL, and HiC mapping (or anything we can get our hands on)
- Step 3:
	- Interpret polygenicity, test for pathways, tissuesm and cell types
		- Genes that are similarly similarly active / expressed (FUMA/MAGMA)
## Functional experiments for a plygenic problem
1. Single cell technology
	1. Alows you to profile gene expression for individual cells, map gene expression levels to single cells
2. Novel neurobiological tools that do not necessitate the focus on signle genes
	1. DREADD, iPSC
- You integrate GWAS and look for sensical follow-ups
	 - A good bridge between genetics and neurobiology
## SNP associations
- Many SNPs aggregate in a single gene, many genes contribute to 1 function
- *Bottom-up study design:* Looking a SNPs, looking at phenotype
- *Using endophenotypes:* Paying more attention at what happens in between
	- Could make for more informative or testable hypotheses
	- Endophenotypes are intermediate phenotypes
### Endophenotypes
- Intermediate (biological traits that lie int he pathway between the genes and behavior/disease)
	- More power to study, because they are closer (fewer steps in between) the SNPs
- 3 criteria
	- associated with disease / trait
	- More prevalent in relatives of affected individuals than in the general population
		- Closer to SNP, so more likely to manifest in relatives than the full disease
	- Heritable & genetically correlated with disease/trait
### Top-down model
- You look at different subtypes of a disease as well
	- Different SNPs might only correlate with a certain subtype
	- If you take this into account, you can have a lot higher power
- Like with alcoholL
#### Collective syndrome of “Alcohol Use Disorder” (DSM/ICD):
- Must exhibit some combination of symptoms:
	• Tolerance
	• Withdrawal
	• Drank more than intended
	• Unable to reduce use
	• Craving
	• Much time spent obtaining/using/recovering from alcohol
	• Important activities given up due to use
	• Use despite physical or psychological complications
	• Hazardous use (e.g. drunk driving)
	• Drinking interfered with responsibilities
	• Continued use despite harms to relationships
- These clusters of symptoms were made 100 years ago by some psychiatrists, which might not be the most accurate lol
- If you have the same types of global clustering, the specific symptoms or causes might be *very heterogeneous*
- So, if you do twin modeling and genetic factor analysis, some sets of genes cluster together with specific symptoms
	- Genetic factors:
		1. Tolerance and excess drinking
		2. Loss of control and social dysfunction
		3. Withdrawal and continued use
- Means that dimension of alcohol misuse are genetically distinct
- 