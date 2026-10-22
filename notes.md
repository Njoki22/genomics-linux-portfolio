# Data notes
Date started: 2026-10-20

## Reference genome
Organism: Escherichia coli B str. REL606
Accession: NC_012967.1 (assembly GCF_000017985.1)
Sequences: 1
Length: 4,629,812 bases
GC content: 50.77%

## Sequencing reads
Run: SRR2584863 (study PRJNA295606, sample SAMN04096083, REL7179B)
Platform: Illumina HiSeq 2500, paired-end
MD5 _1: 4a1529a4165970302d6d8cb50b6e7a43
MD5 _2: 33492a66dcc95c3f8fc847b41d2c8ceb

## FASTQ Read Audit 
Data type : Paired-end sequecning reads
Files : SRR2584863_1.fastq.gz and SRR2584863_2.fastq.gz
## File Inspection
Command: ls -lh to inspect the sequencing files and their sizes 
## File Intergrity 
Command: md5 SRR2584863_1.fastq.gz SRR2584863_2.fastq.gz -  checksums to check whether the downloaded files match the expected ENA values md5 SRR2584863_1.fastq.gz SRR2584863_2.fastq.gz - command run 
- Read 1: `4a1529a4165970302d6d8cb50b6e7a43`
- Read 2: `33492a66dcc95c3f8fc847b41d2c8ceb`

### FASTQ Structure
 
Command: gzcat SRR2584863_1.fastq.gz and head -n 8
         gzcat SRR2584863_2.fastq.gz | head -n 8 
Each FASTQ read contained four lines 
1. Read identifier beginning with @.
2. DNA sequence.
3. Separator beginning with +.
4. Quality scores, one character per base.

### Read Counts
 
Commands used:
gzcat SRR2584863_1.fastq.gz | wc -l
gzcat SRR2584863_2.fastq.gz | wc -l

Results:
Read 1: 6213036 lines 
Read 2: 6213036 lines 
Reads per file: 6213036 / 4 = 1553259 

### Read Length 
Command: echo "465977700 / 1553259 / 2" | bc
Read length: 150 bases per read 
