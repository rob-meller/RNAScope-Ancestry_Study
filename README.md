# RNAScope-Ancestry_Study
Scripts for RNAScope Study in collaboration with Dr R Verma.

This repository contains the main scripts used in the preparation of our RNAScope Ancestry paper.  

The first script covers the process of taking paired end data, cleaning with TRIM-Galore and aligning with our STAR/ Bowtie2 pipeline. Subsequent data are merged, sorted and then quantified in Stringtie2.  

The second script covers the GATK pipeline to extract SNV data from the RNA seq data. The pipeline focuses on teh STAR aligned data only to avoid a clash of cigar scores, per GATK best practices.  The original script was designed such that if you have a sample ran on multiple flowcells, they are processed separately, and then combined prior to haplotype caling. 

Raw data will be posted in dbGAP.  Raw data sheets are available on request, but they contain sensitive data hence they are not available on an open basis in alignment with our participant consent form.  

The first script is based on the Ion Torrent platform software approach for aligning data.  The GATK pipeline was developed with scientists from the COVIRT project specifically Drs Shashwat Nagar, I King Jordan, and Amanda Savaria-Butler. From their original scripts I modified it for the RNA seq dataset here.  Of note if using Ensembl references please check chr edits, and there are some characters that are not accepted in some chromosomes vcfs.    

