# P P3. Análisis No Supervisado de Cáncer Pancreático

En este proyecto se desarrolla un análisis de aprendizaje no supervisado aplicado a datos reales de expresión génica relacionados con cáncer pancreático. El objetivo principal es identificar patrones moleculares y posibles agrupaciones de pacientes utilizando técnicas de reducción de dimensionalidad y clustering, además de explorar la relación entre dichas agrupaciones y variables clínicas relevantes.

El análisis se realizó utilizando datos del cohorte **GDC TCGA Pancreatic Cancer (PAAD)** obtenidos mediante la plataforma **UCSC Xena**, trabajando específicamente con datos de expresión génica RNAseq tipo **STAR-TPM**, información clínica y datos de supervivencia.

Durante el desarrollo del proyecto se realizaron procesos de preparación y tratamiento de datos, incluyendo:

- Mapeo de identificadores génicos
- Tratamiento de genes duplicados
- Filtrado de genes de baja variabilidad
- Escalamiento y normalización de datos
- Reducción de dimensionalidad mediante **PCA**

Posteriormente, se implementaron y compararon modelos de clustering utilizando algoritmos como:

- **K-Means**
- **Clustering jerárquico**

Además del análisis de agrupamiento, se realizó una interpretación molecular y clínica de los clusters obtenidos, incluyendo comparación de expresión génica, identificación de genes diferenciadores y análisis descriptivo de variables clínicas y de supervivencia.

Durante el desarrollo se utilizaron bibliotecas de Python orientadas a ciencia de datos, bioinformática y aprendizaje automático, incluyendo **pandas**, **NumPy**, **matplotlib**, **scikit-learn**, **SciPy** y **statsmodels**.

## Archivos incluidos

- [Descargar reporte en formato ipynb](./P%20P3.%20Aprendizaje%20no%20supervisado.ipynb?raw=1)
- [Reporte en formato html](./P%20P3.%20Aprendizaje%20no%20supervisado.html)

## Archivos de datos

Este proyecto utiliza archivos de datos externos obtenidos desde UCSC Xena para el cohorte **GDC TCGA Pancreatic Cancer (PAAD)**. Debido al tamaño del archivo principal de expresión génica, `TCGA-PAAD.star_tpm.tsv` no se incluye directamente en el repositorio. En su lugar, se proporciona la fuente oficial para su descarga.

### Archivos incluidos en el repositorio

- [`TCGA-PAAD.clinical.tsv`](./TCGA-PAAD.clinical.tsv)
- [`TCGA-PAAD.survival.tsv`](./TCGA-PAAD.survival.tsv)
- [`gencode.v36.annotation.gtf.gene.probemap`](./gencode.v36.annotation.gtf.gene.probemap)

### Archivo no incluido por tamaño

- `TCGA-PAAD.star_tpm.tsv`

Este archivo puede descargarse desde UCSC Xena seleccionando el cohorte **GDC TCGA Pancreatic Cancer (PAAD)** y el dataset de expresión génica RNAseq tipo **STAR-TPM**.

Fuente: [UCSC Xena](https://xenabrowser.net/datapages/)
