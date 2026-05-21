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

## Características de la base de datos

La base de datos utilizada contiene información molecular y clínica de pacientes diagnosticados con cáncer pancreático pertenecientes al cohorte **GDC TCGA Pancreatic Cancer (PAAD)**.

Los archivos principales utilizados incluyen:

- `TCGA-PAAD.star_tpm.tsv`: matriz de expresión génica RNAseq tipo STAR-TPM, donde cada fila representa un gen y cada columna corresponde a una muestra de paciente.
- `TCGA-PAAD.clinical.tsv`: variables clínicas asociadas a los pacientes, incluyendo información demográfica y características clínicas relevantes.
- `TCGA-PAAD.survival.tsv`: información relacionada con supervivencia y seguimiento clínico de los pacientes.
- `gencode.v36.annotation.gtf.gene.probemap`: archivo de mapeo utilizado para relacionar identificadores génicos con nombres de genes interpretables.

La base de datos contiene miles de variables génicas de alta dimensionalidad, por lo que fue necesario aplicar técnicas de filtrado, escalamiento y reducción de dimensionalidad para facilitar el análisis e interpretación de los datos.

## Archivos incluidos

- [Reporte en formato ipynb](./P%20P3.%20Aprendizaje%20no%20supervisado.ipynb)
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
