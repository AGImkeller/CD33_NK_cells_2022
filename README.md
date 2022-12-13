# CD33_NK_cells_2022

These scripts are part of the paper "CRISPR/Cas9 gene editing of immune checkpoint receptor NKG2A improves the efficacy of primary CD33-directed CAR-NK cells". 

They are used to generate the figures of the CITE-seq experiments. 

D1.Rmd includes pre-processing and downstream analysis such as clustering of donor 1 (D1).
D2.Rmd includes pre-processing of donor 2 (D2).
D1D2Pseudobulk.Rmd includes pseudo-bulk analysis on a combined dataset of D1 and D2. This is used to study the effect of CAR, KO and CAR:KO before coculture with AML-cells as well as the effect of coculture. 
D1D2Differentiation.Rmd includes after-coculture differentiation of D1 and D2. 

We generate two intermediate SingleCellExperiment objects from D1.Rmd and D2.Rmd. These are sce_donor1.Rds and sce_donor2.Rds. They are loaded into D1D2Pseudobulk.Rmd and D1D2Differentiation.Rmd before being used in their analyses. 