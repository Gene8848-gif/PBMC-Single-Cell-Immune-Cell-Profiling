# PBMC Single-Cell Immune Cell Profiling

## Overview

This project analyzes single-cell RNA-sequencing (scRNA-seq) data from peripheral blood mononuclear cells (PBMCs) using Python and Scanpy.

The goal of the project is to identify and characterize different immune-cell populations based on their gene-expression patterns and to demonstrate a complete introductory single-cell RNA-seq analysis workflow.

## Research Question

**Can single-cell gene-expression data be used to identify and characterize different immune-cell populations in peripheral blood?**

## Dataset

The analysis uses the publicly available **PBMC3k** dataset, consisting of approximately 2,700 peripheral blood cells measured across thousands of genes.

The dataset contains a mixture of immune-cell populations, making it useful for learning single-cell RNA-seq analysis and immune-cell identification.

## Analysis Workflow

The analysis follows these major steps:

1. Load the PBMC3k dataset
2. Perform quality-control analysis
3. Calculate mitochondrial gene expression
4. Filter low-quality cells
5. Normalize and log-transform gene expression
6. Identify highly variable genes
7. Scale the data
8. Perform principal component analysis (PCA)
9. Construct a neighborhood graph
10. Generate a UMAP embedding
11. Perform Leiden clustering
12. Identify cluster-specific marker genes
13. Annotate immune-cell populations
14. Quantify the identified cell populations
15. Interpret the biological findings

## Tools and Technologies

- **Python**
- **Scanpy**
- **AnnData**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Single-cell RNA-seq analysis**
- **PCA**
- **UMAP**
- **Leiden clustering**
- **Marker-gene analysis**

## Identified Cell Populations

Seven major cell populations were identified based on cluster-specific gene-expression patterns:

| Cell Population | Representative Markers |
|---|---|
| T cells | CD3D, CD3E |
| NK/cytotoxic cells | NKG7, GNLY, CCL5 |
| Classical monocytes | S100A8, S100A9, LYZ, FCN1 |
| B cells | MS4A1, CD79A, CD74 |
| FCGR3A+ monocytes | FCGR3A, LST1, FCER1G, AIF1, CST3 |
| Dendritic cells | FCER1A, HLA-DRA, CST3 |
| Megakaryocyte-like cells | PF4, PPBP, RGS18 |

## Cell Population Distribution

The identified populations showed the following approximate distribution:

- **T cells:** 43.33%
- **NK/cytotoxic cells:** 17.48%
- **Classical monocytes:** 16.72%
- **B cells:** 13.08%
- **FCGR3A+ monocytes:** 7.58%
- **Dendritic cells:** 1.33%
- **Megakaryocyte-like cells:** 0.49%

T cells represented the largest population, followed by NK/cytotoxic cells, monocytes, and B cells.

## Biological Interpretation

The analysis demonstrates the heterogeneity of peripheral blood immune cells at the single-cell level.

Distinct gene-expression patterns allowed lymphoid and myeloid populations to be separated into different clusters. The analysis also identified heterogeneity within the monocyte compartment, with separate classical and FCGR3A+ monocyte populations.

These cell identities were assigned using patterns of marker-gene expression rather than relying on individual genes alone.

## Key Learning Outcomes

Through this project, I gained practical experience with:

- Working with single-cell RNA-seq data
- Performing quality control and normalization
- Dimensionality reduction using PCA and UMAP
- Unsupervised cell clustering
- Identifying marker genes
- Interpreting immune-cell gene-expression profiles
- Annotating cell populations using biological knowledge
- Quantifying cell-type composition
- Using Python and Scanpy for computational biology

## Limitations

Cell-type annotations in this project are working annotations based primarily on marker-gene expression.

More detailed annotation approaches, additional marker genes, reference-based annotation methods, and biological validation would be required to establish definitive cell identities.

The dataset also represents peripheral blood from a healthy context and therefore does not directly model disease or the tumor microenvironment.

## Conclusion

This project demonstrates an introductory single-cell RNA-seq workflow for identifying and characterizing immune-cell populations in peripheral blood.

Using the PBMC3k dataset, quality control, normalization, PCA, UMAP, Leiden clustering, and marker-gene analysis were combined to identify seven major cell populations.

This project provided practical experience with Python-based single-cell analysis and established a foundation for applying similar computational approaches to more complex disease and tumor-immune datasets.

## Project Structure

```text
PBMC-Single-Cell-Immune-Cell-Profiling/
│
├── PBMC_Single_Cell_Immune_Cell_Profiling.ipynb
└── README.md
