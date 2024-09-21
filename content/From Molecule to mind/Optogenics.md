## Why optogenics?
- You want to to study the brain and different parts and function *without* destroying it
	- Especially causal information --> When this area / neuron is active, this happens
- A causal understanding can be gotten by seeing if a certain area is necessary & sufficient to give rise to a certain behavior
	- Usually, to do this you do an intervention and see behavior
		- For *necessary*: disable and see if its not there
		- for *sufficient*: stimulate and see if behavior is displayed
- traditional ways of doing this:
### Traditional ways of understanding cause and effect
- *Limitations*:
	- cell-specificity
	- temporal resolution
	- reversibility
		- Some do permanent damage
	- firing frequencies
#### 1. Lesions
- *Mechanical lesion*
	- Due to lesions (especially from the war), see what area is damaged and function is impaired
- *Chemical lesion*
	- Animal models, you kill a certain brain area with chemicals and see how it affects the animal --> often for memory function --> this is fucking cruel but sure
#### 2. Pharmacology
- You can stimulate or inhibit a certain area of the brain with drugs
	- Receptor agonists / antagonists
#### 3. Deep brain stimulation
- Temporary intervention 
- Can both silence / stimulate function in the brain
- so both for *necessary* and *sufficient* causal effect studies
#### 4. Genetic
- This one speaks for itself
#### Optogenetics
- This solves all of the limitations discussed earlier
	- Has a high temporal resolution --> uses light to activate / silence neurons
	- Reversible, act at time scale of [[Action potentials]] --> can intervene really well!
## How does optogenics work?
- Using *naturally occurring light-sensitive ion channels and pumps
	- almost exactly like *rhodopsin*, the protein in our eyes
- These mostly come from bacteria or algae in salt lakes, freshwater lake, or soda lakes.
	- Green light: *bacteriorhodopsin* from a salt lak
	- Blue light: *channelrhodopsin* from freshwater lake
		- Gives rise to action potentials
	- yellow light: *halorhodopsin* from soda laker
		- Cl- channel, silences neuron
- When these are put in the genes of neurons, you can turn them on and off willy nilly
- We can now do way more than this, even [[g-protein]] light sensitivity
## Virus-mediated transfection
- *AAV* - adeno associated virus, *Lenti virus*, or other ones
- We put genetic material in to the virus, so when it enters a cell it will express the genes
- We can use this method from birth to adulthood 
	- Depending on specificity you do it later or earlier (earlier is less specific but more universal brain coverage)
- We inject very little so immune system does not react
## How to make optogenics cell-specific
- make use of promotors such as *CAMK2* which is used by only excitatory neurons in the forebrain
- Promoter controls expression of *Cre-recombinase* --> [[Neural systems#Conditional mutations, Cre/Lox system|cre/lox system]]
	- *Cre-recombinase* is a protein cutting DNA normally only in bacteria
		- Is used here to flip direction of DNA which allows channelrhodopsin to be expressed
		- Probably will be discussed more later!
	- EYFP protein --> yellow fluorescent dye to see which cells have the particular gene expression
## How to generate light in the brain
- Chronic implantation of optic fiber (100-200 µm core) in brain region of interest
	- Optic fibers connected to led light in the brain
