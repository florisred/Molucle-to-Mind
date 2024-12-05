# Part 1: genetic architecture & correlation
## Genetic architecture of complex traits
- Complex traits are influenced by multiple genetic variants
- Different views on how this works
	- *polygenic models*
		- Common disease, common variant *CDCV*
		- Common disease, rare variant *CDRV*
	- *Omnigenic model*
## SNP associations
- We assume SNP ---affects-->  gene ---affects--> function
- But, multiple SNPs are association with a single gene
- And, there are many genes affecting function -> you have many many loci and SNPs to worry about
- Are all associated SNPs randomly distributed or do they cluster in genes?
	- This is what you do with gene mapping (what we did last week in the practical)
	- Gene based tests (week 5)
	- IF we affect another gene, it may not lead to the same problem but again deleteriously affect the pathway's functioning

## Polygenic model
- Many common variants of small effect (or rare variants?) contribute to disease
- No single SNP is necessary or sufficient to cause disease
	- Different individuals have different alleles associated with the same phenotype
- So many SNPs contribute to one gene, and many genes contribute to 1 function
	- Which means that there is a lot of backup. Explains that if there is damage to multiple genes that contribute to the same function, a person becomes diseased. 1 gene not functioning might not be sufficient to cause disease.
- We are likely to see small effects from one SNP, because there are many SNPs deterioting one gene, damage to one gene might not be enough to eradicate function.
- Associated variants likely converge in pathways
- *Pathways themselves* are the cause of the disease -> going to talk about this next week
### CDCV vs CDRV
- CDCV -> diseases common in the population are affected by SNPs that are common within the population -> only contribute small effects. (otherwise they would have been eliminated)
- CDRV -> diseases common in the population are caused by variants that are individually rare within the population
	- Hard to identify genetically (you need huge sample sizes)
	- Might have a larger effect size, but more likely to be within single family
	- Still might be variation in the population
### Polygenic model
- Mostly additive effects of disease-associated alleles
- Liability threshold model of risk
- Cases will be those individuals that have a sufficient amount of disease-causing alleles
- Allows for environmental factors to be part of individual risk burden
## Omnigenic model
- Used to be a hot topic, not anymore
- All genes are going to be associated with a phenotype somehow
- Not completely mutually exclusive with the polygenic model
- But, assumes that there are certain core genes for a phenotype that directly affect its function
	- Within those core genes, there will be rare variants that fucks up the gene completely, but there will also be normal variations that affect the expression of those genes
		- So, core genes are most relevant to function of the disease
- Compatible with:
	- Most common variants have small effects, rare variants have large effects on disease risk
	- Most GWAS hits seem to be in no-coding regions suggesting regulatory functions
	  HWAS hits seem to spread broadly across the genome, not concentrated in genes/functions
## (measured) heritability
- What is it? ->  Proportion of trait variance between individuals that is attributable to genetic variance between individuals
- Heritability can also be calculated from DNA
- SNP-based heritability, h2SNP
- Measure (distant) relatedness between all pairs of individuals
- Genetic similarity based on proportion of alleles shared across the genome
- ![[Pasted image 20241119163615.png]]
## Polygenic influences are shared across traits
- Genetic correlation can be used to quantify the extent to which the same genes affect multiple phenotypes
- Standardized measure of genetic covariance, range -1 to +1
	- Heritability = proportion of trait variance due to genetic variation between individuals
	- Genetic covariance = proportion of trait covariance (overlap of 2 traits) due to genetic variation
## Correlation might imply causation
- Pleiotropy -> the same genetic variant affects multiple traits 
	- Use of this term is very debated
- *Vertical pleiotropy*:
	- A SNP causes 1 trait, which opens up vulnerability for another trait (depression -> anxiety)
	- SNP -> intermediate -> two different traits
- *horizontal pleiotropy*
	- SNP -> depression + SNP -> anxiety
		- Same SNP in this case
	- 1 locus has two different SNPs that then have two different trait outcomes
# Part 2: polygenic risk scores
