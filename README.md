# Identification of Regulatory Hub Genes in Alzheimer’s Disease Using Transcriptomic and Network Analysis

## Overview

This project investigates gene-expression changes associated with Alzheimer’s disease using the GEO transcriptomic dataset **GSE122063**. Differential expression analysis was performed between Alzheimer’s disease and control samples, followed by visualization and protein–protein interaction network analysis to identify regulatory hub genes.

## Objectives

* Identify differentially expressed genes (DEGs) between Alzheimer’s disease and control samples.
* Analyze overall transcriptomic variation using PCA.
* Visualize significant gene-expression changes using volcano plots and heatmaps.
* Construct a Protein–Protein Interaction (PPI) network.
* Identify highly connected hub genes using network centrality analysis.
* Interpret the biological relevance of the identified hub genes.

## Dataset

**Dataset:** GSE122063
**Source:** Gene Expression Omnibus (GEO)
**Organism:** *Homo sapiens*

The analysis focused on:

* Alzheimer’s disease samples: **56**
* Control samples: **44**
* Total samples analyzed: **100**

## Analysis Workflow

```text
GEO Dataset (GSE122063)
        ↓
Expression Matrix Processing
        ↓
Sample Selection
        ↓
Alzheimer’s Disease vs Control
        ↓
Differential Expression Analysis
        ↓
DEG Filtering
        ↓
PCA + Volcano Plot + Heatmap
        ↓
Gene Selection
        ↓
STRING / PPI Network Analysis
        ↓
Network Centrality Analysis
        ↓
Hub Gene Identification
        ↓
Biological Interpretation
```

## Differential Expression Analysis

Gene-expression values were compared between Alzheimer’s disease and control groups. For each gene, log2 fold change and p-value were calculated.

The filtering criteria used were:

```text
|log2FC| > 1
p-value < 0.05
```

The analysis identified:

* **529 significant DEGs**
* **153 upregulated genes**
* **376 downregulated genes**

## Visualization

### PCA

Principal Component Analysis was performed to evaluate the overall transcriptomic variation among samples.

* PC1: **37.6%**
* PC2: **11.3%**
* Combined variance: **48.9%**

### Volcano Plot

A volcano plot was generated to visualize the relationship between fold change and statistical significance of the identified genes.

### Heatmap

A heatmap of the top differentially expressed genes was generated to visualize expression patterns across Alzheimer’s disease and control samples.

## PPI Network Analysis

The selected genes were analyzed using the **STRING database** to investigate protein–protein interactions. Network centrality was then used to identify highly connected genes that may represent important components of the disease-associated interaction network.

## Identified Hub Genes

The analysis identified the following 15 hub genes:

```text
SNAP25
GFAP
BDNF
CALB1
SST
NEFL
SLC17A6
SLC32A1
GAD1
GAD2
SYP
CCL2
TAC1
PVALB
```

These genes are associated with processes including **synaptic function, neuronal signaling, neurotransmitter regulation, neuroinflammation, neuronal structure, and neuronal survival**.

## Key Findings

* Identified **529 significant differentially expressed genes**.
* Detected **153 upregulated** and **376 downregulated** genes.
* PCA demonstrated differences in the transcriptomic profiles of Alzheimer’s disease and control samples.
* Expression patterns of significant genes were visualized using volcano plots and heatmaps.
* PPI network analysis identified **15 candidate hub genes**.
* **SNAP25** was identified as a highly connected hub gene in the network.
* The identified hub genes highlight several biological processes relevant to neuronal function and Alzheimer’s disease.

## Tools & Technologies

* **Python**
* **Jupyter Notebook / Google Colab**
* **Pandas**
* **NumPy**
* **SciPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **GEO**
* **STRING**

## Repository Contents

```text
├── README.md
├── Alzheimer_DEG_GSE122063_MinorProject.ipynb
├── data/
├── results/
└── figures/
```

## Conclusion

This project demonstrates an integrated transcriptomic and network-based approach for identifying candidate regulatory hub genes associated with Alzheimer’s disease. By combining differential expression analysis with PPI network analysis, a set of 15 candidate hub genes was prioritized for further biological investigation.

## Author

**Ruksar Attar**

M.Tech. Biotechnology and Biochemical Engineering
Indian Institute of Technology Kharagpur
