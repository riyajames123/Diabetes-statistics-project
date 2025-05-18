# 🧪 Diabetes Multi-Omics Statistical Analysis

This repository contains the full analysis pipeline and results for a statistical study of multi-omics data (RNA-seq and lipidomics) from human pancreatic islet donors, aimed at understanding molecular differences across stages of diabetes.

---

## 📁 Dataset Overview

- **RNA-seq**: Gene expression data for 16,353 genes across 134 samples
- **Lipidomics**: Quantification of 116 lipid species across 44 samples
- **Metadata**: Clinical covariates including Age, BMI, HbA1c, OGTT, and diabetes diagnosis (ND, IGT, T2D, T3cD)

---

## 🎯 Objectives

- Perform distribution and normality checks across samples
- Apply data transformations and assess improvement in normality
- Detect and remove outliers using appropriate techniques
- Conduct hypothesis testing to identify significant group differences
- Analyze clinical covariate correlations with gene/lipid features
- Perform PCA and clustering to explore sample groupings

---

## 🔍 Key Methods

- **Shapiro-Wilk Test** for normality
- **Transformations**: Log1p, Square Root, Reciprocal, Z-score
- **Outlier Detection**:
  - IQR method for lipidomics (per feature)
  - PCA-based distance for RNA-seq (per sample)
- **Hypothesis Testing**:
  - Kruskal-Wallis (global group comparison)
  - Wilcoxon Rank-Sum (pairwise comparisons)
- **Spearman Correlation** between clinical covariates and features
- **Principal Component Analysis (PCA)** for dimensionality reduction
- **KMeans Clustering** for grouping analysis

---

## 📊 Results Summary

- **RNA-seq** data showed strong group differences, especially between T2D and ND/IGT.
- **Lipidomics** exhibited selective pairwise differences, but no global group separation.
- HbA1c was the strongest clinical correlate with gene expression (Spearman ρ ≈ 0.67).
- PCA and clustering showed clearer separation in lipidomics than RNA-seq.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `diabetes_pca_analysis.ipynb` | Jupyter notebook containing the full analysis pipeline |
| `README.md` | This file |
| `data/` | Folder with input datasets |


---

## 📘 Reference

Wigger, L., Barovic, M., Brunner, A. D., et al. (2021). *Multi-omics profiling of living human pancreatic islet donors reveals heterogeneous beta cell trajectories towards type 2 diabetes.* Nature Metabolism.  
https://doi.org/10.1038/s42255-021-00420-9


---

## 💬 Contact

For questions or collaboration, feel free to reach out at riyajames1909@gmail.com


