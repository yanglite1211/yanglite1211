---
layout: post
categories: posts
title: Build Aggregate Tracks From scATAC-seq
subtitle: >-
  Single-cell ATAC-seq allows scientists to study the chromatin accessibility of
  a heterogenous tissue at single-cell resolution. However, the scATAC-seq data
  is very sparse because in the assay a molecule is present in at most two
  copies for a single cell in a diploid organism (one copy from the father
  chromosome and another form the mother chromosome). As a result, only 1– 10%
  of expected accessible peaks are detected in single cells from scATAC-seq
  data. The sparsity of the scATAC-seq data makes it difficult to recover
  informative features and to assess variability between cells. To overcome this
  problem, one way is to aggregate the data of the same cell types and generate
  ATAC-seq tracks that have deeper sequencing depths while still keeping the
  cell type specificity.
featured-image: /images/scATAC-seq/track.jpg
tags:
  - scATAC-seq
  - ATAC-seq
date-string: 'March 10, 2020'
published: true
---

# Let's get started.

### Prerequisite
1. A 10x scATAC-seq dataset with Cell Ranger ATAC output.
<br>We start with a file named fragments.tsv.gz. It's a BED-like tabular file, where each line represents a unique ATAC-seq fragment captured by the assay. 

<pre><code>## 
## FALSE  TRUE 
##   290  7576</code></pre>

<br>2. Cell type annotation of the dataset. <u><b><a href="https://satijalab.org/seurat/v3.1/atacseq_integration_vignette.html">See an example here.</a></b></u>

### Workflow
<img src="/images/scATAC-seq/workflow.PNG">

### Pipeline and comments
<b><p style="color:#bddd9a">"Demultiplex" fragments.tsv</p></b>
<b><p style="color:#84c1d6">Generate .bed file</p></b>
<b><p style="color:#aa75d2">Generate .bedGraph file</p></b>
<b><p style="color:#da91af">Generate .bw file</p></b>
<b><p style="color:#ffc000">Publish on UCSC Genome Browser</p></b>

------------
<br>Updated on March 11, 2020


<br>Reference
[Chen, Huidong, et al. "Assessment of computational methods for the analysis of single-cell ATAC-seq data." Genome biology 20.1 (2019): 1-25.](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1854-5)
