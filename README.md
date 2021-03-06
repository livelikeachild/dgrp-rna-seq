# Codes for DGRP RNA-Seq analyses

This repository contains various codes to perform the RNA-Seq analyses for the DGRP as described in the manuscript (add link). The majority of the these codes are authored by first author Dr. Logan J Everett (now at US EPA) while a postdoctoral fellow in Dr. Trudy Mackay's lab at NC State University. We note that most of these codes are specific to the computing cluster at NC State. That being said, they are mostly scripts of commands using existing softwares and thus can be adapted to other environments. The purpose of the repository is to provide a documentation of specific strategies and parameters used in the specific analyses. Additional details can also be found in the manuscript describing the results.

There are three major steps, 1) alignment of RNA-Seq reads to the reference genome and estimation of gene expression; 2) quantitative genetic anaysis; and 3) eQTL mapping.

## Alignment and gene expression estimation

The complete set of commands is in the file [commands.sh](alignment/commands.sh). This script uses other commands in the directory [tools/](tools/)

## Quantitative genetics of gene expression

The complete set of commands is in the file [known_novel_genes_analysis.sh](quant_genet/known_novel_genes_analysis.sh). 

## eQTL mapping

The eQTL mapping uses PLINK and summarizes results (calculating empirical FDR) using [empFDR.R](eqtl/empFDR.R). The results are further refined by a forward model selection implemented in [modelSelect.bash](eqtl/modelSelect.bash).

## Characterization of NTR

Scripts and commands in the directory [ntr](ntr/)
