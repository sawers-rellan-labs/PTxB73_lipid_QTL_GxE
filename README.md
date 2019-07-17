# Overlap with biparental phospholipid metabolism GxE QTLs.

[![DOI](https://zenodo.org/badge/193750474.svg)](https://zenodo.org/badge/latestdoi/193750474)

We looked for the GxE interaction QTLs for phospholipids in a B73 x Palomero Toluqueño (a highland landrace from the Central Plateau of Mexico ) BC1S5 Backcross Introgressed Line mapping population made of 87 individuals and genotyped using DARTseq. The mapping population was grown in a highland site in Metepec, Edo de Mexico at 2600 masl during the Summer of 2016 and in Puerto Vallarta, Jalisco at 50 masl during the winter of 2016/17. We collected samples from tip of the second youngest leave above the last leave with a fully developed collar at V4-V6 developmental stages. Samples were extracted according to We analyzed the samples using UHPLC-QTOF and 67 leaf lipid species were identified. Individual levels of each lipid were used for QTL analysis. We also used as phenotypes the sum total of the following lipid classes: diglycerides (DGs), triglycerides (TGs), phosphatidylcholines (PCs) and lysophosphatidylcholines (LPCs). Furthermore, we also included the log base 2 transformed ratios of LPCs/PCs and the ratios of the species with the most negative significant correlation ( t-test, p \< 1e-10) and at least 300 observations in the data (see table). Full details can be found in (paper to be published).

We then used a single QTL model with site (Metepec-Puerto Vallarta) as interaction covariate (function scanone from the R/qtl package, [^1^], and established genomewide significance LOD at alpha = 0.05 with 10000 replicates of the model with randomized phenotypes. This biparental GxE interaction QTLs were then used as a fixed set for testing the statistical significance of the overlap with the GxE GWAS intervals. This last interval set was permuted 10000 times, and the overlap count distribution and p-values were calculated for all QTL phenotype pairs using R Bioconductor package regioneR [^2^]. False discovery rate FDR values were calculated as the Benjamini Hochberg adjusted p-values using the function p.adjust, hypothesis with FDR \< 0.05 were rejected. Analysis scripts are available at [https://github.com/faustovrz/PTxB73_lipid_QTL_GxE]{.underline}.

### Results

We found interaction QTLs for phospholipid metabolites in the PTxB73 cross (see figure upper panel). In particular we found interaction QTLs for total phosphatidylcholines, total lysophosphatidylcholines, and the ratio of PCs/LPCs expressed as fold change. There was GxE QTLs for different specific phosphatidylcholines, lysophosphatidylcholines and a triglyceride (TG-52:4), and also for 2 metabolite ratios LPC-18:2 / PC-36:3 and PC36:4 / TG-52:6. Two single PC species PC-35:2 and PC-36:4, and the ratios LPC-18:2 / PC-36:3 and PC-36:4 / TG-52:6 had a significant overlap with either, cob weight, DTA, grain weight and field weight. No significant overlap between B73xPT RILs QTLxE and GWAS intervals was found for PCs, LPCs, or LPCs/ PCs ratio.

References

1. Broman, K. W., Wu, H., Sen, S. & Churchill, G. A. R/qtl: QTL mapping in experimental crosses. Bioinformatics 19, 889-890 (2003).

2. Gel, B. et al. regioneR: an R/Bioconductor package for the association analysis of genomic regions based on permutation tests. Bioinformatics 32, 289–291 (2016).
