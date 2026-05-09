# Spatial Transcriptomics of Therapy-Resistant Breast Cancer Niches

## Modeling Tumor–Stroma Resistance Ecosystems Using Spatial Omics

This project investigates how **COXIS-high tumor regions** and **LRRC15+ cancer-associated fibroblasts (CAFs)** spatially organize within breast tumors to create therapy-resistant microenvironments.

Using **10x Genomics Visium spatial transcriptomics**, this pipeline combines:

* Spatial omics
* Computational oncology
* Transcriptomic clustering
* Differential expression analysis
* Pathway enrichment
* Tumor microenvironment modeling

to identify biological programs linked to:

* immune exclusion
* EMT activation
* stromal remodeling
* therapy resistance

---

# Why This Matters

Resistance to cancer therapy is often driven not only by tumor cells themselves, but by interactions between tumor cells and the surrounding microenvironment.

This project explores:

* how resistant tumor niches spatially emerge
* how fibroblasts remodel tumor architecture
* how inflammatory signaling programs correlate with immune suppression

The findings support a model where:

> COXIS-high tumor nests coexist with LRRC15+ stromal regions to form spatially organized therapy-resistant ecosystems.

This has potential applications in:

* biomarker discovery
* immunotherapy response prediction
* computational pathology
* spatial AI modeling
* translational oncology

---

# Technical Skills Demonstrated

## Bioinformatics & Computational Biology

* Spatial transcriptomics analysis
* RNA-seq preprocessing
* Gene signature scoring
* Differential expression analysis
* Pathway enrichment analysis
* Tumor microenvironment modeling

## Data Science & Machine Learning Foundations

* High-dimensional data analysis
* Feature selection using HVGs
* Dimensionality reduction (PCA/UMAP)
* Graph-based clustering
* Statistical hypothesis testing

## Tools & Frameworks

* R / Bioconductor
* SpatialExperiment
* scater
* scran
* clusterProfiler
* ComplexHeatmap
* ggplot2
* igraph
* signifinder

---

# Dataset

| Feature   | Description             |
| --------- | ----------------------- |
| Platform  | 10x Genomics Visium     |
| Disease   | Breast Cancer           |
| Data Type | Spatial Transcriptomics |
| Spots     | 355                     |
| Genes     | ~17,943                 |

---

# Analysis Pipeline

## 1. Quality Control

* Low-quality spot filtering
* Library size assessment
* Gene detection thresholds

## 2. Normalization

* Library size factor normalization
* Log-normalization

## 3. Feature Selection

* Top highly variable genes (HVGs)

## 4. Dimensionality Reduction

* PCA
* UMAP

## 5. Graph-Based Clustering

* Leiden clustering on PCA neighbor graph

## 6. Differential Expression

Identified:

* stromal markers
* tumor markers
* hypoxia/stress-response programs

## 7. Gene Signature Scoring

Scored:

* COXIS
* LRRC15 CAF
* EMT
* HRDS
* Immunotherapy non-response signatures

## 8. GO Pathway Enrichment

Revealed enrichment in:

* extracellular matrix organization
* immune interaction pathways
* stress adaptation pathways

---

# Key Findings

## Tumor-Rich Regions

Enriched for:

* COXIS signaling
* stress-adaptation programs
* tumor-associated transcriptional states

## CAF-Rich Regions

Enriched for:

* LRRC15 CAF signatures
* extracellular matrix remodeling
* EMT programs
* immune exclusion signatures

## Spatial Organization

The analysis suggests resistant tumor ecosystems are spatially structured rather than randomly distributed.

---

# Example Biological Signals Identified

## CAF/Stromal Markers

* COL1A1
* COL3A1
* POSTN
* SPARC
* MMP2

## Tumor Markers

* MUCL1
* MAL2
* AZGP1

## Stress/Hypoxia Markers

* HMOX1
* FTL
* IFI6

---

# Repository Structure

```bash id="sccf1l"
├── data/
├── scripts/
├── figures/
├── results/
└── README.md
```

---

# Example Outputs

This project generates:

* Spatial tissue maps
* PCA projections
* UMAP embeddings
* Leiden cluster visualizations
* Differential expression heatmaps
* Signature enrichment plots
* GO enrichment analyses

---

# Future Extensions

Potential future directions include:

* single-cell + spatial integration
* graph neural networks
* spatial AI models
* ligand–receptor interaction analysis
* clinical response prediction
* Neo4j biological knowledge graphs
* multi-cancer comparative analysis

---

# Reproducibility

```r id="rt5vh2"
# Install required packages
BiocManager::install(c(
  "SpatialExperiment",
  "scater",
  "scran",
  "clusterProfiler",
  "ComplexHeatmap",
  "signifinder"
))
```

---

# Authors

* Mojgan Darvishi
* Andrew Kisitu

---

# License

MIT License
