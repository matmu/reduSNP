reduSNP
=======
LD pruning tool

Introduction
------------
reduSNP is a lightweight linkage disequilibrium (LD) pruning tool that is highlighted by its minimum to no pre-processing of input information. It can handle large sets of SNPs with different LD threshold and uses the latest European ancestry Phase 3 release of the 1000 Genomes Project reference population, addressing prior LD-pruning tool 'shortcomings'.

Installation
-------------
Required software
TODO

Parameters
---------------
```~/redusnp.pl <input_file> <output_file> <pop> <ld_method> <corr_threshold>```

\<input\_file\> Tab-separated file with a column "SNP" contain reference SNP identifier (rsID)

\<output\_file\> Filename of the output file

\<pop\>  Currently, only the European population (specify as "EUR") of 1000 Genomes Phase 3 is supported

\<ld\_method\> Method that is used to calculate LD; either r^2 or D' (specifiy as "r2" or "dprime")

\<corr\_threshold\\> correlation threshold, number between 0 and 1, specified LD threshold(s)

Example command
---------------
```~/redusnp.pl input.txt output.txt  EUR r2 0.8```
