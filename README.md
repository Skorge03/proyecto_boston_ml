"# Proyecto Boston Housing 

## Descripción
Este proyecto implementa un modelo de Machine Learning para predecir el precio de viviendas utilizando el dataset Boston Housing.
La variable objetivo es MEDV (valor medio de las viviendas).

Se utiliza un Pipeline de Scikit-Learn que incluye:
- Estandarización de datos con StandardScaler
- Modelo de regresión lineal con LinearRegression

El modelo entrenado se guarda en un archivo .pkl para poder utilizarlo fuera del notebook.

---

## Estructura del proyecto

proyecto_boston_ml/
│
├── boston.csv
├── boston_model.ipynb
├── pipeline_boston.pkl
├── probar_modelo.py
├── requirements.txt
└── README.md

---

## Instalación

1. Crear entorno virtual:

python3 -m venv .venv
source .venv/bin/activate

2. Instalar dependencias:

pip install -r requirements.txt

---

## Entrenamiento del modelo

El modelo se entrena dentro del notebook:

boston_model.ipynb

Pasos principales:
- Carga del dataset
- Separación de variables (X, y)
- División train/test
- Creación del Pipeline
- Entrenamiento
- Evaluación (MSE y R2)
- Guardado del modelo con joblib

---

## Archivo del modelo

pipeline_boston.pkl

Este archivo contiene:
- Escalado de datos
- Modelo entrenado

Permite hacer predicciones sin volver a entrenar.

---

## Probar el modelo fuera del notebook

Ejecutar:

python3 probar_modelo.py

Esto cargará el pipeline guardado y realizará una predicción con nuevos datos.

---

## Librerías utilizadas

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- joblib
- jupyterlab

---
