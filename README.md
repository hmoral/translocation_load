# translocation_load

This repo include SLiM3 v3.4 (Haller and Messer, 2019) code to replicate our simulations of the genetic load and genetic diversity outcomes of translocating individuals under different sampling regimes to investigate the effect of the recommendation from Scott et al. (2020) of translocating only the most genetically diverse indivudals.

- Random: indivduals are selected at random from the metapopulation
- Diversity: individuals among the higest 20% of nucleotide diversity are selected
- Load: individuals among the bottom 20% of genetic load are selected (Genetic load = the sum of selection coefficients in homozygous condition plus the sum of selection coefficients multiplied by their dominance coefficients in heterozygous condition)
- We simulated a 1Mb chromosome with a mutation rate = 1e-7 and recombination rate = 1e-8. The ratio of deleterious to neutral mutations is 0.2:1. 
- First, four populations of variable Ne (50, 100, 500 and 1000) accumulate mutations for 5000 generations (burn-in), followed by individuals selection to be translocated to an admixed population were they mate randomly. 

## References:
Haller, B. C., & Messer, P. W. (2019). SLiM 3: forward genetic simulations beyond the Wright–Fisher model. Molecular biology and evolution, 36(3), 632-637.<br/>
Scott, P. A., Allison, L. J., Field, K. J., Averill-Murray, R. C., & Shaffer, H. B. (2020). Individual heterozygosity predicts translocation success in threatened desert tortoises. Science, 370(6520), 1086-1089.

## Dependencies
The only dependency is SLiM 3.4 or higher. The code has not been tested with the most recent version of SLiM 3.5 which introduce syntax changes that might not be back-compatible with this code.<br/>
SLiM software can be found in: https://messerlab.org/slim/
