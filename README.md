# Comparación de LDA y QDA - Wine Dataset

Proyecto que investiga los fundamentos teóricos del Análisis Discriminante Lineal (LDA)
y Cuadrático (QDA), e implementa ambos modelos en Python usando el Wine Dataset de scikit-learn.

## Cómo ejecutar el proyecto

1. Abrir el archivo `LDA_QDA_Wine.ipynb` en Google Colab o Jupyter Notebook.
2. El dataset se descarga automáticamente desde scikit-learn con `load_wine()`, no requiere
   descarga manual.
3. Ejecutar las celdas en orden (Entorno de ejecución > Ejecutar todo, en Colab).
4. Requiere las librerías: pandas, numpy, matplotlib, seaborn, scikit-learn (incluidas por
   defecto en Google Colab).

## Principales hallazgos

- El Wine Dataset (178 observaciones, 13 variables químicas, 3 clases) es altamente separable
  mediante métodos discriminantes.
- LDA obtuvo un desempeño muy alto (accuracy, precisión, recall y F1-score cercanos a 1),
  generando fronteras de decisión lineales.
- QDA obtuvo métricas muy similares a LDA, con fronteras de decisión curvas, ya que permite
  una matriz de covarianza distinta por clase.
- La diferencia de desempeño entre ambos modelos fue marginal, lo que indica que el supuesto
  de covarianza compartida de LDA es razonable para este dataset tras estandarizar las variables.
- LDA resulta preferible por su simplicidad e interpretabilidad, mientras que QDA sería más
  útil en datasets donde las clases muestren covarianzas claramente distintas.

## Informe técnico
El informe técnico en PDF con la investigación teórica se encuentra en Google Drive: https://drive.google.com/file/d/1n6gIsEIbYNYyIs8RtgogMiiII7a-CUkF/view?usp=sharing
