# Bulk-RNAseq-Project
Bulk RNA-seq differential expression analysis pipeline using edgeR in R. Includes TMM normalization, QL GLM statistical testing, and visualization.

## Authors:
Giacomo Pogliana

## Overview
This R-based bioinformatics pipeline is designed to process bulk RNA-seq count data for differential gene expression analysis. It automates data preprocessing, filtering of low-expressed genes, Trimmed Mean of M-values (TMM) normalization, dispersion estimation, statistical testing using Quasi-Likelihood Negative Binomial GLMs, and functional visualization (e.g., Volcano plots, Heatmaps, and MDS/PCA plots).

## Prerequisites & Dependencies
To run this pipeline, ensure R (version >= 4.0) is installed along with the following packages:
- **R** (>= 4.0)

- **edgeR** (Differential expression analysis)

- **limma** (Linear models and RNA-seq normalization utilities)

- **ComplexHeatmap** (Hierarchical clustering and heatmaps)

- **EnhancedVolcano** (Publication-ready volcano plots)

- **ggplot2 & pheatmap** (Data visualization)

- **dplyr & tidyr** (Data manipulation and tidying)

- **rmarkdown & knitr** (HTML report generation)

Install dependencies in R using `BiocManager`:
```R
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install(c("edgeR", "limma", "ComplexHeatmap", "EnhancedVolcano", "ggplot2", "dplyr", "rmarkdown"))
