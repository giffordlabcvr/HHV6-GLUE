# AAV-GLUE

## Description

This is AAV-GLUE, a [GLUE](http://glue-tools.cvr.gla.ac.uk/) project designed to support
comparative genomic and evolutionary analysis of dependoparvovirus genomes.

AAV-GLUE contains aligned, annotated genome sequence data for:

1. Dependoparvoviruses (family Parvoviridae; genus Dependoparvovirus)
2. Endogenous viral elements (EVEs) derived from dependoparvoviruses

## Sequence data

The sequence data in this project have been organised into the following sources:

*ncbi-refseqs*: Genome-length reference sequences of representative dependoparvovirus species (GenBank XML).

*ncbi-curated*: All dependoparvovirus sequences in GenBank, except those used as references (GenBank XML).

*fasta-curated-*: A non-redundant set of parvovirus-derived EVE loci. These sequences
were extracted from [whole genome sequence](https://www.ncbi.nlm.nih.gov/genome/browse#!/eukaryotes/)
(WGS) assemblies, and were identified using the [DIGS tool](https://giffordlabcvr.github.io/DIGS-tool/). 

*fasta-refseqs-epv*: EVE reference sequences - i.e. best-guess estimates of the ancestral
genome sequences of the ancient dependoparvoviruses that gave rise to EVEs.

## Sequence-associated data

Sequences included in this project are linked to auxiliary data in tabular format, this includes:

1. [Basic taxonomic data](https://github.com/giffordlabcvr/AAV-GLUE/blob/master/tabular/references/parvo-ncbi-refseqs-side-data.tsv) for genome-length virus reference sequence in ncbi-refseqs.
2. [Locus data](https://github.com/giffordlabcvr/AAV-GLUE/blob/master/tabular/locus/epv-locus-data.tsv) for the EVE sequences in fasta-curated.

## Multiple sequence alignments (MSAs)

Several distinct categories of MSA are included in this project, each representing a distinct taxonomic level.

1. [Tip (i)](https://github.com/giffordlabcvr/AAV-GLUE/tree/master/alignments/tips/virus): Virus species (genome-length)
2. [Tip (ii)](https://github.com/giffordlabcvr/AAV-GLUE/tree/master/alignments/tips/eve): EVE lineages (single gene). These alignments contain sets of EVE sequences derived from the same ancestral germline colonisation event (i.e. orthologs or duplicates)
3. [Internal](https://github.com/giffordlabcvr/AAV-GLUE/tree/master/alignments/internal): Dependoparvovirus subclades (genome-length)
4. [Root](https://github.com/giffordlabcvr/AAV-GLUE/tree/master/alignments/root): Dependoparvoviruses (genome-length)

## GLUE project

On computers with
[GLUE](http://glue-tools.cvr.gla.ac.uk/) installed, the AAV-GLUE project can be instantiated by
navigating to the project folder, initiating GLUE, and issuing the following command in the GLUE shell:

	Mode path: /
	GLUE> run file aavProject.glue


## Contributors

Robert J. Gifford (robert.gifford@glasgow.ac.uk)

