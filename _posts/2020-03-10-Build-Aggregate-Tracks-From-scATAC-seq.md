---
layout: post
categories: posts
title: Build Aggregate Tracks From scATAC-seq
subtitle: >-
  Single-cell ATAC-seq allows scientists to study the chromatin accessibility of
  a heterogenous tissue at single-cell resolution. However, the sparsity of the
  scATAC-seq data makes it to recover informative features and to assess
  variability between cells.
featured-image: /images/scATAC-seq/track.jpg
tags:
  - scATAC-seq
  - ATAC-seq
date-string: 'March 10, 2020'
published: true
---
Single-cell ATAC-seq allows scientists to study the chromatin accessibility of a heterogenous tissue at single-cell resolution. However, the scATAC-seq data is very sparse because in the assay a molecule is present in at most two copies for a single cell in a diploid organism (one copy from the father chromosome and another form the mother chromosome). As a result, only 1– 10% of expected accessible peaks are detected in single cells from scATAC-seq data. The sparsity of the scATAC-seq data makes it difficult to recover informative features and to assess variability between cells. To overcome this problem, one way is to aggregate the data of the same cell types and generate ATAC-seq tracks that have deeper sequencing depths while still keeping the cell type specificity.

<br>**What we have before start



------------
<br>Updated on March 10, 2020


<br>Reference
[Chen, Huidong, et al. "Assessment of computational methods for the analysis of single-cell ATAC-seq data." Genome biology 20.1 (2019): 1-25.](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1854-5)
