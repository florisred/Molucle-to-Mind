## Case mr. V
- 57 yo male
- focal epileptic seiures
	- coordination problems in right arm
	- Word finding difficulties
	- Poor verbal memory, including encoding
	- Slow information processing
	- Poor executive functioning
	- Personality changes for >1 year in retrospect
		- Disinhibition
- Giant white spot in the right half of the brain, indicates BBB broken
- Mass effect: tissue squished around the tumor
- In the middle of the tumor: Black: necrosis (dead tissue)
## Case mrs. M.
- 60 yo female
- Generalized seizure
- Other symptoms:
	- No deficits on neuropsychological assessment
	- severe personality changes
	- anosognosia
- MRI: 
	- Dark center, more active white ring (ring enhancement)
	- Mass effect
	- Looks like neoblastoma
- Anosognosia: Does not realize that she has the disease
	- almost makes it more severe, so size of tumor does not matter
	- Location of tumor does not explain symptoms fully, very unpredictable what will happen to patients

## Current standard: MRI
- Pre-contrast T1 -> best see anatomy
- Post-contrast T1 -> best see inflammation / BBB being broken  (gadoliminium injection)
- Post contrast T2 -> Makes it easier to see tumor itself
## Meningioma
- Mostly grade I
	- Grow from the meninges (not primary)
		- Not infiltrating the tissue of the brain itself
		- More common than Gliomas
## Gliomas -> most important from this lecture
### Low grade glioma
- Grow from glial cells
- Called low-grade glioma (grade II)
	- Or astrocytoma and oligodendroglioma grade II
	- Large tumor with ill-defined boudnaries on T1, no or very little contrast enhancement
		- There are (semi) normal brain cells still functioning 
	- Can look weird on CT
### High grade glioma
- Grade III
- Not a full ring, more patchy
- You cannot really discern astrocytoma from oligodendroglioma
	- Oligodrendroglioma grows slower, but gives brain more time to adapt -> appears bigger when found
- Glioblastoma Fultiforme (grade IV)
	- Righ shaped contrast enhancement, central necrosis, edema, mass effects, midline shifts
## PET
- Can see parts of body that are more glucose-hungry
	- So, Great for visualizing tumors?
		- Sometimes, but the brain is a very hungry organ so it does not show that well
## Diagnosis of neuro-oncological tumors
- Before 2016: only histopathology --> immunohistochemistry from sample
- As of 2016: Xombinoation of histopathology and molecular markers
### Histopathological era
- Still being used today (even in papers)
- Classifications made by WHO
	- Who grade 1: (ecluded)
	- WHO grade II (astrocytoma, oligodendroglkoma, oligoastrocytoma)
## Combined histopatho/molecular leval
![[Pasted image 20241209140707.png]]
- Oligodendroglioma: best prognosis
- Glioblastoma: Worst prognosis
## Treatment options
- **Wait & scan**:
	- Not really done anymore, only done if it is in a brain area will immediately kill somone
	- Only if resection not possible
- **Surgery**
	- Almost the best option if it is possible
	- Correlates with survival
	- Complete resection is NOT possible
	- Tumors grow infiltratively, the "ball" on the MRI is not everything
	- Many cells outside of main tumor, so it will always come back
	- Dual optimization:
		- Resect as much of tumor as possible
		- Keep functional areas intact
			- Done by awake craniotomy 
			- Brain does not have pain sensors
			- Patients are very able to communicate and undergo this treatment
			- First gives a little shock to a certain place which gives transient paralysis
				- See if anything goes wrong, if not, cut it out!
			- After 2 hours, patients are done (because it is so tiring)
			- 
- **Chemotherapy**
	- Very difficult to get medicine into brain
	- Temozolomide (primary treatment
		- Alkylating agent
		- Binds methyl (CH3) group to DNA, DNA breaks
		- Induces cell loss
	- Works particularly well in IDH-mut
	- PCV (combination therapy)
		- Only given if tumor stops reacting to temozolomide
- **Radiotherapy**
	- Beam moves around the tumor and brain 
	- By angling the beam toward the tumor you kill the tumor
	- But still radiation going into the brain
	- Radiotherapy only given with a limited fraction dose
		- Limited number of rays per session and in total
		- Only given once
	- Proton radiotherapy is more limited harm
	- Thing to remember for radiotherapy:
		- Can be cognitive deficits very delayed
		- Between 12-26 years after they could still be declining
- **Combination, particularly in GBM** (most often used)
	- Glioblastoma
	- First get a resection
	- 6 weeks of TMZ / RT
	- Short break
	- Another 6 months of TMZ
- Standard treatment (takes 9 months in total)
- Big difference in number of people still alive after 30 months
## Optune -> most clinical trails have stopped
- Tumor Treating Fields
- Blocks cell division with fields
- Seems to work better with TMZ + TTF than just TMZ
## Very promising new treatment for IDH mutant gliomas
- Vorasidenib 
- Dual inhibitor of the mutant IDH1 and IDH2 enzymes
- Survival benefit is huge
- Thing to remember: 
	- Mensen hebben pauze nodig
## Side effects of treatment
- Neurologicla deficits
- Cognitive dysfunction
- Reduced quality of life
## Graph theoretical concepts II
- Graph theory can help us with how tumors result in symptoms
- Most things are a network
	- Networks are a collection of Nodes (edges and vertices)
	- Different patterns of connections
- We can describe networks in different ways:
	- Weighted / unweighted (edges have a number)
	- Directionality
- Use for analysis:
	- Matrix annotation
- Measures:
	- Integration: How one node is in a whole network
	- Hubness: how much a node serves as a hub
## Overview of connectomics
- Diffusion MRI
	- Yields a matrix / probability of white matter tracts
	- More like a road
- rs-fMRI
	- Correlation between time series
	- more like a bike
		- no idea what that means
- EEG / MEG
	- Measure brain activity in a much more direct manner
### Global connectome relates to IQ
- Small-world network seems to be the best of both worlds
## Glioma and the connectome
- Patient network looks different very different everywhere
### Network disease: Symptoms
- There is a high level of *local clustering*
	- Disturbance in local clustering throughout the entire brain
	- Higher seizure vulnerability
	- Increased clustering and longer path length relate to cognitive deficits
## Glioma locations:
- Tumors never appear in the occipital lobe
- Mostly in the frontal and parietal lobes
- Premorbid regional profile is relevant
	- Intrinsic connectome based on large cohorts of healthy subjects
	- Then extracted connections at tumor locations
	- Tumors appear in highly active and highly clustered areas with a lot of local connections 