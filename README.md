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
There will be two different race group(white vs. Black), and I also want to look at sexual distribution(female vs.Male), I will download 10 data each group from TCGA website, these datas should contain the smoke history, the reslute of Vital Status, tumor stage, and so on:
https://portal.gdc.cancer.gov/repository?cases_offset=20&facetTab=cases&filters=%7B%22op%22%3A%22and%22%2C%22content%22%3A%5B%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.demographic.gender%22%2C%22value%22%3A%5B%22female%22%2C%22male%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.disease_type%22%2C%22value%22%3A%5B%22squamous%20cell%20neoplasms%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.primary_site%22%2C%22value%22%3A%5B%22bronchus%20and%20lung%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.program.name%22%2C%22value%22%3A%5B%22TCGA%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.project_id%22%2C%22value%22%3A%5B%22TCGA-LUSC%22%5D%7D%7D%5D%7D&searchTableTab=cases

## Milestone 1
•	Firstly, I downloaded 20 HTseq data from TCGA website. Then, I made a DGEList that combine 20 files to a matrix of counts, Use this DGEList, I got the geneName and geneId from Homo.sapines pacakage base on the ENSEMBL. Moreover, I transformed raw counts to CPM and log-CPM values and removed the low expressed gene. Finally, I normalised the gene expression distributions and draw a MSD plot base on these counts.
   
     Update 11/3/20: complete milestone1 on time, and upload milestone 1.

## Milestone 2
•	For milestone 2, I get the code at the beginning and run the code, but I find the group and lane variables cannot show me the right result. So I change the group varibles from age to race, and add sexual lane. However, the up and down table cannot get the correct values, so I download more data from TCGA website. At the end, maybe the result is not very clear, but I learn lots of analysis method in this project.
    
     Update 11/12/20: adding more data, and complete milestone2 on time, change R markdown to R notebook, and get the html link.

## Deliverable
• R MarkDown
• R NoteBook
