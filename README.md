# TRGN510_Fall2020_Final_Project
- Author: Lili Xu
- Email: lilixu@usc.edu
- Date: 10/25/2020

## Overview of project:
- RNA-sequencing (RNA-seq) has become the primary technology used for gene expression profiling, with the genome-wide detection of differentially expressed genes between two or more conditions of interest one of the most commonly asked questions by researchers. The edgeR (Robinson, McCarthy, and Smyth 2010) and limma packages (Ritchie et al. 2015) available from the Bioconductor project (Huber et al. 2015) offer a well-developed suite of statistical methods for dealing with this question for RNA-seq data. This analysis is enhanced through the use of interactive graphics from the Glimma package (Su et al. 2017), that allows for a more detailed exploration of the data at both the sample and gene-level than is possible using static R plots.
- My project wants to use the bioinfomatics tool "Bioconductor" to analysis Lung cancer(TCGA-LUSC) based on the age(0-50)/(50-100).
- References/Links to Vignettes:
  - English version: https://www.bioconductor.org/packages/devel/workflows/vignettes/RNAseq123/inst/doc/limmaWorkflow.html
  - Chinese version: https://www.bioconductor.org/packages/devel/workflows/vignettes/RNAseq123/inst/doc/limmaWorkflow_CHN.html
## Data:
There will be two different age groups, young people and old people, I will download 10 datas each group from TCGA website, these datas should contain the smoke history, the reslute of Vital Status, tumor stage, and so on:
https://portal.gdc.cancer.gov/repository?cases_offset=20&facetTab=cases&filters=%7B%22op%22%3A%22and%22%2C%22content%22%3A%5B%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.demographic.gender%22%2C%22value%22%3A%5B%22female%22%2C%22male%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.disease_type%22%2C%22value%22%3A%5B%22squamous%20cell%20neoplasms%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.primary_site%22%2C%22value%22%3A%5B%22bronchus%20and%20lung%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.program.name%22%2C%22value%22%3A%5B%22TCGA%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.project_id%22%2C%22value%22%3A%5B%22TCGA-LUSC%22%5D%7D%7D%5D%7D&searchTableTab=cases
## Milestone 1
- I want to show the analysis result based on two age groups, 0-50/51-100. I will clean the data through R studio, and prepare for analysis.
## Milestone 2
- I want to generate plots of my data to detail display the RNA-seq result, like mean-variance plots, Venn diagram, Heatmap, Barcode, Interactive mean-difference plot, MDS plots and so on.
## Deliverable
- R MarkDown
