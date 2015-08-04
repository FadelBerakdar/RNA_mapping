# NCBI 2nd Hackathon - RNA-seq Tutorial

RNA-seq data analysis relies on the alignment to the genome. With this tutorial, we outline the command-line basics to perform alignments with four different alignment algorithms: BLASTMapper, HISAT, STAR, and BWA. 

**short explanation of fundamental differences in alignment strategies

Each approach requires the construction of an index file. This file allows the algorithm to effeciently map reads to the genome.

### STAR
  Index file construction:
  ```BASH 
  STAR  --runMode genomeGenerate --runThreadN 24 --genomeDir GRC28_star --genomeFastaFiles ~/tan/genome/Homo_sapiens.GRCh38.dna_sm.chromosome.20.fa
  ```
<div style="background-color:rgba(0, 0, 0, 0.5); text-align:center; vertical-align: middle; padding:40px 0;">
<a href="/donate">DONATE</a>
</div>  
  
  Aug 03 21:35:40 ..... Started STAR run
  Aug 03 21:35:40 ... Starting to generate Genome files
  Aug 03 21:35:42 ... starting to sort  Suffix Array. This may take a long time...
  Aug 03 21:35:43 ... sorting Suffix Array chunks and saving them to disk...
  Aug 03 21:36:08 ... loading chunks from disk, packing SA...
  Aug 03 21:36:10 ... writing Suffix Array to disk ...
  Aug 03 21:36:10 ... Finished generating suffix array
  Aug 03 21:36:10 ... starting to generate Suffix Array index...
  Aug 03 21:36:33 ... writing SAindex to disk
  Aug 03 21:36:34 ..... Finished successfully


  Alignment:
  
  

### BLASTMAPER
  Index file construction:
  ```BASH
  makeblastdb -parse_seqids -dbtype nucl -title chr20 -out chr20 -in ../genome/Homo_sapiens.GRCh38.dna_sm.chromosome.20.fa
  ```
  
  
  Alignment:
  
  
### HISAT
  Index file construction:
  
  Alignment:
  
  
### BWA
  Index file construction:
  
  Alignment:
  
  
