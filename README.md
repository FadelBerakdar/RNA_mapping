# NCBI 2nd Hackathon - RNA-seq Tutorial

RNA-seq data analysis relies on the alignment to the genome. With this tutorial, we outline the command-line basics to perform alignments with four different alignment algorithms: BLASTMapper, HISAT, STAR, and BWA. 

**short explanation of fundamental differences in alignment strategies

Each approach requires the construction of an index file. This file allows the algorithm to effeciently map reads to the genome.

### BLASTMAPER
  ####Index file construction:
  ```
  makeblastdb -parse_seqids -dbtype nucl -title chr20 -out chr20 -in ../genome/Homo_sapiens.GRCh38.dna_sm.chromosome.20.fa
  ```
  
  
  #### Alignment:
  
  
### HISAT
  #### Index file construction:
  
  #### Alignment:
  
  
### STAR
  #### Index file construction:
  
  #### Alignment:
  
  
### BWA
  #### Index file construction:
  
  #### Alignment:
  
  
