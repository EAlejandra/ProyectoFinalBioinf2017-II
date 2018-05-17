# README 

This readme contain scripts for the analysis of genes related to prostate cancer, mainly analyze the CAG  repeated in the androgen receptor (AR) and identify  specific mutations in the other genes analyzed.   

### Prerequisites

For the analysis you need Install:

samTools

```
docker pull biocontainers/samtools
```

Script 1

```
## This script is for downloading 6 NCBI sequences of genes related to prostate cancer and that will be used as reference

# Create a directory to save the data
mkdir secuenciasreferencia 

# Download the NCBI sequences
curl -s "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgidb=nucleotide&rettype=fasta&id=179033,206725550,23491728,1518793,1732377" > secuenciasreferencia

# Check if the sequences are lowered 
grep ">" secuenciasreferencia


```

### 







