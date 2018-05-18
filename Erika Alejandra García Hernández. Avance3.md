## Erika Alejandra García Hernández 

### Avance 3

Hasta el momento ya instale **Samtools** por medio de docker hice el pull en bioconteiners. 

```
docker pull biocontainers/samtools

#El siguiente texto es lo último que me salio al hacer el pull y se ve que si se instaló la imagen 

Digest: sha256:6644f6b3bb8893c1b10939406bb9f9cda58da368100d8c767037558142631cf3
Status: Downloaded newer image for biocontainers/samtools:latest
```

También instale pindel

```
git clone git://github.com/genome/pindel.git
```

También descargue de **NCBI- GeneBanck** las secuencias de referencia de los genes que voy analizar 

```
curl -s "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgidb=nucleotide&rettype=fasta&id=179033,206725550,23491728,1518793,1732377" > secuenciasreferencia
```

Al correr este comando me crea un archivo pero  cuando hago un  head del archivo me sale este mensaje de error:  **{"error":"Invalid eutil name 'efetchdb=nucleotide&rettype=fasta&id=179033,206725550,23491728,1518793,1732377'","api-key":"189.206.137.178","type":"ip","status":"ok"}** 

#### Nota:

Hasta el momento no he podido analizar las secuencias, debido a que la secuenciación no se hizo en mi laboratorio y los archivos .bin no me los han entregado, pero me prometieron que sin falta mañana me los darán.  

Link al Readme 
https://github.com/EAlejandra/ProyectoFinalBioinf2017-II