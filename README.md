# DBD in the EMP dataset

1. Construct_fasta_per_sample.py : builds Fasta files from the EMP summary file. 

2. dbd_analys_input.py : for every sample, it associates the taxonomic annotations of all the ASVs it contains. 

3. glmm_analys_input.py : uses the output of dbd_analys_input.py to estimate diversification rate for every taxonomic ratio   (ASV:Genus, Genus:Family, Family:Order, Order:Class and Class:Phylum), as well as diversity (the number of non-focal lineages: non focal phyla, classes, orders, families and genera numbers).

4. percentidentity.py : clusters ASVs by different percent identity using USEARCH.

5. figure4.r : plot the figure 4 using GLMMs output (1: glmm with the interaction between diversity and biome as fixed effect to predict diversification (supplementary, file1, section 5), and 2: the GLMM of the genome size analysis (supplementary, file1, section 5)


