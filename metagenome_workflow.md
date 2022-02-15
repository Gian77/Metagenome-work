# Metagenomics Pipeline

#### MIT License - Copyright (c) 2021 GMNB

## **(1)** EVALUATING RAW SEQUENCE READs QUALITY

This step serves to have a general idea of the overall quality of the `fastq` reads.
* Tools required: [FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/)<br>

## **(2)** QUALITY FILTERING

In this steps, low quality reads are removed and adapters are trimmed of the read pool.
Tools required:<br>
* [Trimmomatic](http://www.usadellab.org/cms/?page=trimmomatic)<br>
* [Fast-p](https://github.com/OpenGene/fastp#fastp)<br>

## **(3)** TAXONOMIC CLASSIFICATION

In this step we assigns taxonomic labels to sequence reads by examining different k-mers and using the information within those k-mers to query a database. We can then can model the abundances at any standard taxonomy level, including species/genus-level abundance.
Tools required:<br>
* [Kraken2](https://ccb.jhu.edu/software/kraken2/)<br>
* [Braken](https://ccb.jhu.edu/software/bracken/)<br>

## **(4)** ASSEMBLY

We can the extract the classified reads and we can perform a meta-assemly.
Tools required:<br>
* [Meta-spades](https://github.com/ablab/spades)<br>
* [Mega-Hit](https://github.com/voutcn/megahit)<br>

## **(5)** BINNING

The we can clusters the metagenomic contigs into different "bins", each of which should correspond to a putative genome. There are several tools for this step. One apprach is to use 2 or 3 different tools and then generate a consensus among them.

Tools required:<br>
* [Metabat2](https://bitbucket.org/berkeleylab/metabat/src/master/)<br>
* [MaxBin](https://sourceforge.net/projects/maxbin2/)<br>

For Consensus:<br>
* [Das Tool](https://github.com/cmks/DAS_Tool)<br>

# **(6)** MAGs QUALITY and COMPLETEDNESS
This steps is to evaluate contamination and completedness.
Tools required:<br>
* [CheckM](https://ecogenomics.github.io/CheckM/)<br>
* [GTDB-tk](https://github.com/Ecogenomics/GTDBTk)<br>

# **(7)** EXTRACTING MAGs

# **(8)** ANNOTATION
Tools required:<br>
* [prokka](https://github.com/tseemann/prokka)<br>
* [metaprodigal](https://github.com/hyattpd/Prodigal)<br>
* [eggnog](https://github.com/eggnogdb/eggnog-mapper)<br>
