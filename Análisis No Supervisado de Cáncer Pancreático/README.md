# P P3. Análisis No Supervisado de Cáncer Pancreático

En este proyecto se desarrolla un análisis de aprendizaje no supervisado aplicado a datos reales de expresión génica relacionados con cáncer pancreático. El objetivo principal es identificar patrones moleculares y posibles agrupaciones de pacientes utilizando técnicas de reducción de dimensionalidad y clustering, además de explorar la relación entre dichas agrupaciones y variables clínicas relevantes.

El análisis se realizó utilizando datos del cohorte **GDC TCGA Pancreatic Cancer (PAAD)** obtenidos mediante la plataforma **UCSC Xena**, trabajando específicamente con datos de expresión génica RNAseq tipo **STAR-TPM**, información clínica y datos de supervivencia. :contentReference[oaicite:0]{index=0}

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

- [Reporte en formato ipynb](./P%20P3.%20Aprendizaje%20no%20supervisado.ipynb)
- [Reporte en formato html](./P%20P3.%20Aprendizaje%20no%20supervisado.html)

## Archivos de datos utilizados

- `TCGA-PAAD.star_tpm.tsv`
- `TCGA-PAAD.clinical.tsv`
- `TCGA-PAAD.survival.tsv`
- `gencode.v36.annotation.gtf.gene.probemap`

## Fuente de los datos

- TCGA vía UCSC Xena:
https://xenabrowser.net/datapages/
