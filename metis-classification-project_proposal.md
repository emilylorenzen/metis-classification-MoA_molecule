Metis Bootcamp - Classification Project Proposal
Emily Lorenzen
06/03/2021

# Predict the protein family targeted by a ligand 

## **Question/Need:**
Cellular signaling is driven by ligand binding to receptor proteins, and is instrumental to all aspects of human physiology. Ligands can be naturally occurring or synthetic, have huge range of properties and consequences. Since ligands are the basis for pharmaceuticals, screening them for desired effects and properties is instrumental. Ligand screens are often performed by high-throughput bioassays, which are tedious, expensive and time-consuming. By reducing the number of ligands in a screen, researchers and biotech companies can reduce the time and money needed to find potential new therapeutics.

In this proposal, I will focus on creating a model that can predict whether a ligand will bind to a g protein-coupled receptor (GPCR). To date, GPCRs have been the most pharmaceutically exploited family of proteins. Thus, ligands that might target GPCRs are of great interest in pharmaceutical development. 

 
## **Data:**
I will use the following databases to obtain the specified features: 

IUPHAR/Guide to Pharmacology interaction database - includes a list of ligands and their protein targets 

Uniprot database, peptide ligand search - post-translation modifications, molecular mass

Uniprot database, target search - target superfamily 

Human protein atlas, peptide ligand search - tissue specificity, single cell specificity, blood specificity, brain specificity, predicted location, extracellular location

Pubchem, ligand search - chemical and physical properties (molecular weight, XLogP3, hydrogen bond donor count, hydrogen bond acceptor count, rotatable bond count, topological polar surface, heavy atom count, formal charge, complexity, isotope atom count, define atom sterocenter count, undefined atom stereocenter count, )

One unit of data will be the peptide ligand and the features described above. 

## **Tools**
Pubmed API - grabbing data
Biopython or another package - structural bioinformatics 
Pandas - data cleaning and exploratory data analysis
Sklearn - modeling
Matplotlib/Seaborn - visualization

## **Minimal Viable Product**
For the MVP I will initially use 3 features to create a classification model and evaluate the model. Since the target variable is not numerical,  I will use a random forest model. The features I will initially examine will be based on the correlation coefficients calculated during 
