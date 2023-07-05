
# Repositorio del Trabajo de Fin de Grado (TFG)

Este repositorio contiene todos los archivos y el código fuente utilizados en mi Trabajo de Fin de Grado (TFG). A continuación, se proporciona una descripción detallada de cada carpeta y archivo presente en el repositorio:

## Carpetas

### 1. DataSet
Contiene los conjuntos de datos originales utilizados en el estudio. Estos datos se utilizaron como base para los análisis y los modelos de predicción realizados. Esta carpeta está compuesta a su vez de subcarpetas correspondientes a cada empresa. Cada una de estas carpetas cuenta con archivos .csv referentes a los datos de cotización y capitalización diarios, así como datos trimestrales sobre balance, ratios, beneficios 
y flujo de fondos. 

### 2. Estacionariedad
Esta carpeta contiene los resultados del análisis de estacionariedad. Esencial para el preprocesamiento de datos en la modelización de series temporales, este análisis asegura que los datos cumplan con los supuestos necesarios para los modelos de predicción. En esta carpeta se encuentran los .xlsx donde se han almacenado los resultados del test ADF, junto al resto, antes y después de la conversión a estacionario. Asimismo encontramos los archivos .xlsx y .csv de los conjuntos de datos estacionarios.

### 3. Figuras TFG
Aquí se encuentran todas las figuras y gráficos generados durante el estudio. Estos gráficos ilustran los resultados y hallazgos clave obtenidos durante el análisis. El resto de gráficos no incluidos en la memoria del TFG se pueden encontrar en los notebooks de jupyter.

### 4. Hypertunning
Esta carpeta contiene los resultados del ajuste de hiperparámetros para la red LSTM. En ella encontramos los resultados preliminares para cuatro de las seis empresas estudiadas. De las otras dos decidimos quedarnos sólo con la mejor combinación en vez de generar los .xlsx, por eficiencia computacional. Sobre estos resultados se hicieron pequeñas modificaciones en busca de mayor eficiencia

### 5. Merged_Data
Esta carpeta contiene los datos originales que se han procesado y combinado para su análisis. Estos son los datos previos a los obtenidos en la carpeta de estacionariedad.

## Archivos Jupyter Notebook

### 1. Data_Processing.ipynb
Este es el cuaderno Jupyter que contiene el código para el procesamiento de datos. Contiene desde la importación de archivos de Merged_Data, hasta la creación de los indicadores financieros y la variable objetivo. Además se muestran los resultados del estudio de la estacionariedad y de valores atípicos. Se finaliza con la creación de retardos y una serie de visualizaciónes útiles que se incluyeron en la memoria del trabajo.

### 2. Models_Archivo_Final.ipynb
Este cuaderno Jupyter contiene el código para la construcción y evaluación de los modelos de aprendizaje automático. Incluye desde la aplicación de ACP y Lasso a nuestros conjuntos de entrada (aplicando una búsqueda en rejilla de los hiperparámetros para optimizarlos), las funciones auxiliares para dividir el set en entrenamiento y test, para el escalado y la reducción de dimensionalidad, la transformación de incremento porcentual a valor nominal y la creación de un dataframe (result_df) con la predicción y los valores reales nominales, así como la implementación de la red LSTM, XGboost, Random Forest y Regresión lineal, junto a la optimización de parámetros de los dos primeros 

## Otros Archivos
### 1. Resultados_Lasso_ACP.txt
En este archivo de texto se muestra la ejecución al aplicar el código para la reducción de dimensionalidad. Se muestra lo impreso por la terminal referente a las variables elegidas por Lasso sin y con retardos, y lo mismo para ACP.
### 2. FernándezdelAmoPablo_TFG.pdf
Memoria del TFG, en la que se muestra tanto el marco teórico del desarrollo del trabajo como los resultados obtenidos.

Si tienes alguna pregunta sobre este repositorio o el trabajo en general, no dudes en contactarme.

