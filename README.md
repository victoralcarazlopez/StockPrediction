# StockPrediction

Este proyecto supone el TFG del grado en Ingenieria del Software de Víctor A. Alcaraz López en la UPM (2022). El pdf de la memoria puede encontrarse dentro de la carpeta 'docs'. 

Se presentan dos modelos de predicción bursatil sobre las empresas del NASDAQ 100.

Se plantean dos modelos:
- Modelo 1: creación de una red neuronal (LSTM) y predicción individual sobre cada empresa y calculo del error medio cometido entre todas.
- Modelo 2: se crea un dataset con los datos de todas las empresas y se entrena una sola red neuronal (LSTM) para todas las empresas juntas

Para entrenar se utilizan los datos desde 2017 hasta 2022 (aproximadamente los últimos 5 años). Se reservan los datos del último mes de 2022 para validación.


Las libretas de este proyecto:
- Data_Collection.ipynb: mediante Tiingo obtenemos los datos de la cotización de las empresas y generamos los ficheros .csv sobre los que trabajaremos para hacer predicciones.
- Stock_Prediction-Model1(Individual).ipynb: recuperación de los datos desde los ficheros, preprocesamiento, entrenamiento y validación de el modelo implementado.
- Stock_Prediction-Model1(OneCompany_withGraphics).ipynb: identico que el anterior pero para una sola empresa (usado para generar gráficas de empresas)
- Stock_Prediction-Model2(All_Companies).ipynb: recuperación de los datos desde los ficheros, preprocesamiento, entrenamiento y validación de el modelo implementado.
- Results.ipynb: comparación los resultados obtenidos por ambos modelos.


Versiones del entorno desplegado: 
- Python - 3.9.11
- Tensorflow - 2.6.0
