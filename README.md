
## Overview

This repository presents a reproduction of selected computational analyses from the publication *Dynamical Modeling of Proliferative-Invasive Plasticity and IFNγ Signaling in Melanoma Reveals Mechanisms of PD-L1 Expression Heterogeneity*.

---

## Objectives

- Reproduce the computational analyses presented in the publication.
- Validate reported proliferative–invasive correlations using updated public datasets.
- Compare reproduced results with the published findings.
- Investigate sources of variation arising from different dataset versions.

---

## Figures Reproduced

| Figure | Status | Notes |
|---------|--------|------|
| Figure 1B | ✓ Reproduced | Heatmap generated using authors' workflow |
| Figure 1C | ✓ Reproduced | Scatter plot reproduced using GitHub reference |
| Figure 1D | ✓ Independently reproduced | Correlation analysis using latest datasets |
| Figure 1F(i) | ✓ Independently reproduced | Alternative scRNA-seq dataset used |
| Figure 1F(ii) | ✓ Independently reproduced | Bulk RNA-seq validation |

---

## Datasets

| Dataset | Purpose |
|----------|---------|
| DepMap Public 25Q2 (CCLE Skin) | Figure 1D |
| TCGA-SKCM | Figure 1D |
| GSE115978 (scRNA-seq) | Figure 1F(i) |
| GSE134432 (Bulk RNA-seq) | Figure 1F(ii) |

---

## Key Results

### Figure 1D

| Dataset | Paper | Reproduced |
|----------|-------|-----------|
| CCLE Skin | -0.558 | **-0.651** |
| TCGA-SKCM | -0.427 | **-0.368** |

The observed differences are expected because this analysis used the latest DepMap (Public 25Q2) and TCGA datasets, whereas the original publication used earlier releases.

---

### Figure 1F(i)

The original single-cell dataset (GSE134432) was unavailable through GEO during reproduction.

An alternative melanoma single-cell RNA-seq dataset (**GSE115978**) was therefore used.

Observed Spearman correlation: 0.210

---

### Figure 1F(ii)

Bulk RNA-seq analysis of **GSE134432** produced

- Spearman correlation = **-0.701**
- p-value = **5.57 × 10⁻⁶**

---

## Repository Structure

```
.
├── notebooks/
├── figures/
├── data/
├── README.md
└── requirements.txt
```

---

## Software

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Scikit-learn

---

## Notes

Figures 1B and 1C were reproduced using the authors' GitHub implementation as a reference for the computational workflow.

Figures 1D and 1F were reproduced independently using publicly available datasets.

---

## Reference

Rane A. et al.

*Dynamical Modeling of Proliferative-Invasive Plasticity and IFNγ Signaling in Melanoma Reveals Mechanisms of PD-L1 Expression Heterogeneity.*

---

## Author

**Kinjal Mehendale**

Undergraduate Student  
Electrical Engineering, VJTI Mumbai

Interested in Computational Oncology • Cancer Genomics • Systems Biology • AI for Precision Medicine
