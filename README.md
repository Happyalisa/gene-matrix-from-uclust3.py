# gene-matrix-from-uclust3.py
#Theo Allnutt, 2016 
#script to parse the uclust .uc file and make a table of clusters with their %identity 
#usage: gene-matrix-from-uclust2.py clusters_sorted.uc pangenome.txt 60 -cds- 
#60 is the identity threshold below which presence of a gene is not scored 
#'-cds-' is the chosen delimiter between genome file names and the cds locus number 
#e.g. input cds fasta file to usearch has headers like this: 
#>genome1-cds-_001 
#.e.g using prokka to make fasta file: prokka --fast --force --outdir prokka --prefix genome1 --locustag  genome1-cds- --cpus 0 --metagenome --mincontiglen 200 genome1.fasta
