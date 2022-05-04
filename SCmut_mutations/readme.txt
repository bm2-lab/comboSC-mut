This folder contains cell-level mutation calls from SCmut with fdr2d < 0.2 of three patients in binary matrices: 
- BC03 (breast cancer): includes BC03_tumor_mutations.txt for primary tumors and BC03_LymphNode_mutations.txt for lymph node
- BC07 (breast cancer): includes BC07_tumor_mutations.txt for primary tumors and BC07_LymphNode_mutations.txt for lymph node. It is noting that we discovered no mutation calls (with fdr2d < 0.2) from this patient 
- SF10282 (glioblastoma): in SF10282_mutations.txt

Each row of the matrix indicates to one mutation, the rowname is in format "chr_position_genename"
Each column of the matrix present a single cell
The value at position (i,j) of mutation i from cell j is a binary value: 0 is no mutation, 1 is mutation with fdr2d < 0.2