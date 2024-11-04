# Caenorhabditis Elegans
## What is it?
- Small model animal --> *Sydney Brenner* was the man with the vision
	- 1.5mm in length, lives in soil
- Nematode, member of the phylum Nematoda
- Feeding on microbes such as bacteria
- It is of no economic importance --> we dont eat it for example
- 959 cells exactly, of which 302 neurons
	- If it differs, you have a dead c.elegans
- Males are very rare *(.05% are male)*
	- Generate sperm, but as soon as that sperm fertilizes the females, that female will never have to be fertilized again
- 3 Day life cycle
	- Egg -> different larva stages (3 days of dev) -> adult
	- egg -> dauer larva (takes 4 months) -> larva -> adult
		- Waiting for temperatures & food supply to rize
		- You can put them into this state yourself 
			- And you can freeze them with oil and keep them forever
		- Now you can make mutants and store them to put it into the wormbase
## Why use it?
- Small, easy to maintain
- short generation time and self fertilizing
- cell lineage is constant and completely mapped
- transparent body: suitable ofr high=throughput screening methods
- simple nervous system
- sequenced genome & extensive molecular toolbox
	- https://wormbase.org
- many research results are translatable to human processes
- ethical!
## What does it look like?
![[Pasted image 20240918105200.png|500]]
## Genome
- 6 chromosomes
	- 5 autosomes and 1 X chromosome
	- 97 million base pairs --> first completed in 1998, it was the first multi-cellular genome
		- 20% of what humans have
	- 20,470 genes --> 23,000 in humans (genome is smaller, but number of genes is not lower)
		- 40% of them have human equivalents
		- humans have more base pairs that code for for example transcription factors
			- This is what creates complexity in humans
		- 40% of human genome is viral 
## Cell lineage
![[Pasted image 20240918110625.png|400]]
- *John Sulston* has meticulously figured this out for every cell
	- He found out that some of the divisions stopped and one of the daughter cells would not survive (*apoptosis*) --> **strictly regulated programmed cell death**
		- Programmed cell death was a new thing at the time
			- *Bob Horvitz* did this
		- This causes the 959 number
## Nervous system
- 302 [[neurons]]
	- All neural connections are identified
		- Synapses differ a little ofc due to use
	- Transmitter use of each neuron is known
- Basically uses all the same neurotransmitters as humans do
	- Invertebrates use a lot more *neuropeptides*
## Sophisticated behavior
- Moves forward and backward
- Responds to odors, chemicals, pheromones, temp differences (0.1C), tactile and mechanical stimuli
- Associative learning & habituation
## Genetics and genetic manipulations in C.elegans
### Forward genetics
#### 1. Random mutagenesis
- Random mutagen (EMS/TMP-UV) to generate point mutations or small deletions
- Analysis of F2 for the selected phenotypes
	- How do you do this? --> Screening a lot of animals
		- 3 day life cycle, self fertilizing hermaphrodites
	- Screen for Phenotype:
		- Behavior (unc, roller)
		- Morphology (dumpy, long)
		- Lethal (let)
		- neuronal network (EGFP)
- Mapping using visible markers and polymorphic DNA sequences
	- This is still very tedious
#### 2. Transposons
- Transposons: Discrete segment of DNA moving in the genome 
	- Encodes a transposase
	- They are the *parasites of the genome*
		- they hop around the genome and sometimes destroy genes
- Normally present in C.elegans in different copies (strain dependent)
- activated by forced expressions of transposases
- Most common: Tc1 ("Cut and paste mechanism")
- Insertional mutagenesis with Tc1 will generate mutant alleles tagged by the transposon that can be used for identifying the mutated gene. 
- 
### Reverse genetics
- You target one specific type of interest
- in vertebrates, many mothods to replace genes --> KO in mouse
- They do not work very well in invertebrates
- So, we use *Antisense RNA*
![[Pasted image 20240918115652.png|400]]
- How to interfere
	1. injection of dsRNA in gonads
	2. Soaking animals in dsRNA
	3. feeding animal with bacteria producing dsRNA
- Is a transient KO
	- works fine but not always
	- can give interesting results when full phenotype is death --> not completely activated
#### Genome-scale analysis
- The entire genome has been analyzed in this way --> automated
	- The effect of the missing of a gene has on the animal
- You can make transgenic worms that express GFP --> are fluorescent
	- The cells affected by the gene expression will glow --> for example gaba-ergic neurons