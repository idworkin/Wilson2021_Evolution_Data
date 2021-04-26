# README

This README file explains the data files and associated R scripts associated with the forthcoming paper:
Wilson, AE. Siddiqui, A and I. Dworkin. 2021.Spatial heterogeneity in resources alters selective dynamics in Drosophila melanogaster
Accepted at Evolution.

Currently available as a pre-print version on [biorxiv](https://www.biorxiv.org/content/10.1101/2020.09.05.283705v1)


## data

there are three csv files associated with this study.

**AW_Allele_purge_counts.csv**

This file contains the genotypic frequencies for the primary allele purging experiment. Variable names are as follows
mutant_type: The mutant allele (bw, y, f, vg, w, px)

generation: generation of allele purging experiment

treatment: Spatial treatment for allele purging experiment. (SCT, UCT, NT)

replicate: Replicate lineage of experimental evolution (for allele purging). Nested within mutant_type and treatment.

wt_male: counts of male individuals showing wild type morphology (but could be genotypically het)

mutant_male: counts of male individuals showing mutant morphology

ditto for female columns.


**AW_Allele_purge_true_freq_counts.csv**

This file contains the genotypic frequencies from experimental crosses for the primary allele purging experiment. These were done to accurately assess genotypic frequencies.

Variable identifiers as above, but with the following differences:

homo_wt: number of female parents who are inferred to be homozygous for wild type allele based on progeny phenotypes.

hetero_wt: number of female parents who are inferred to be heterozygotes based on progeny phenotypes.

mutant: number of females (of the 50 counted) who were homozygous for mutant allele. These females did not need to be crossed to experimental males (since genotype was known).

q: allele frequency of mutant allele based on the experimental cross data.

**AW_Allele_purge_2_counts.csv**

This is the dataset for the second allele purging experiment. All variable names are the same as in AW_Allele_purge_counts.csv. Note however that there are two additional levels of Treatment (NC = no choice or "vial no choice" in the paper, PNT = an old term we used, but in the study this is "vial choice", in other words, with mate choice)


## scripts

**AW_Allele_purge1_6_mutants.Rmd** This script contains the code to replicate all of the main analyses for the paper for the first allele purging experiments with the 6 deleterious alleles.

**AW_Allele_purge1_singlematepairings.Rmd** this contains the code to replicate the analyses from the experimental crosses. This also has the analyses confirming that the populations are in Hardy Weinberg Equilibrium.


**AW_Allele_purge2_2_mutants.Rmd** This script contains the code to replicate analyses for the second allele purging experiment with the 2 alleles.
