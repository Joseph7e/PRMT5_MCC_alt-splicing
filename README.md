# PRMT5_MCC_alt-splicing  

This repository contains scripts related to the manuscript:  
**"PRMT5-dependent SRSF1 modification drives Tip60-EP400 complex oncogenic activity through exon inclusion."**  

## Overview  
This repository includes scripts for analyzing **PRMT5-driven alternative splicing** in **Merkel cell carcinoma (MCC)**. The analyses focus on:  
- Illumina short-read RNA-seq data and PacBio long-read HiFi IsoSeq3 processing and quantification  
- Identification of PRMT5-dependent splicing events
- Construction of summary tables
- Data visualization and figure generation  

### **General Requirements**  
- **Operating System:** Linux / macOS  
- **Programming Languages:** Python (>=3.8), R (>=4.0)

### **Contact**
For questions of issues, please open an issue or contact joseph.sevigny@unh.edu


### **Description of Files**
 - 'pacbio-commands.txt' - a simple README file with the PACBIO isoseq workflow. This provides the BASH commands to create the read counts and isoform classifications starting from multiplexed PacBio HiFi reads.
 - 'GSEA-plots.ipynb' - generates enrichment plots for GSEA analysis. Used for construction of Figure 2C. The input dataset is a CSV of GSEA results which includes fields for FDR q-val and NOM p-val.
 - 'isoform-plots.ipynb' - generates Figures 3A, 3B and Figures EV4. The input to the script is a TSV file of the classifications produced by the pigeon report software.
 - 'saturation-curve.ipynb' - generates a saturation curve for isoseq data. The input file is generated using the pigeon report function. This provides a TSV with the number of reads and identified genes/transcripts.
