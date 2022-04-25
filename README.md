# comboSC-mut
A pipeline for gene mutation identification from single-cell RNA-sequencing

## 1. Introduction

comboSC-mut is a pipeline based on [SCmut](https://github.com/nghiavtr/SCmut/projects)
, which is used to provide more information for the selection of treatment stretegy in comboSC. SCmut is a novel and robust statistical method for cell-level somatic mutation detection from single-cell RNA-sequencing. SCmut requies RNA-sequencing data of single cells and bulk-cell DNA-sequencing (e.g whole exome sequencing - WES) of matched samples (tumor and normal). If the DNA-sequencing data are not available, the list of somatic mutations can be used.

Software requirements for SCmut:

SCmut
Java 1.8 or higher

R 3.2 or higher

Samtools 1.3 or higher

Picard 2.3 or higher

VarScan 2.3.7 or higher

GATKAnalysisTK 3.6 or higher

## 2. Usage
### 2.1 Create a file named "comboSC-para", containing the following parameters:fasta, dbsnp, known_Mills_indels, known_1000G_indels.

#### example
fasta="/home/zhouchi/pTuneos/database_backup/Fasta/human.fasta"
dbsnp="/home/zhouchi/pTuneos/database_backup/VCF_annotation/dbsnp_138.hg38.vcf.gz"
known_Mills_indels="/home/zhouchi/pTuneos/database_backup/VCF_annotation/Mills_and_1000G_gold_standard.indels.hg38.vcf.gz"
known_1000G_indels="/home/zhouchi/pTuneos/database_backup/VCF_annotation/1000G_phase1.indels.hg38.sites.vcf.gz"

### 2.2 run code:
`bash SCmut.R`


