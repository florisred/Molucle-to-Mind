## Why do we do the simple UNIX code?
- We have to have some skills to work with the cluster computer (which has to use UNIX) in order to do the analysis later on
	- We have to know how to look through the filesystem, make a file, edit or remove a file, etc
	- We DONT need to know everything by hard completely, be assured. 
## What do we need to know from the literature?
- Not every detail, not every gene, don't worry about that
- Just know the *main concepts* and the takeaway messages from them
- It is there to provide *repetition, repetition, repetition*

# Background in genetic variation
## Genetic studies in neuroscience
- Typically aim to identify the disease genes / mutations
	- Basically already resolved for monogenic disorders
	- The majority of neuropsychiatric disorders are *polygenic*
- Studies now aim to *identify genetic influences* on normative traits
	- Is important to get grants lol
	- Often as a means to understand related disorders (*liability threshold model*)
		- A novel / widespread idea within genetics:
			- The diagnosis of diseases is not necessarily *qualitatively different* from normal sadness, but some people have a *genetically higher risk* that lead to clinical 
			- It's like a normal distribution (for example of sadness), where certain genes give individuals a *higher* *propensity* to develop clinical depression, but this is still within the same distribution
- Why do we want to use DNA for this?
	- You can use *DNA* to learn about the *underlying biological processes* 
	- Could be useful for treatment
## What are the goals of disease genetics?
- DFor a given disorder we would like to 
	1. *Predict* if someone will sick
		- Since DNA is fixed at birth, we can attribute *causal roles*
	2. *Test hypotheses* about *relationships to other diseases* and traits
		- *Pleiotropic* (multiple phenotypes) genes 
	3. If we u*nderstand the DNA and how it contributes to downstream processes*, we could better treat those processes
		- Until now it has mostly been guesswork with regards to drug treatment (we dont know why they work), but with actual disease mechanisms we could better achieve these goals
### Genetic variation is fundamental to these goals
- DNA differences between individuals contribute to phenotype differences between individuals
- With twin studies, we cannot really see this
## Terminology in genetic variation
- SNP -> *single nucleotide polymorphism (variant)*
	- If there is variation on one single nucleotide in the genetic pool, it is called a *SNP*
- Allele -> *which version of the polymorphism an individual has* 
	- Usually 2 alleles per locus (we have two copies right)
- Genotype -> *the alleles that a person has for that particular SNP*
	- Lots of genotypes throughout your genome
	- Sometimes these are independent of each other, but
- Linkage Disequilibrium -> *Not independent!*
	-  *recombination* does not look at SNPs, but is random. So physically close SNPs will be inherited together
- Haplotype
	- Of you know one allele of two with Linkage disequilibrium, you will be able to predict the SNPs one has. -> is one type, called a *haplotype*
	- always *population* and *family* specific 
	- Are *probabilistic* -> to infer missing genotype information
- There is a useful slide on *slide 12* of the presentation, which shows clearly what a SNP is, how they contribute to *alleles*, and genotypes, and how they make up a *haplotype* (a single SNP always goes with another SNP)
	- While we actually have 4 types of alleles (we have two double-stranded chromosomes) this makes it more complicated than necessary (since the complementary base pair can alwyas be inferred) -> we only really use 2. 
## Structure of genes in DNA
- Specific sets of 3 bases ([[From RNA to Protein#Codons|codons]]) provide the blueprint for 1 amino acid.
	- Since there are more than one codons for an amino acid, it is *partially redundant*
		- If a mutation keeps coding for the same amino acid (due to the redundancy), it does not necessarily mean that it has no effect
			- DNA does *more than just code amino acids* -> binds transcription factors, or does more -> can still have an effect!!
- If an SNP has a detrimental effect, or any effect, that allele might contribute to a different genotype
## Types of genetic variation
- Monomorphic sites -> not relevant
- SNPs -> most frequent, GWAS variants
- Insertion, deletion 
- Copy number variants
- Inversion
## Genetic variation within a typical human

| Variant Category                  | Common (Frequency > 2,500) | Rare (Frequency < 2,500) |
| --------------------------------- | -------------------------- | ------------------------ |
| **Nonsynonymous (coding region)** | > 2,500                    | 130                      |
| **Predicted to be damaging**      | 20–40                      | 2–5                      |
| **Loss of function**              | 150                        | 10–20                    |
| **Cancer causing**                | 0                          | 1–2                      |
| **Copy Number Variations (CNVs)** | 0                          | > 70 (some common)       |

## Measuring genetic variant associations
- twin studies have found that most traits are consistent with a model where all genetic variance is *additive*
	- One allele increases or decreases risk relative to the other allele
	- Each copy of the risk allele increases trait linearly -> could be seen as a regression model
## Linkage disequilibrium induces associations with non-causdal SNPs
- If a mutation occurs, it is going to passed along with other alleles that share the same linkage disequilibrium
	- It begins perfectly correlated with all alleles on a chromosomes (one individual)
		- As more offspring exists, recombination will occur and the haplotype block will get smaller (chopped up), causing fewer alleles to be associated with each other 
	- As more offspring causes recombination to separate causal from non-causal alleles, the number of non-causal alleles *decreases*
		- **Non-causal changes** are genetic variations that do not have a direct effect on the trait or outcome. These might be changes that are simply associated with causal variants (often because of linkage disequilibrium) but do not independently influence the trait.
		- **Causal changes** are genetic variations that directly contribute to or cause a particular effect or trait. For instance, if a specific genetic variant increases susceptibility to a disease, this variant would be considered causal.
### Linkage disequilibrium can be levaraged
- While it can hamper research -> we might not know which changes are causal and which aren't
- But, Since there is a limited number of chromosomal combinations, we can sequence fewer parts of the genes and infer there rest
# GWAS
## What do we do with GWAS?
- Main goal: Finding statistical associations of base pair differences 
## Collection of DNA and phenotypic information
### Research cohorts: Biobanks
- For example, UK Biobank
	- 500,000 people
	- Genetic and phenotypic data
		- Physical measures, MRI, health records, etc
	- aged between 40 and 69
	- Database regularly augmented with additional data
	- Globally accessible to approved researches
- Ancestral composition of GWAS studies
	- right now we have a large bias towards european ancestry
	- Initially we thought this would not be a big problem, but LD causes ancestral gropus to have different LD patterns
	- Therefore, haplotypes might differ still. 
		- Causes problems for disease prediction
		- But, since haplotype blocks are smaller and older between old ancestral populations we can use narrow down the window to find the causal variant
			- *older ancestral groups* have been having children in the same population group for a long time -> africa is oldest
				- Therefore, the haplotype is smaller (more recombination) 
### microarrays
- GWAS genotyping arrays use correlational nature of our genome to selectively genotype most informative SNPs
- Genotypes of these 'most informative SNP' also captures information of ungenotyped SNP with which they correlate thanks to linkage disequilibrium
	- Costs are lowered by not genotyping all SNPs
- Recent new techniques allow very low cost *WES* (whole exome sequencing) or *WGS* Whole genome sequencing 
- How it works
	- You first collect your DNA, extract and store it
	- Then you denature the DNA and make it single stranded
	- Fragment it -> have lots little pieces
		- Makes it possible to have a higher throughput
	- Including a fluorescent light probe you can then see which genotype you have
		- On 30 base pairs where you know there is a polymorphism
			- DNA itself is randomly cut, but you have the correct sequences on the microarray so they stick
		- Im sorry for not explaining well i think its very hard lol
- About 30 euros per sample
- Good quality control and analysis
- Can only capture known mutation
- Imputation gives good coverage of the genome
- Some regions are difficult to genotype
### Sequencing
- About 1,000 euros per sample
- Gives a lot (too much) data
	- Harder to quality control
- 
#### Whole genome sequencing
- allows to detect completely new 
- You can only read small sequences at once, so you dont know the order
	- We have to do mapping to map it to the reference genome, which is not perfect
		- If you have repetitive sequences it is very hard to map
#### Whole exome sequencing
- You just target the coding regions, same process as WGS, but you include a little capture phase that uses *antibodies* to grab most relevant DNA sequences
- 