# PG-CdBG

PG-CdBG is an application of the succinct colored de Bruijn graph constructed by  [VARI-merge](https://github.com/cosmo-team/cosmo/tree/VARI-merge). It overcomes the complexity of graphs and organize a set of species- or population-specific haplotype sequences of interest. Based on this model, three main works have been achieved.
1. VARI-cSupB:A directed acyclic graph can be decomposed as colored superbubbles and reoganized by their relationships. Then a tri-tuple coordinate system that combines an offset value, topological structure and sample information. Moreover, VARI-cSupB can adapt to a complex cycle structure.
2. VARI-MSA: It provides a novel method that utilizes complete topological information to achieve mutiple sequences alignment.
3. VARI-AF: Firstly, it provides a novel method that utilizes complete topological information and efficiently detects variants for highly similar samples, which can be validated by simulated datasets. Secondly, it output all the basis weight matrix which can be used to calculate kinships of samples.
# Installation
VARI-cSupB is based on the colored de Bruijn graph constructed by [VARI-merge](https://github.com/cosmo-team/cosmo/tree/VARI-merge), so the installation processing is the same as the VARI-merge. We only need to add the files to VARI-merge's main directory.

# Usage
The construction of graph and color matrix can be seen  [VARI-merge](https://github.com/cosmo-team/cosmo/tree/VARI-merge).To obtain the coordinate system or variants, simply use the command line as follows:<tab>
```
VARI-cSupB primates_mtDNAs_kmc_list.dbg primates_mtDNAs_kmc_list.colors.sd_vector >log1
VARI-MSA primates_mtDNAs_kmc_list.dbg primates_mtDNAs_kmc_list.colors.sd_vector >log2
VARI-AF primates_mtDNAs_kmc_list.dbg primates_mtDNAs_kmc_list.colors.sd_vector >log3
```
