# Fraud-Detection-Neural-Network

## Detección de fraudes con Redes Neuronales Artificiales

Este proyecto fue realizado para la materia de Redes Neuronales Artificiales. El objetivo es detectar transacciones fraudulentas realizadas con tarjetas bancarias utilizando diferentes arquitecturas de redes neuronales y comparar su desempeño.

## Dataset

Se utilizó el conjunto de datos **Credit Card Fraud Detection** de Kaggle:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data?select=creditcard.csv

El dataset contiene transacciones bancarias etiquetadas como:

- Clase 0: Transacción normal.
- Clase 1: Fraude.

Debido a que el conjunto de datos está desbalanceado, además de la exactitud se evaluaron métricas como precisión, recall, F1-score y ROC-AUC.

## Metodología

Durante el desarrollo del proyecto se realizaron las siguientes etapas:

- Carga y exploración del dataset.
- Análisis de la distribución de fraudes y no fraudes.
- Escalamiento de las variables **Time** y **Amount**.
- División de los datos en entrenamiento, validación y prueba.
- Entrenamiento de tres arquitecturas de redes neuronales artificiales (MLP).
- Evaluación mediante métricas de clasificación y matriz de confusión.
- Registro de experimentos utilizando MLflow en DagsHub.

## Modelos evaluados

**Modelo 1**
- 1 capa oculta (64 neuronas)

**Modelo 2**
- 2 capas ocultas (128 y 64 neuronas)

**Modelo 3**
- 3 capas ocultas (128, 64 y 32 neuronas)
- Dropout de 0.3

## Resultados

Se compararon los tres modelos utilizando:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Matriz de confusión

El Modelo 3 obtuvo el mejor recall y ROC-AUC, por lo que fue seleccionado como el modelo con mejor desempeño para la detección de fraudes.

## Experimentos (MLflow - DagsHub)

Los experimentos fueron registrados utilizando MLflow en DagsHub.

**Enlace a los experimentos:**

https://dagshub.com/luceritosr/Fraud-Detection-Neural-Network/experiments

## Código

Repositorio de GitHub:

https://github.com/Luciernaga2303/Fraud-Detection-Neural-Network/tree/Luciernaga2303-Fraud_Detection_NN

## Autor

María Lucero Sánchez Ramírez
