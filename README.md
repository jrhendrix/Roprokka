# ROP
Report on Prokka
This script reports important information about a bacterial genome assembly using Prokka annotation data

## Table of Contents

Table of Contents
0. Run Prokka
1. Record the basic assembly and annotation stats
2. Calculate % hypothetical proteins.
3. BLAST species identifying genes
4. Plasmid detection

## Usage
As input, this script takes a directory of Prokka output or a FASTA sequence file. If only a FASTA is provided, Prokka will be run.


## Report Basic Stats
Currently, this functionality is set up to display the statistics presented in the Prokka tsv file

## Calculate the percentage of CDS that are hypothetical proteins
The percent hypothetical is an important statistic for determining assembly quality. Due to limitations in current knowlege, there are many bacterial CDS that have not been annotated. Thus, an assembly where 40-60% of CDS are hypothetical proteins may still be a high quality assembly. However, if the percent hypothetical exceeds 90%, the quality/usability should be questioned.

## Species identification
