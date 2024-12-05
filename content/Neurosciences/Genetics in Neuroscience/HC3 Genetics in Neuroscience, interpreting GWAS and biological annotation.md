## Terms people get confused from
- Genetic variation
	- Lots of different variation in the genome -> genomic variance
	- Types of variance:
		- SNP -> we look at the most, most common (single nucleotide polymorphism)
		- Mutation -> any new / disease causing change in the genome
			- If a mutation becomes common, its a polymorphism
		- CNV -> copy number variation
		- Markers: Another term for variants, usually SNPs
	- Alleles / genotypes: exactly which sequence a person has on a specific locus
## DNA variation -> Phenotypic variation
- Therefor, monomorphic sites are not relevant for GWAS
- SNP (rare or common), most frequent variation, GWAS variants
- Copy number Variants (CNVs):
	- Insertion / deletion
	- Duplication
- Inversion
## Identify DNA variation -> disease mechanism
- We can identify variations in DNA, but we really want to know the disease mechanism
- First step is *gene discovery phase* (GWAS) -> looking at which genes are correlated with disease outcome
	- We have gotten pretty good at this
	- Challenge: we know what the variation is, challenge to understand *why*
		- If it is statistically relevant, the question becomes what biological outcome it has
		- We already have quite a bit of knowledge about the genome, to infer something about the function of the genes / variation
			- For example, with *FUMA*, can link candidate SNPs to a certain function
			- We can also aggregate the effects of different SNPs
				- If there are multiple different variants affecting the same gene, we can aggregate the effects using *MAGMA* for example
			- We can also use this to find drugs that downregulate the affected genes for example --> week 6
- Any results we get from GWAS are not experimentally confirmed -> we need to design experiments or mouse models in order to confirm!
	- Proving causation is very hard, costs a lot of resources! 
	- Not something you just kind of want to do -> important to interpret GWAS results to find most likely candidate genes
## Starting simple: Mendelian traits
- Monogenic traits -> only caused by a single allele, and then its certain you get it
	- Always gonna be seen very highly in families
	- Also makes it easy to find the gene & to do causal experiments
## Complex traits
- We didnt really start with this until GWAS era -> 2006
	- Fundamentally polygenic disorders are a different beast
	- All genes have a small effect, that might increase the chance for developing disease like 1-2%
		- Many people that have the allele will not have the disease, many different diseased people will not have the gene -> makes it difficult to find them!
	- Regions of the genome that are found are often *not* areas that code for a genome, but in the non-coding area
		- Makes it even harder to find a biological explanation
## Criteria for causality

| criterion                                                     | Mendelian traits | polygenic traits |
| ------------------------------------------------------------- | ---------------- | ---------------- |
| Strength size -> larger association -> more likely its causal | this             |                  |
| Consistency -> between samples                                | both             | both             |
| Specificity -> single cause causes single effect              | this             |                  |
| Temporality -> cause precedes outcome                         | both             | both             |
| Biological gradient -> greater exposure leads to more outcome | both             | both             |
| Plausibility -> consistent with processes                     | both             | both             |
| Coherence -> compatible with theory                           | both             | both             |
| Experimental change                                           | both             | both             |
| Analogous (to other processes)                                | both             | both             |
## Why do we want to know the causal SNPs?
- Those can point in the direction of a potential remedy or prevention
	- You do not have to know the causal SNPs to find correlation / prediction of disease
- We need:
	- *Actionable* variant
		- Something we can manipulate in a design 
	- *Large effect sizes*
- 4 issues with GWAS results:
	1. GWAS hits are mostly located outside of genes
		- A few years ago we looked at a catalogue, and 93% are located outside of genes 
			- Often in *active chromatin* (27.74%) and *eQTLs* (57.41%) -> will be talked about more
		- Not surprising since 95% of genome is made up of outside of genes
		- 2.4% of SNPs are in coding regions
	2. Single SNPs have small effects
	3. causal / non-causal SNPs correlated with each other
		- If there is a single causal SNP, we will cary over *many* different non-causal SNPs due to Linkage Disequilibrium
		- There may be multiple cuasal SNPs in a region generating a complex pattern of statistical associations -> the strongest statistical association is not necessarily the causal SNPS
			- If we have two different variants in the same gene that affect the disease in different ways, (multiple causal loci)
	4. Extreme polygenicity
## GWAS result -> Schizophrenia
- After initial results, we can *zoom in* on a single locus
	- Then you can do a correlation between a location of the SNP and all the other snips, you can see LD in effect [[HC2 Genetics in neuroscience#Terminology in genetic variation|Linkage disequilibrium]]
- We can use statistical tools to model Linkage disequilibrium and find the causal SNPs
- We could also find biological mechanisms
### Strategy 1: Statistical fine-mapping (we do not need to know too much about this, but just know it exists and we can use it)
- After running GWAS we know: 
	- What the observed association pattern is
	- What SNPs are in LD within the locus
- Therefore, we can try to model what the expected association pattern would be 
	- We can take all of the SNPs in the locus and predict what it would look like if *that SNP* were to be the causal SNP -> gives us a *posterior probability* (likelihood that that is the causal SNP)
		- You can do this multiple times, and run multiple models (for if there are multiple causal SNPs -> find the best fit model) -> process of *prioritization*
### Strategy 2: Functional fine mapping
- If a SNP is causal, we can assume that it affects the phenotype by altering a gene
	- We can use this to prioritize SNPs functionally
	- Coding SNPs have a higher chance of being causal, since they directly code for genes
		- If a gene code is changed, it could affect phenotype -> we *prioritize it*
	- Non-coding can affect too if it affects transcription factors
		- If we see a non-coding SNP which affects transcription / regulatory, we could *prioritize it*
#### Functional categories of SNPs / genetic variants
- Protein coding
	- SNPs can affect protein structure / function
- Splicing regulation
	- SNPs in splice sites may disrupt splicing regulation -> exon skipping / intron retention
	- Interfere with alternative splicing -> changing splicing enhancers
- Transcriptional regulation
	- transcription factors / binding sites
	- regulatory genes can affect *many* gene regulations
- post-translational modifications
	- may alter modification sites
## Annotating SNPs in GWAS risk loci
1. Are there functional variants in the GWAS risk loci?
2. Are there SNPs with likely deletrious effects
	-  High cadd scores -> look at *CADD* score
	- Combined annotation dependent depletion
		- computational prediction of likely functional effect of sequence changes
		- Based on type of variant, properties of amino acid changes, changes for motifs
		- High cad score probably deleterious
3. Are there regulatory variants or *eQTLS*
	- *eQTLs* are identified via GWAS in which the phenotype is the expression level of certain gene in a certain tissue
		- SNPs with significant association are eQTLs
	- Repeat for all genes to form a tissue-specific eQTL database
4. are there SNPs with other likely regulatory effects?
	- Open chromatin regions -> DNase hypersensitive sites
	- If the chromatin is open DNA can be transcribed
		- DNase can only access DNA where it is open, not where closed
- Using all these techniques, you can kind of use them as 'filters' and eliminate unlikely SNPs
	- In a longer process you can find the casual SNP
		- You can also see if where your SNP is is a promoter region for another gene, which then might also be the causal gene
- *FUMA* does all of this! amazing! 

## Gene mapping: three strats
- We usually do all three, so we combine the info from all of these
### Positional mapping
- If the SNPs are physically close to gene -> more likely to be causal gene
	- If it has a *functional variant* its more likely to be the right gene
### eQTL mapping
- We can see which genes those SNPs are in eQTLs for a certain gene
	- *affect the expression for that gene*
	- Even though some genes are not mapped to genes based on positional mapping, they can still be mapped through eQTL
### Chromatin interaction mapping
- Map SNPs in a genomic region interacting with promotor regions of genes
- SNPs can be further filtered on overlap with predicted enhancers or promotor regions from roadmap
	- 
