# Metagenome Assembly and Annotation

### Some references that can be useful:

* [Quince et al. 2017 - Shotgun metagenomics, from sampling to analysis](https://pubmed.ncbi.nlm.nih.gov/28898207/)
* [Sharpton, 2014 - An introduction to the analysis of shotgun metagenomic data](https://pubmed.ncbi.nlm.nih.gov/24982662/)
* [Kunin et al. 2008 - A bioinformatician's guide to metagenomics](https://pubmed.ncbi.nlm.nih.gov/19052320/)

Other general web pages

* https://rpubs.com/ednachiang/MetaG_Pipeline

Before starting, is very important to understand the questions that were behind your metagenomic experiment. What were your goals? Perhaps you were interested in pooling  
out several genes of interest and compare them across treatments; reconstruct and assemble different genomes coming from the same substrate (e.g. MAGs); identify specific taxa and even characterize simple biological communities and their potential functions etc.

## **(1)** EVALUATING SEQUENCE READS QUALITY

This step serves to have a general idea of the overall quality of the `fastq` reads.
Tools required: [FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/)  

## **(2)**  QUALITY FILTERING

In this steps, low quality reads are removed.
