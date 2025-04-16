# 🧬 Single-Cell RNA-seq Analysis of Pancreatic Cancer (PDAC)

This repository contains the analysis pipeline for exploring **single-cell transcriptomic differences** between **normal and tumor samples** in **pancreatic ductal adenocarcinoma (PDAC)**. The project applies dimensionality reduction, clustering, differential gene expression, and functional enrichment techniques to reveal tumor-specific biological insights at single-cell resolution.

## 🔍 Project Overview

- **Objective**: Identify molecular and cellular differences between tumor and normal cells in PDAC using single-cell RNA-seq data.
- **Approach**: Dual-path analysis using **separate** and **combined** representations of tumor and normal samples.
- **Key Highlights**:
  - Unsupervised clustering of cell populations
  - DEG analysis at both global (tumor vs normal) and local (within clusters) levels
  - Functional enrichment and pathway analysis (GO & KEGG)
  - Automated cell type annotation using reference datasets

---

## 🧪 Methods & Workflow

### 📦 Preprocessing & Quality Control
- Filtering low-quality cells
- Normalization and log transformation
- Selection of highly variable genes

---

### 🔹 Path 1: Separate Latent Representations (Normal & Tumor)
- Dimensionality reduction using PCA, UMAP, and t-SNE
- Clustering using KMeans and DBSCAN
- Cluster-level differential gene expression (DEG)
- Identification of cluster-specific driver genes
- GO enrichment analysis for top markers

---

### 🔸 Path 2: Combined Latent Representation (Merged Dataset)
- Unified analysis of tumor + normal cells
- UMAP and t-SNE visualization of integrated space
- Clustering (KMeans, DBSCAN)
- DEG between tumor and normal conditions
- KEGG pathway enrichment of tumor-associated DEGs
- Reference-based automated cell type annotation
- Cluster visualization with annotated cell types

---

## 🧰 Tools & Technologies Used
- **Single-cell RNA-seq** (10x-style format)
- **Dimensionality reduction**: PCA, UMAP, t-SNE
- **Clustering**: KMeans, DBSCAN
- **Differential Expression**: Wilcoxon Rank-Sum Test
- **Functional Enrichment**: GO, KEGG
- **Cell Type Annotation**: Reference-based automated annotation


---

## 📂 Repository Structure

