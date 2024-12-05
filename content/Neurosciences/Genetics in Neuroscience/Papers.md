## Schwabe 2019 -> unraveling genetic architecture
- Two strategies to increase number of genetic risk loci in MDD
	1. Maximize sample size by combining more sources
	2. Reduce phenotypic heterogeneity by by selecting homogenous subtypes
- Both are essential for further research
- Higher sample size has worked so far
	- However, some of the loci found are from general internalizing disorders, so not for MDD
	- More phenotypic data needed to link genes to specific subtypes
## Uffelman 2020
### Available resources to assess the potential impact of genetic vriants on gene function
- Two ways SNPs might cause disease:
	1. SNP in coding region causes genetic defect in genes
	2. Genetic variant may affect expression level of a gene (eQTLs or chromatin structure)
### positional mapping
- Check in a database (like ENCODE) which genes do what, so we can see if there is biological plausibility for a SNP
- This way, we can see if a coding-SNP is likely to result in a disease
### Transcriptional landscapes
- Uses eQTLs
	- cis-eQTLs: nearby genes, <1mb away (larger effects)
	- trans-eQTLs: far away genes, >5mb
- Gene expression is a stochastic, time-bound phenomenon
	- We need more eQTL studies across time
### Epigenomic landscapes
- eQTL cannot tell us how regulation of expression works (eQTLs), and using epigenomic landscapes can mitigate this
### Pinpointing the most likely variant
- *Functional annotation:* FUMA
- Cannot be done willy-nilly: SNP association is likely affected by LD
- *Statistical fine-mapping*: looking at nearby SNP association patterns and leveraging what we know about LD to pinpoint causal SNP
### Gene to function: looking for convergence
- Looking for convergence along associated/causal variants can pinpoint *which biological mechanism* a disease might be caused by
#### Tools for looking for convergence
- *Gene Set Analysis*
	- Self-contained: See if the genes in the gene-set are significantly associated with trait
		- Higher background heritability causes spurious positives
	- competitive: see if the genes in the gene-set are more associated with trait than genes not in the gene set
- Most widely used tools: LDSC and MAGMA
- Statistical power *decreases* as heritability increases
- Conditional GSA testing addresses gene-set interaction, and sub- and supersets
### Challenges with neuropsychiatric disorders
- few eQTL studies have done extensive research on brain gene expression
- Even if they did, GWAS only allows us to select pathways SNPs converge on, actually applying this info to aid people is going to be hard
- Neuropsychiatric disorders show a lot of overlap between each other, making specific conclusions hard

## Tam, 2019: Benefits and limitations of GWAS
### Benefits
- GWAS have been very successful in identifying novel variant-trait associations
- GWAS can lead to the discovery of novel biological mechanisms
	- GWAS -> loci -> genes -> biological mechanism
- GWAS findings have diverse clinical applications
	- GWAS have identified genetic variants that can be used to inform drug selection and dosage and prevent adverse drug reactions
- GWAS can provide insight into ethnic variation of complex traits
- 