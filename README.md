These scripts are part of the paper "CRISPR/Cas9 gene editing of immune checkpoint receptor NKG2A improves the efficacy of primary CD33-directed CAR-NK cells". 

They are used to generate the figures of the CITE-seq experiments. 

D1.Rmd includes pre-processing and downstream analysis such as clustering of donor 1 (D1).
D2.Rmd includes pre-processing of donor 2 (D2).
D1D2Pseudobulk.Rmd includes pseudo-bulk analysis on a combined dataset of D1 and D2. This is used to study the effect of CAR, KO and CAR:KO before coculture with AML-cells as well as the effect of coculture. 
D1D2Differentiation.Rmd includes after-coculture differentiation of D1 and D2. 

We generate two intermediate SingleCellExperiment objects from D1.Rmd and D2.Rmd. These are sce_donor1.Rds and sce_donor2.Rds. They are loaded into D1D2Pseudobulk.Rmd and D1D2Differentiation.Rmd before being used in their analyses.

CITE-Seq data analysis was performed on:
----------------------------------------
- R version 4.3.0 (2023-04-21)
- Platform: x86_64-pc-linux-gnu (64-bit)
- Running under: Ubuntu 20.04.6 LTS

The R packages/software used:
-----------------------------
- edgeR (Robinson et al., 2010)
- limma (Ritchie et al., 2015)
- tidyverse (Wickham et al., 2019)
- SingleCellExperiment (Amezquita et al., 2020)
- scran (Lun et al., 2016)
- scater (McCarthy et al., 2017)
- igraph (Csardi & Nepusz, 2006)
- bluster (Lun, 2022)
- aricode (Chiquet et al., 2022)
- Wind (Wu & Wu, 2019)
- ggplot2 (Wickham, 2016)
- pheatmap (Kolde, 2019)
- patchwork (Pedersen, 2022)
- cowplot (Wilke, 2020)
- ggrepel (Slowikowski, 2022)
- ggplotify (Yu, 2021)
- ggpubr (Kassambara, 2022)
- magrittr (Bache & Wickham, 2022)
- scDblFinder (Germain et al., 2021)

The version of all the R packages/software used and session info is prined out in the scripts' corresponding html files.
