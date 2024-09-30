## How Humans Compare with Other Organisms  
1. Unlike the human's seemingly random distribution of gene-rich areas, many other organisms' genomes are more uniform, with genes evenly spaced throughout.  
2. Humans have on average three times as many kinds of proteins as the fly or worm because of mRNA transcript "alternative splicing" and chemical modifications to the proteins. This process can yield different protein products from the same gene.  
3. Humans share most of the same protein families with worms, flies, and plants; but the number of gene family members has expanded in humans, especially in proteins involved in development and immunity.  
4. The human genome has a much greater portion (50%) of repeat sequences than the mustard weed (11%), the worm (7%), and the fly (3%).
## The two principles for producing mutant mice:  
###  Transgenesis (general):  random insertion  
- DNA is injected into one of the pronuclei.
	- The oocyte is fixed in position with a holding pipette
- Transgene construct: CMV- GFP
	- CMV: a strong ubiquitous promoter from Cytomegalovirus
	- GFP: a Green Fluorescent Protein from jellyfish
		- Can make active neurons green
### Homologous recombination: targeted modification (2 ways to do that)
- Goes in a very specific direction
- Say, you have a gene of interest
	- You can knock it out of the mouse --> knock-out mouse
	- Or, you can change one amino-acid into another
		- A single amino-acid change is *almost as effective* as completely deleting it
			- *phosphorylation for example*, turns it off -> [[How proteins work#Control with phosphorylation|Control with phosphorylation]]
- You introduce cells that have a manipulation to a *blastocyst-stage embryo* (like 64 cells)
	- This way its most effective --> but why???
#### How to make a targeted manipulation in a cell
1. Homologous recombination w
	- You need a *omnipotent cell* --> not *specialized* yet.
	- You have a *gene of interest* 
		- You take a *homologous* sequence on both sides of the gene and copy it to a *targeting vector*
			- A *targeting vector* is something you make in the lab in order to replace a sequence with something you created in a lab
			- But the *gene* itself will be NEO<sup>R</sup> --> makes a cell resistant to neomicine
			- You can use this to select those cells against non-resistant cells. ![[Pasted image 20240925094552.png|300]]
2. CRISPR/Cas9
	- You take a *guide sequence* that is the opposite of the sequence that is where the gene is
	- *Cas9* protein will cut the DNA at the *cut site*
- How to replace the DNA then?
	- There is a moment when the strands are single in the cell (during division or gene expression)
		- Then, we can inject a piece of lab-made DNA containing a gene with its own promotor
			- And, it has a homologous sequence to the genome on both sides (a lot, like 20,000 sequences)
			- You need this sequence to 'glue' the DNA together with hydrogen bonds, as the new gene does NOT stick to the other side (its loose)
		- During replication, the enzyme recognizes that there is already a second strand on the DNA, and falls off --> happens on both sides.
			- If it then gets replicated again, one daughter cell has both strands with new gene, and does not --> select them with neomicine *(selectable marker)*
	- When you let them grow then, they become *embryonic stem cell colonies*
		- Stem from a single resistance cell.
		- Needs to be kept in *omnipotent stage* with chemicals
		- Then, you need to separate the Targeted ES clones and the *random integrations*
			- There are often many more random insertions than well-replaced cells.
	- Then, you deliver about 20 cells in the blastocyst. Its a miracle that it survives.
		-  *hybrid blastocyst*: ES cells from brown mouse, black mouse original parent
	- When the mouse then grows up, you can see a stripe pattern on their fur
		- If you see a lot of brown, you know that most the cells are mutants
		- If the cells contributed to the gonads, the next generation will have all cells with the knock-out gene. 
#### Conditional Knock-out using Cre
- Uses LoxP site (specific small genetic code) to 
	- When you add two of these to the *targeting vector*, you can combine a mouse in which a locus is flanked by two LoxP sites, cross it with a mouse with Cre recombinase, and a tissue specific promotor or inducible promotor. So you can knock out the gene in only a very specific area of cells, or turn it off and on at will.
- This way you can also knock out genes that are vital in early development