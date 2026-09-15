[README.txt](https://github.com/user-attachments/files/32239483/README.txt)
Vaginal microbiota analysis

This repository contains the R workflow that was used for analyses presented in the manuscript: 

"Vaginal microbiota composition, inflammation, and preterm birth vary by HIV status and ethnicity in a UK pregnancy cohort"

Files: 

- 16SPipeline_EthnicityHIV_CS_Longitudinal_Combined.rmd	
	- R pipeline for downstream analyses of pre-processed ASV data 	
	- Pairs the ASV file with metadata to perform analyses and create figures and tables 

- 16SPipeline_EthnicityHIV_CS_Longitudinal_Combined.html	
	- Knitted version of above R pipeline	
	- Ability to see full analyses, figures, and tables complete without running code 

- CSTData.csv	
	- CSTs identified via VALENCIA and mapped to ID that corresponds to sequence file	
	- CSTs in this file are mapped to samples in the early steps of the R file 

- Mergedfiles_EmilyEditFullASVs.csv	
	- ASV table of sequences following removal of contaminating sequences (using Decontam) 	
	- Describes the counts of bacterial species identified in each sequence 

- Timepoint1SectionMetadata_UpdatedSamples_DI.csv 	
	- Deidentified (date data removed) metadata used in cross-sectional analysis 	
	- Maps patient data to sequences in the ASV file that are used in the Timepoint 1 analyses 

- FullHIVEthnicityUKMetadata_PairedSearch_DI.csv	
	- Deidentified (date data removed) metadata used in longitudinal analysis	
	- Maps patient data to sequences in the ASV file that are used in the  longitudinal analysis (Timepoint 1 and Timepoint 2) 

Reproducing the analyses: 

1. Open the markdown file
2. Update file paths 
3. Run all code chunks or knit the document 

Outputs:

1. Participant characteristic tables
2. Alpha and beta diversity analyses and figures
3. CST composition figures and regression models
4. Cytokine analyses (including individual and PCA)
5. Longitudinal CST transition analyses and regression models 
6. All figures included in manuscript and supplementary tables
7. Differential abundance by subgroup and concerning preterm birth  

Data availability of raw sequencing files 

16S rRNA gene sequencing data are deposited in the European Nucleotide Archive (ENA) under accession number PRJEB114705  and are available at:https://www.ebi.ac.uk/ena.
