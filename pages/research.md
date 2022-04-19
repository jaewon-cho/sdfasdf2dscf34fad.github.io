---
layout: page
title: Research
permalink: /research
---

The cell is the fundamental unit of biology, and long term changes involve a coordinated response which is ultimately determined by the genome. Today it is possible to obtain high-throughput, global, quantitative measurements of the genome, the transcriptome, the epigenome, and the proteome from individual cells. Analysis and integration of these large, complex, noisy datasets pose many challenges. As a computational genomics group, our goal is to develop machine learning methods that will provide new insights both for basic biology as well as for understanding how aberrant gene regulation plays a role in cancer, neurodegeneration and other diseases. We seek to develop scalable, robust, rigorous computational tools for tackling important biological problems. We are particularly interested in areas involving single-cell analysis, including multi-omics assay, spatial methods, and datasets from population studies. 

## Methods Development


![Computational methods development](/assets/img/desk.png)

We are interested in developing novel computational methods for analyzing high throughput sequencing data. In particular, there has been a focus on single-cell RNAseq, but we are also interested in other types of sequencing data.

### Fast unsupervised clustering

![SC3s flow chart](/assets/img/sc3s.png)

In 2017, we published the single cell consensus clustering [method](https://github.com/hemberg-lab/SC3) (SC3) which is a robust and accurate method for unsupervised clustering of scRNAseq data. The main shortcoming of the algorithm, however, is its poor scalability to samples with more than a few thousand cells. The new [SC3 with speed](https://github.com/hemberg-lab/sc3s) (SC3s) improves several bottlenecks in the algorithm which allows it to scale linearly in time and memory with the number of cells.

### Coordinated splicing events in scRNAseq data

Protocols that allow for full-length coverage of transcripts make it possible to investigate the utilization of different splice junctions at the single-cell level. Even though isoform quantification is a challenging problem given the protocols used today, it is possible to accurately assess the usage of splice junctions. By building a data structure that allows for fast queries of splice junction usage across all cells profiled in a scRNA-seq experiment, we can systematically search for cell-type specific splicing patterns, e.g. flip-flop exons and other co-regulated splicing events. Moreover, it will allow us to identify cell-type specific splicing events, akin to marker genes.

### Quantitative models of regulatory motifs at promoters and enhancers


![Example scover analysis](/assets/img/scover.png)

Building on our recent work using convolutional neural networks for identification and quantification of regulatory motifs, we will expand the model to study the impact of distal enhancers as well. This will allow us not only to discover regulatory elements that are preferentially found at either promoters or enhancers, but also to quantify their impact on gene expression. Furthermore, we also seek to incorporate non-coding genetic variants.

## Collaborative Projects

We have worked with several experimental group in a wide range of areas including neuroscience, immunology and cancer.

### Perianal fistulizing disease

We are working with the [Salas lab](https://www.clinicbarcelona.org/en/idibaps/research-areas/liver-digestive-system-and-metabolism/inflammatory-bowel-disease) at IDIBAPS in Barcelona to profile patients with this subtype of inflammatory bowel disease. It is our hope that single-cell profiling will make it possible to identify biomarkers and therapeutic targets.

### Characterization of sequences absent from the genome

In collaboration with the [Ahituv lab](https://pharm.ucsf.edu/ahituv) we are investigating [nullomers](https://en.wikipedia.org/wiki/Nullomers), short k-mers that are *absent* from the genome. In our first publication we have characterized both nullomers and nullpeptides across 30 species as well as across human populations, and in a subsequent [preprint](https://www.medrxiv.org/content/10.1101/2021.08.15.21261805v1) we demonstrate how these sequences can be used as cancer biomarkers. Importantly, this includes liquid biopsies which implies that no tumor DNA is required.


### CAR T-cells for solid tumors

Together with the [Marasco lab](https://marascolab.dana-farber.org/) at the Dana-Farber Institute we are trying to understand the mechanisms involved in a novel design which is aimed at overcoming the suppresive tumor microenvironment. We are using scRNA-seq to profile the immune microenvironment.
