# HAMRbox: A user-friendly adaptation of HAMR

## Overview
- HAMRbox is a box of selected tools that capture different parts of the pipeline tailored for the [High Throughput Annotation of Modified Ribonucleotides](https://github.com/GregoryLab/HAMR), abbreviated HAMR, developed by [Paul Ryvkin et al](https://rnajournal.cshlp.org/content/19/12/1684). HAMRbox aims to make the original method more accessible by automating the tedious pre-processing steps, allowing users to analyze RNA-seq data at an experiment scale. 
- HAMRbox is high-throughput and performs RNA-modification analysis at a bioproject scale. HAMRbox performs constitutive trimming of acquired reads using Trim-Galore, and makes use of STAR as the aligning tool which reduces runtime with a comparable robustness compared to TopHat2 as suggested in the original pipeline.


## Command Line Arguments and Description

| Command | Description |
| --- | --- |
| -o | \<project directory\> |
| -t | \<SRA accession list.txt or folder of raw fastq files\> |
| -c | \<filenames for each fastq.csv\>|
| -g | \<reference genome directory\> |
| -l | \<read length\> |
| -s | \<genome size in bp \> |
| -a | \[use TopHat2 instead of STAR\]|
| -b | \[Tophat library choice: fr-unstranded, fr-firststrand, fr-secondstrand\]|
| -A | \[use TopHat2 instead of STAR\]|
| -f | \[filter\]|
| -Q | \[HAMR: minimum qualuty score, default=30\]|
| -C | \[HAMR: minimum coveragem default=50\]|
| -E | \[HAMR: sequencing error, default=0.01\]|
| -P | \[HAMR: maximum p-value, default=1\]|
| -F | \[HAMR: maximum fdr, default=0.05\]|
| -m | \[HAMR model\]|
| -n | \[number of threads\]|
| -h | \[help message\]|
