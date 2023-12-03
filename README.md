# CF-ETI-scRNA
Cell-hashing Single-cell RNA sequencing Data Analysis Pipeline

Author: Anson Wong, Hieu Nim, Mirana Ramialison

## Description
Computational analyses of single-cell RNA-seq data from bronchoalveolar lavage (BAL) of preschool cystic fibrosis receiving Elexacaftor-Texacaftor-Ivacaftor (ETI) therapy.
Single-cell RNA-seq libraries were generated using the Cell Hashing with 10x Single Cell 3' Reagent Kit v3.1 (Dual Index) Protocol (Stoeckius et al., 2018).

There are two batches for this dataset. 
For batch 1, ~110,000 cells from 10 hashed samples with a distinct Hashtag Antibody (HTO) were pooled into one tube to generate four captures.
For batch 2, ~60,000 cells from 6 hashed samples were pooled to generate two captures.
Sequencing data from each capture was pre-processed separately. Two batches were integrated into one dataset for clustering and downstream analysis.

Developers: Anson Wong (main), Hieu T Nim (contributor), Ramialison Laboratory, Australian Regenerative Medicine Institute & Murdoch Children's Research Institute, Australia

Code included in the "src" directory:
  01. Shell script for cellranger multi
  02. R script for QC, HTO demultiplexing and preprocessing
  03. R script for reference-based Human Lung Cell Atlas v2 annotation
  05. R script for clustering
  06. R script for sub-clustering of macrophage
  07. R script for differential expression and pathway enrichment
  08. R script for pseudotime analysis of recruited lung monocytes & macrophages

## References
Stoeckius, M., Zheng, S., Houck-Loomis, B. et al. Cell Hashing with barcoded antibodies enables multiplexing and doublet detection for single cell genomics. Genome Biol 19, 224 (2018). 
