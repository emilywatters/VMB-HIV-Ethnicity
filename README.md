# VMB-HIV-Ethnicity

Vaginal microbiota analysis

This repository contains the R workflow that was used for analyses presented in the manuscript: 

"The vaginal microbiota varies by self-identified ethnicity and HIV status throughout pregnancy and relates to preterm birth risk in a United Kingdom observational cohort"

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
	- ASV table of sequences following removal of contaminating sequences  	
	- Describes the counts of bacterial species identified in each sequence 

- HIVEthnicityUKMetadata_CS_DI.csv 	
	- Deidentified (date data removed) metadata used in cross-sectional analysis 	
	- Maps patient data to sequences in the ASV file that are used in the trimester 2 cross-sectional analysis
	- Includes column that maps patient IDs/data to FASTQ files and specific ENA ID  

- HIVEthnicityUKMetadata_Longitudinal_DI.csv	
	- Deidentified (date data removed) metadata used in longitudinal analysis	
	- Maps patient data to sequences in the ASV file that are used in the  longitudinal analysis 
	- Includes column that maps patient IDs/data to FASTQ files and specific ENA ID 

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

16S rRNA gene sequencing data are deposited in the European Nucleotide Archive (ENA) under accession number PRJEB114705  and are available at: https://www.ebi.ac.uk/ena
