# RNAScope-Ancestry_Study
Scripts for RNAScope Study 

This repository contains the main scripts used in the preparation of our RNAScope Ancestry paper.  

The first script covers the process of taking paired end data, cleaning with TRIM-Galore and aligning with our STAR/ Bowtie2 pipeline. Subsequent data are merged, sorted and then quantified in Stringtie2.  

The second script covers the GATK pipeline to extract SNV data from the RNA seq data. The pipeline focuses on teh STAR aligned data only to avoid a clash of cigar scores, per GATK best practices.  The original script was designed such that if you have a sample ran on multiple flowcells, they are processed separately, and then combined prior to haplotype caling. 

Raw data will be posted in dbGAP.  Raw data sheets are available on request, but they contain sensitive data hence they are not available on an open basis in alignment with our participant consent form.  



