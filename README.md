# pa-sputum-transcriptome

### Introduction

The goal of this research project was to identify transcriptomic signatures – individual genes, biological pathways (KEGG, GO terms), and correlated gene sets – that define the behavior of P. aeruginosa in real CF sputum (i.e., expectorated sputum from the lungs of donors with cystic fibrosis or CF). Sputum is simply mucus that settles in the airways during infection, serving as a habitat and nutrient source for bacteria like Pseudomonas. 

In the laboratory setting, P. aeruginosa is often studied in different forms of laboratory culture. Certain media, like the common LB broth, are not designed to mimic the characteristics of sputum to which P. aeruginosa is exposed in the lung. Other media – like artificial sputum media (ASM) – are specifically designed to mimic CF sputum.  However, even when studied in ASM, the biological behavior of P. aeruginosa does not completely mimic its behavior in real CF sputum. 

In this study, we sought to quantify the transcriptomic differences between P. aeruginosa growth in real CF sputum versus ASM and identify candidate biological factors that exist in the CF lung that drive the observed transcriptomic differences. Researchers can take the observed signatures into account when interpreting their experimental results, and even choose to supplement their laboratory media with biological factors (e.g., divalent metals) that better recapitulate the conditions of the CF lung. 

In this repository, we have made available our source code and data. The whole suite of transcriptomic signatures identified are available as a resource and stimulant for future study. In the associated paper [see reference below], we emphasize the role of metal availability in defining the P. aeruginosa transcriptomic profile in the CF lung, and focus most of our attention on gene sets related to metal acquisition. Other researchers may be interested in different gene sets and can use the code and data presented here as a starting point for their own follow-up experiments.  

### Directory Contents

**Figure Production Code**

- Figure Production.Rmd: R markdown file containing all the analysis code – including the definition of transcriptomic signatures featured in the paper, the performance of differential gene expression analysis, and the production of figures and tables, both primary and supplemental.
- Data_Files: Folder containing the necessary raw data to run the Figure Production.Rmd script successfully. This includes the raw count data for all the samples described in the paper, the concentrations of metals in the samples, the correlated gene sets identified by ADAGE, and gene ID mappings for P. aeruginosa (P. aeruginosa gene locus ID – Uniprot ID – gene function – GO terms)
- Paper Analysis.Rproj: The R project file associated with the code and data files. If running the code on your own personal computer, it is easiest to download Figure Production.Rmd, the Data_Files folder, and Paper Analysis.Rproj into the same directory. Simply clicking the Paper Analysis.Rproj file will open a session where the script has access to the data files and no re-arrangement of files is necessary.

**Primary Tables**

- This folder contains primary tables 2 and 3 from the manuscript. Table 1 is a donor metadata table that was small enough to be included within the paper itself. 

**Supplementary Material**

- This folder contains all the supplementary tables (S1-S5) and the document of supplementary figures (S1-S8) featured in the manuscript.

**Processing Sputum RNASeq**

- This folder contains the necessary scripts for processing the RNA-seq count data and generating a raw count table with Salmon.
- This folder contains its own README file with additional information about how these scripts work together.
- The raw data was made publicly available in a database as described in the data availability statement of the associated manuscript. The count table is present in the Data_Files folder within the Figure Production Code directory of this repository. 

### Requirements

To run the code featured in this directory, you should download all contents of the repository by clicking the green ‘Code’ button at top right and selecting ‘Download ZIP’

Once the repository files are downloaded, you will need R and Rstudio installed on your computer (preferably the latest versions of both). The code file itself includes the necessary packages to be installed in R. 

### Reference

If you use the contents of this repository to advance your own research, please cite the following publication:

*Placeholder: Reference will be available as soon as the associated manuscript is submitted.*

If you have any questions about the contents of this directory, please reach out to neff [dot] sam1 [at] gmail [dot] com
