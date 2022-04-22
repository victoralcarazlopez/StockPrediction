# StockPrediction

Este proyecto implementa una red neuronal recurrente LSTM que predice el valor bursatil las empresas del NASDAQ 100.

Se sigue un modelo generalista que no se especializa en la predicción de una sola compañia. Se entrena para cada empresa y despues se calcula el error promedio obtenido entre todas ellas.

Para entrenar utilizamos los datos desde 2017 hasta 2022 (aproximadamente los últimos 5 años). Se reservan los datos del último mes de 2022 para validación.


Las libretas de este :
- Data_Collection: mediante Tiingo obtenemos los datos de la cotización de las empresas y generamos los ficheros .csv sobre los que trabajaremos para hacer predicciones.
- Stock_Prediction: recuperación de los datos desde los ficheros, preprocesamiento, entrenamiento y validación de el modelo implementado.


Versiones del entorno desplegado: 
- Python - 3.9.11
- Tensorflow - 2.6.0
