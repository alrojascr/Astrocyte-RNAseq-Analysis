# **Palmitic Acid Upregulates Type I Interferon-Mediated Antiviral Response and Cholesterol Biosynthesis in Human Astrocytes**

The following repository contains the notebooks and the libraries used to obtain the results of this article. All datasets and libraries are open sourced and free to use. If you use any of the following in your analysis, please cite them properly.


## **1. RNAseq-pipeline**

A detailed report of the astrocyte transcriptome analysis is found with the `rnaseq` pipeline from `nf-core`, which is generated by MultiQC; a visualization tool that generates a single HTML report summarizing all samples in the project


## **2. Expression**

Differential expression analysis was conducted using the bioconductor `edgeR` package. We used the gene-level counts matrix to identify significant differentially expressed genes (DEGs) across 12 comparisons


## **3. Overlapping**

The identification of overlapping DEGs was conducted with the `ggVennDiagram` package through differentiating those that were significantly up- and down-regulated


## **4. Enrichment**

It contains the functional enrichment results for human astrocytes. Over-representation analyses were performed using the `clusterProfiler` package implemented in R


## **5. PPI_network**

PPI network was constructed from the STRING database using Cytoscape. From this network, we identified significant gene clustering modules and hub genes using the MCODE and Cytohubba plugins, respectively


## **6. Notebooks**

All source code is in `Rmarkdown` style to run step by step all the analysis


## **Running analysis**

1. Install R and R Studio if needed
2. Clone this repository
3. Install required R packages
4. Knit the R Markdown files in order


## **Bug Reports**

Please report bugs through the GitHub issues system
