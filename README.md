# HCC and age
Analysis code (R/Python scripts) for the scRNA-seq, scATAC-seq and survival analyses of hepatocellular carcinoma samples in this study. The scripts build on published, mature software packages; no novel software or algorithm is distributed here.

# Description
The codes include the scRNA-seq and scATAC-seq analysis code.

# System requirements
Operating systems: tested on Linux Ubuntu 20.04 and macOS
R version 4.3.1; Python >= 3.8
No non-standard hardware is required; a normal desktop computer is sufficient.

R packages (versions as described in the manuscript)：
Seurat (V4.4.0)
DoubletFinder (V2.0.3)
harmony (V0.1.0)
inferCNV (V1.19.1)
ArchR (V1.0.1)
CytoTRACE (V0.3.3)
Slingshot (V2.7.0)
Monocle3 (V1.3.7)
survival (V3.5-8)
survminer (V0.4.9)
cmprsk (V2.2-12)
DESeq2 (V1.41.2)
GSVA
ggplot2, dplyr

Other software called by the scripts (versions as described in the manuscript)：
PISA (MGI DNBelab C Series HT scRNA-analysis software, https://github.com/MGI-tech-bioinformatics/DNBelab_C_Series_HT_scRNA-analysis-software)
d2c (V1.4.4)
STAR (used for alignment to the human genome reference GRCh38)
featureCounts (V2.0.8)
MACS2 (V2.2.7.1)
CellPhoneDB
PAGA

Installation
Install R (4.3.1) from CRAN and Python (>= 3.8).
R packages from CRAN: install.packages(c("Seurat", "DoubletFinder", "harmony", "survival", "survminer", "cmprsk", "ggplot2", "dplyr"))
R packages from Bioconductor: BiocManager::install(c("DESeq2", "GSVA", "inferCNV", "Slingshot"))
R packages from GitHub: devtools::install_github("GreenleafLab/ArchR"); devtools::install_github("cole-trapnell-lab/monocle3")
Python packages: pip install MACS2==2.2.7.1; pip install cellphonedb
Typical install time: approximately 30–60 minutes on a normal desktop computer.

# Instructions for use
Scripts are organized by analysis module: scRNA-seq analysis (Seurat, harmony, DoubletFinder, inferCNV), scATAC-seq analysis (ArchR, MACS2), trajectory inference (CytoTRACE, Slingshot, Monocle3, PAGA), cell-cell communication (CellPhoneDB), and survival analysis (survival, survminer, cmprsk).
The main analyses can be reproduced using the scripts in this repository together with the processed data matrices described in the manuscript.

# Contact
Any question please contact him1996@163.com (Huang Miao)

Copyright (C) 2025 Zhou Lab
