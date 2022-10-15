# Supplementary Background Information
This file contains additional background information for ropro. This information is not necessary for running ropro or for understanding the output. Instead, this document contains notes describing the biological implications and for possibly inturpreting the significance of the output. 

## Annotations

## tRNA
The number of tRNAs in an assembly can be indicative of assembly completeness and quality (Land, 2014).
In order to express a gene and make a protein, DNA is transcribed into mRNA (messenger RNA) which will contain the reverse compliment sequence where Ts have been replaced with Us). The mRNA is then translated into protein (the Central Dogma of Genetics). 

During translation, the sequence is read in units of three nucleotides, called codons by tRNAs (transfer RNA). The tRNA contains an anticodon sequence on the base which binds to its respective codon on the mRNA. The anticodon is the reverse compliment of the codon which is the reverse compliment of the DNA strand; thus, the tRNA anticodon sequence matches the original DNA seqence, cool huh? The tRNA recognizes its sequence on one end and carries its AA (amino acid) molecule on the other in order to deliver the molecule to the growing AA strand. Thus, the genetic sequence is read and the AA molecule is assembled in the correct order.

Each position can contain one of the four nucleic acids (A, C, G, T/U), giving rise to 64 possible codons (`4^3`). Three of these codons signal for termination of AA production while the rest signal for the addition of one of the 20 AAs. Becasue there are only 20 AAs, one AA could be delivered by multiple tRNAs (where each tRNA recognizes a unique codon). But the number of codons/tRNAs is not the same for each AA. For example, Methionine is only delivered by one tRNA. In contrast, Arginine can be delivered by 6 different tRNAs.

Land et. al examined the number and distribution of tRNAs in 15,000 completed and draft assemblies on GenBank. They found that completed assembies had an average of 55 total tRNAs that represented on average 37 anticodons. The maximum number of unique anticodons identified per genome were 46 in the completed genome set and 47 in the draft genome set. The unrepresented anticodons were overwhelmingly those that started with A (the codon ends with U or T). They use the number of represented AAs (rather than anticodons) in their assessment of genome completion. A genome with fewer than 10 represented AAs was considered to be poor quality (Land, 2014). An assembly with fewer than 20 AAs may be missing genetic content or the annotations may be split accross fragments. Genomes often contain many tRNA genes for each AA, but an excessive number may indicate erronous duplicated content or multiple genomes.

According to Land et. a. 2015, the mathematical range of tRNAs in one organism is 20-62. The minimum of 20 ensures that the organism has at least one way of getting each AA. The maximum of 62 reflects the number of unique anticodons (Land, 2015). NOTE: I propose a different range: 21-64.  The minimum of 21 includes the 20 AAs and one tRNA to stop the AA elongation process. The maximum of 64 reflects the total number of anticodons because the three stop tRNAs recognize different codons. To be efficient, a genome would in theory need to have a number of tRNAs somewhere in this range.

However, biology is not exactly efficient. Land et. al. 2014 examined 30,000 prokaryotic genome sequences available in GenBank. They found a wide range in the number of tRNAs per completed and draft genomes. Note the minimum and maximum number of tRNAs found in complete (7; 173) vs. draft (0; 284) assemblies. 

Table: % of genomes with num tRNAs per genome
| Num. tRNAs | Complete | Draft |
| ---------- | -------- | ----- |
| 0-40 | 23 | 27 |
| 41-50 | 27 | 23 |
| 51-60 | 21 | 19 |
| 61-70 | 11 | 13 |
| 71-100 | 15 | 16 |
| > 100 | 3 | 1 |
| Statistics |
| Min | 7 | 0 |
| Max | 173 | 284 |
| Mean | 55 | 53 |
| N | 2,672 | 12,530 |
| SD | 19 | 20 |
Legend: Table reports the data in Table S5 of Land et. al 2014.



Table: % of genomes with num of unique anticodons represented
| Unique Anticodons | Complete | Draft |
| --- | --- | --- |
| 0-25 | 1 | 12 |
| 26-30 | 10 | 15 |
| 31-35 | 31 | 25 |
| 36-40 | 27 | 27 |
| 41-45 | 31 | 20 |
| > 45 | 0.07 | 0.06 |
| Statistics |
| Min | 0 | 0 |
| Max | 46 | 47 |
| Mean | 37 | 34 |
| N | 2,674 | 12,530 |
| SD | 5 | 8 |
Legend: Table reports the data in Table S6 of Land et. al 2014.

Note that in about 15,000 genomes, no genome either completed or in draft state represented more than 47 anticodons. It is also interesting that anticodons starting with 'A' (these are codons that end with 'U'/'T') were significantly under represented (not shown).


They consider a genome with fewer than 10 AA to be of poor quality.

## Identifier genes


## References (APA)
* Land, M. L., Hyatt, D., Jun, S. R., Kora, G. H., Hauser, L. J., Lukjancenko, O., & Ussery, D. W. (2014). Quality scores for 32,000 genomes. Standards in genomic sciences, 9(1), 1-10.
* Seemann, T. (2014). Prokka: rapid prokaryotic genome annotation. Bioinformatics, 30(14), 2068-2069.


