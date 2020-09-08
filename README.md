# Trabajo de Fin de Máster

## Estructura
Este repositorio contiene el script y los documentos de interés que están referenciados en el apartado "Anexos" en el Trabajo de Fin de Máster del Máster en Bioinformática por la Universidad de Murcia.
Dicho trabajo se titula: "Estudio de alteraciones genéticas en la ruta de la N-glicosilación y su implicación en el desarrollo de cardiopatías congénitas a través de secuenciación masiva y análisis bioinformático."

Este repositorio contiene las siguientes carpetas:

- Script: en ella se encuentra el script, en formato RMarkdown (.rmd) denominado "AnalisisVariantes". Ha sido utilizado para el análisis de variantes en controles y pacientes con cardiopatía congénita. Genera diversos XLSX para el análisis de resultados a partir de ficheros XLSX con la información de cada uno de los pacientes. Adicionalmente, se encuentran dos ficheros HTML obtenidos desde RMarkDown, uno para cada conjunto de muestras (casos y controles).
- Ficheros: consta de dos carpetas: "Casos" y "Controles". En ellas, se encuentran los ficheros XLSX obtenidos con el script en homocigosis y heterocigosis, de la totalidad de las variantes de pacientes y controles. 

## Librerías

Para ejecutar el script, se necesitan los siguientes paquetes, disponibles en CRAN.

- readxl
- dplyr
- writexl
- tidyr
- stringr

## Ficheros XLSX
Las columnas de los ficheros contienen la siguiente información:

- Sample: nombre de la muestra.
- Gene: nombre del gen.
- Variant: representa la variante del gen, donde se muestra el alelo de referencia y el genotipo diploide para la muestra: "Referencia>AleloA/AleloB".
- Chr: cromosoma en el que se encuentra el gen.
- Coordinate: ubicación de la variante en el genoma.
- Transcript: nombre del transcrito, generalmente un identificador de base de datos de RefSeq o Ensembl.
- Consequence: efecto que puede tener esa variante en la transcripción, descrita en el vocabulario estandarizado de Sequence Ontology.
- Protein-Position-AminoAcids: posición del aminoácido en la proteína y el cambio que se ha producido de qué aminoácido o aminoácidos.
- SIFT: puntuación de la herramienta SIFT.
- PolyPhen: puntuación de la herramienta PolyPhen.
- dbSNP-ID: es una etiqueta de identificación asignada por el NCBI a un grupo de SNP (o grupo) de SNP que se asignan a una ubicación idéntica. dbSNP contiene variaciones de un único nucleótido humano, microsatélites e inserciones y deleciones a pequeña escala junto con la publicación, frecuencia de población, consecuencia molecular e información de mapeo genómico y RefSeq para variaciones comunes y mutaciones clínicas.
- ExACFreqNfe: frecuencia alélica de la variante en la base de datos ExAC de población no finesa.
- Significance: importancia clínica o clasificación asignada al alelo según la base de datos ClinVar.

Las abreviaturas "Het" y "Hom" corresponden a "heterocigosis" y "homocigosis", respectivamente.

