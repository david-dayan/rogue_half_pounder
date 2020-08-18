###################################################
############# Genotype Files Readme ###############
###################################################

###### file suffix log

0.1: Raw, unfiltered GTs including all controls and replicates  
0.2: Raw, unfiltered GTs, replicates and controls removed  
0.3: filtered for IFI, GTperc (inds), and Missingness (loci) > 20%  
0.4: filtered for IFI, GTperc (inds), and Missingness (loci) > 20%, and allele correction issues  
1.0: 0.4 + removed monomorphic  
2.0: 1.0 + duplicate sample removal  
2.2:  final genotype dataset with metadata (population, run, sample date) 
bug: data from genotyper script with a bug in it (over calls NA)

###### readme

This project used two lanes of data, an initial analysis used on the first lane, then 
extra individuals were added, the final analysis uses both lanes

- Omy_Rogue2018-19half-pounders-baseline_307snps_genotype-table.xlsx : first lane genotypes fully filtered 
- genind_2.0.R : final filtered genind object (adegenet)
- genotypes_2.2.R : r object for the 2.2 (final filt with metadata) genotypes
- gtseq_marker_summary.txt: subset of marker info (used in run 1.0 scripts)
- half_pounder_GTs_0.1.csv : raw genotype output from GTseq pipeline
- half_pounder_GTs_0.1_bug.csv : raw genotype output from GTseq pipeline
- just_genos.txt : genotypes formatted for coancestry
- marker_info.txt : marker x individual information from 0.1 dataset (concatenation of .genos)
- marker_info_bug.txt
- prefiltered_genotypes.csv
- relatedness.Rdata : r object for duplicate id