**#Genetic Potential and Phenotypic Switching**

This repository contains the code implementation and extension of the single loci model presented in the paper "Evolution of Genetic Potential" by Meyers et al (2005). The authors highlighted how the genetic potential of a species influences phenotypic switching in response to changing environments. Our project aims to expand their model and investigate how frequency distributions of alleles and genotypes may change using a two-loci model and how introducing a recombination parameter affects the allele frequencies.

**#Implementation**

We began by assuming two loci, L1 and L2, each with 5 alleles (g0,g1,g2,g3,g4) and (h0,h1,h2,h3,h4) respectively. We used the fitness equations to determine the fitness for each of the possible 25 genotypes. Then, we ran a simulation for a defined number of generations while tracking the allele frequencies over time.

We found that the two-loci model produced similar results to the single-loci model. For relatively stable environments, the population alternates between genetic robustness for phenotype A and mutation-selection balance around the single allele for phenotype B. At intermediate fluctuation rates, mutation between the two phenotypes occurs frequently due to genetic potential. For highly variable environments, the population converges on phenotype V, which corresponds to organismal flexibility. The allele for both phenotypes tolerates the two conditions EA or EB but neither does exceptionally well.

**#Extension**

To understand how crossing over could influence frequency distributions over generations, we added a recombination parameter to the simulation. We assigned randomly selected recombination values to each of the 5 alleles (ensuring that all values sum to 1) and ran the simulation using the two-loci model.

We found that alleles for phenotype A performed consistently well in stable environments and even in highly variable environments due to the nature of the environment existing in state A where these are beneficial phenotypes. For alleles of phenotype V and B, we observed a drop in allele frequency in highly variable environments. We observed that the allele frequencies increased to nearly the initial frequencies observed in the highly fluctuating region for intermediate fluctuating environments. For relatively stable environments, the allelic frequencies for V and B decreased again. These results are in line with what would happen to deleterious or intermediate phenotypes in environment A. For environment B, we observed that the deleterious phenotype (in this case A), and the frequency of their corresponding alleles decreased. We observed that except for the highly variable regions, the allelic frequency for the beneficial phenotype increased as expected due to the environment being B. Surprisingly, the alleles with the highest representation are of phenotype B, depicting the occurrence of organismal flexibility.

**#References**

Meyers LA, Ancel FD, Lachmann M. Evolution of genetic potential. PLoS Comput Biol. 2005 Aug;1(3):236-43. doi: 10.1371/journal.pcbi.0010032. Epub 2005 Aug 26. PMID: 16158095; PMCID: PMC1193991.
