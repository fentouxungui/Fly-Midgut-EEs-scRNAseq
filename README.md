# Fly-Midgut-EEs-scRNAseq
## About
This is the analysis code of the scRNAseq data from paper: [The Cellular Diversity and Transcription Factor Code of Drosophila Enteroendocrine Cells](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3409458).

## Region_specific_gene_enrichment
Region specific gene enrichment (RSGE) arthrogram
To evaluate the regional preference of each cluster, we used the bulk EE RNA-seq data of different midgut regions from the Flygut-seq database (http://flygutseq.buchonlab.com/resources) (Dutta et al., 2015). For each region, genes with RPKM >= 3.5 and fold enrichment over other four regions more than 2.5 were profiled, and the top 100 genes according to fold enrichment were selected as the region-specific gene sets to perform subsequent analysis. To evaluate whether cells from scRNA-seq data express certain genes, we set a cutoff with the scaled value of 0.5, and then calculated the percentages of the cells expressing these region-specific genes in each cluster. The summed percentages of the 100 genes of each region were represented as the regional enrichment score for each cluster.

## neuropeptides_combination
To investigate peptide hormones co-expression patterns at single cell level, we set the scaled value 0.5 as the threshold to distinguish whether a peptide is expressed or not. Totally 14 peptide hormones were composed in this step. The barplot of peptides combination was made by R package ggplot2. 

## EEs_TF_Code_1e4
TF code analysis, please see [felixhorns/FlyPN](https://github.com/felixhorns/FlyPN)

## Data Portal
We also provide an online scRNAseq data query [portal](https://xilab.shinyapps.io/database).
