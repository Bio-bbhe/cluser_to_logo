# cluser_to_logo
Parse a SSN file and make sequence logo for each cluster

cluster_parser.py parses network file generated by mmseq2
```
optional arguments:

  -i , --input_tsv
  Network file generated by mmseq2, in general, it is a .tsv file
  
  -fasta , --fasta_file 
  Original protein fasta file used for clustering, e.g.,/data/test.fasta
  
  -node , --node_num
  Minimal number (included) of nodes in a cluster
  
  -o , --outdir
  A path to save all files. e.g., data/output
```  
  
makelogo.py performs sequence alignment and then generate logo sequence .svg file to
display sequence biases

optional arguments:
```  
  -i , --input_fasta
  Folder contains to-be-processed protein or nucleotide sequence files, e.g., /data/protein/
  
  -o , --outdir
  A path to save all files, including .aln alignment file and .svg/.png seq log file. e.g., data/output
  
  -n , --num_threads
```
**E.g., below is the SSN of small peptide**
![image](https://github.com/Bio-bbhe/cluser_to_logo/assets/82441159/062373d3-6d75-4fdd-8107-3d9e10045c85)
**seq_logo of the first cluster is:**
![Picture2](https://github.com/Bio-bbhe/cluser_to_logo/assets/82441159/095c8ede-c9a5-4fc3-9401-9454a094902a)



