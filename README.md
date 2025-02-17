```                                                                                                   
╔═══╗────────╔═══╗─────╔╗────────╔═══╗
╚╗╔╗║────────╚╗╔╗║─────║║────────╚╗╔╗║
─║║║╠══╦══╦══╗║║║╠══╦══╣║╔╦╦═╗╔══╗║║║╠══╦═╦══╗
─║║║║║═╣║═╣╔╗║║║║║╔╗║╔═╣╚╝╬╣╔╗╣╔╗║║║║║╔╗║╔╣║═╣
╔╝╚╝║║═╣║═╣╚╝╠╝╚╝║╚╝║╚═╣╔╗╣║║║║╚╝╠╝╚╝║╔╗║║║║═╣
╚═══╩══╩══╣╔═╩═══╩══╩══╩╝╚╩╩╝╚╩═╗╠═══╩╝╚╩╝╚══╝
──────────║║──────────────────╔═╝║
──────────╚╝──────────────────╚══╝
```

The **DeepDockingDare** (**DDD**) data set has been compiled as a scientific collaboration between the University of Copenhagen (Data Science for Drug Design lab headed by Albert J. Kooistra) and Structure Therapeutics (Dr. Chris de Graaf and colleagues) to evaluate co-folding and deep learning docking methods for their ability to predict:
*Small molecule binding modes in diverse protein systems for Structure-Based Drug Discovery (SBDD)*

Criteria for the preparation of the DDD data set are:

**1)** Minimise data leakage with respect to training sets of current state-of-the-art co-folding methods, considering the following three prediction scenarios:

* Novel protein subset (229 entries)*
	- There are no PDB entries (with resolution <5.0 Angstrom) in PDB Sequence Clusters of 70% or higher that have been released in the Protein Databank (PDB) before January 2021.


* Novel modality subset (82 entries)*
	- There are no PDB entries in PDB Sequence Clusters of 70% or higher that have been released in the Protein Databank (PDB) before January 2021, that are bound to the same modality.
Distinction is made between the following modalities:
	- Agonist,  Antagonist, Negative Allosteric Modulator, Positive Allosteric Modulator
	- Inhibitor, Activator, Negative Allosteric Modulator, Positive Allosteric Modulator
	- Peptide ligand, small molecule ligand (distinct from co-factor)


* Novel binding site subset (39 entries) *
	- There are no PDB entries in PDB Sequence Clusters of 70% or higher that have been released in the Protein Databank (PDB) before January 2021, where the ligand is bound to the same binding site.



**2)** Therapeutically relevant protein targets
- Human or mammalian protein targets
-  Antibiotic proteins targets

**3)** Drug-like molecules
- Exclude e.g. nucleotides (e.g. AMP, ADP, ATP, GDP, GTP), flavinoids (e.g. FMN), sugars (e.g. maltose), steroids (e.g. cholesterol)
- Drug-like properties

**4)** Structure resolution (with focus on small molecule ligand binding mode)
- Resolution <3.1 Angstrom
- Small molecule ligand fits electron density map

____________________________

This DDD repository contains:

1) The annotated and parsed DDD data set

2) Soon: all results of different co-folding methods, including:

* AlphaFold3
* Boltz-1
* Chai-1
* HelixFold3
* Protenix
