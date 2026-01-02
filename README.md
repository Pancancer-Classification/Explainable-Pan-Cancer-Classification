# Explainable Pan-Cancer Classification and Biomarker Discovery

This repository accompanies the paper:

**Explainable Pan-Cancer Classification and Biomarker Discovery from mRNA Gene Expression**

We propose an interpretable machine learning framework for accurate pan-cancer classification and cancer-type–specific biomarker identification using TCGA mRNA gene expression data.

---

## Overview

- **Cancer types**: 33  
- **Samples**: 10,496  
- **Initial features**: 19,238 genes  
- **Selected features**: 500  
- **Best accuracy**: 96.61%

The proposed approach addresses high-dimensional RNA-seq data, limited cancer-specific biological insight, and the lack of interpretability in high-performing classifiers.

---

## Dataset Summary (TCGA)

### Number of Samples per Cancer Type

| # | Cancer Type | Sample Count |
|---|------------|--------------|
| 1 | ACC | 77 |
| 2 | BLCA | 426 |
| 3 | BRCA | 1211 |
| 4 | CESC | 309 |
| 5 | CHOL | 45 |
| 6 | COAD | 329 |
| 7 | DLBCL | 47 |
| 8 | ESCA | 195 |
| 9 | GBM | 165 |
|10 | HNSC | 564 |
|11 | KICH | 91 |
|12 | KIRC | 603 |
|13 | KIRP | 321 |
|14 | LAML | 173 |
|15 | LGG | 522 |
|16 | LIHC | 421 |
|17 | LUAD | 574 |
|18 | LUSC | 548 |
|19 | MESO | 87 |
|20 | OV | 427 |
|21 | PAAD | 183 |
|22 | PCPG | 185 |
|23 | PRAD | 548 |
|24 | READ | 102 |
|25 | SARC | 264 |
|26 | SKCM | 470 |
|27 | STAD | 450 |
|28 | TGCT | 137 |
|29 | THCA | 571 |
|30 | THYM | 121 |
|31 | UCEC | 194 |
|32 | UCS | 57 |
|33 | UVM | 79 |
| **—** | **Total** | **10,496** |

---

## Differential Gene Expression Analysis (DESeq2)

Differential expression analysis was performed using DESeq2 to statistically validate cancer-specific genes identified through explainable AI.

### Cancer-wise Differentially Expressed Genes

| Cancer | Tumor Samples | Healthy Samples | DEGs |
|-------|---------------|-----------------|------|
| BLCA | 364 | 19 | 802 |
| BRCA | 984 | 112 | 707 |
| CHOL | 33 | 11 | 1904 |
| COAD | 287 | 43 | 878 |
| ESCA | 185 | 13 | 818 |
| HNSC | 462 | 44 | 889 |
| KICH | 62 | 27 | 1449 |
| KIRC | 477 | 74 | 821 |
| KIRP | 238 | 31 | 768 |
| LIHC | 297 | 50 | 737 |
| LUAD | 505 | 61 | 1026 |
| LUSC | 491 | 53 | 1769 |
| PRAD | 428 | 50 | 266 |
| READ | 89 | 12 | 883 |
| STAD | 382 | 35 | 637 |
| THCA | 443 | 55 | 445 |
| UCEC | 143 | 25 | 1205 |

---

## Methodology

1. Feature normalization and selection to mitigate dimensionality  
2. Ensemble classification using Logistic Regression, SVM, and XGBoost  
3. Explainable AI (SHAP) for global and cancer-specific gene attribution  
4. Statistical validation using DESeq2  

---

## Code Availability

> **Code will be made available upon reasonable request.**

---

## Citation

Please cite the corresponding paper if you use this work.
