# **Name article**

The following repository contains the notebooks and the libraries used to obtain the results of this article. All datasets and libraries are open sourced and free to use. If you use any of the following in your analysis, please cite them properly.


## **1. Layout**

In the file tree, it is possible to browse an overview of the contents of this repository

├── Enrichment
│   ├── GOBubble
│   │   ├── PA_down.pdf
│   │   └── PA_up.pdf
│   ├── GOChord
│   │   ├── PA_down.pdf
│   │   └── PA_up.pdf
│   ├── enrich_GO
│   │   └── GO_PA.csv
│   ├── enrich_KEGG
│   │   └── KEGG_PA.csv
│   ├── enrich_RE
│   │   └── RE_PA.csv
│   ├── enrich_Wiki
│   │   └── Wiki_PA.csv
│   └── enrich_plots
│       ├── enrichGO.pdf
│       ├── enrichKEGG.pdf
│       ├── enrichRE.pdf
│       └── enrichWP.pdf
├── Expression
│   ├── Annotation
│   │   ├── Anno_astrocyte_counts.csv
│   │   └── allgenesfilt.csv
│   ├── Boxplot.pdf
│   ├── DEGs
│   │   ├── DMEMvsVH.csv
│   │   ├── PA_TIBvsDMEM.csv
│   │   ├── PA_TIBvsVH.csv
│   │   ├── PAvsDMEM.csv
│   │   ├── PAvsTIB.csv
│   │   ├── PAvsVH.csv
│   │   ├── TIBPAvsDMEM.csv
│   │   ├── TIBPAvsVH.csv
│   │   ├── TIB_DMEMvsVHDMEM.csv
│   │   ├── TIBvsVH.csv
│   │   └── VHvsDMEM.csv
│   ├── Heatmap
│   │   └── heatmap.pdf
│   ├── PCA.pdf
│   ├── Volcano
│   │   ├── Vol_DMEMvsVH.pdf
│   │   ├── Vol_PA_TIBvsDMEM.pdf
│   │   ├── Vol_PA_TIBvsVH.pdf
│   │   ├── Vol_PAvsDMEM.pdf
│   │   ├── Vol_PAvsTIB.pdf
│   │   ├── Vol_PAvsTIBPA.pdf
│   │   ├── Vol_PAvsVH.pdf
│   │   ├── Vol_TIBPAvsDMEM.pdf
│   │   ├── Vol_TIBPAvsVH.pdf
│   │   ├── Vol_TIB_DMEMvsVHDMEM.pdf
│   │   ├── Vol_TIBvsVH.pdf
│   │   ├── Vol_TivsDMEM.pdf
│   │   └── Vol_VHvsDMEM.pdf
│   └── astrocyte.rsem.gene_tpm.tsv
├── Notebooks
│   ├── Astrocyte_PPI.Rmd
│   ├── Astrocyte_edgeR.Rmd
│   ├── Astrocyte_enrich.Rmd
│   └── Astrocyte_venn.Rmd
├── Overlapping
│   ├── overlap_DEGs
│   │   ├── PA-DEG_down.csv
│   │   └── PA-DEG_up.csv
│   └── venn
│       ├── PA_down.pdf
│       ├── PA_up.pdf
│       ├── TIBPA_down.pdf
│       ├── TIBPA_up.pdf
│       ├── TIB_down.pdf
│       └── TIB_up.pdf
├── PPI_network
│   ├── PA_proteins.csv
│   ├── PPI
│   │   └── Astrocyte-PPI.cys
│   ├── hub_genes
│   │   ├── DMNC_top20.csv
│   │   ├── Degree_top20.csv
│   │   ├── MCC_top20.csv
│   │   ├── MNC_top20.csv
│   │   ├── common-hub
│   │   │   ├── Upset.pdf
│   │   │   ├── common.csv
│   │   │   └── enrichment
│   │   │       └── GO
│   │   │           ├── GO_hub.csv
│   │   │           └── GO_hub.pdf
│   │   └── curated-hub
│   │       ├── DMNC.csv
│   │       ├── Degree.csv
│   │       ├── MCC.csv
│   │       └── MNC.csv
│   └── modules
│       ├── module_1
│       │   ├── curated-module.csv
│       │   ├── enrichment
│       │   │   ├── GO
│       │   │   │   ├── module1_GO.csv
│       │   │   │   └── module1_GO.pdf
│       │   │   └── KEGG
│       │   │       ├── module1_KEGG.csv
│       │   │       └── module1_KEGG.pdf
│       │   └── raw-module.csv
│       └── module_2
│           ├── curated-module.csv
│           ├── enrichment
│           │   ├── GO
│           │   │   ├── module2_GO.csv
│           │   │   └── module2_GO.pdf
│           │   └── KEGG
│           │       ├── module2_KEGG.csv
│           │       └── module2_KEGG.pdf
│           └── raw_module.csv
├── README.md
└── RNAseq-pipeline
    ├── SRA.csv
    └── astrocyte_multiqc_report.html


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
