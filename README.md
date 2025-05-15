# Machine Learning para predecir cancelaciones y mejorar la retención en seguros

Repositorio del Trabajo Final de Máster (TFM) para el Máster Universitario en Ciencia de Datos (UOC).

---

## Descripción

Este repositorio contiene la memoria y el código asociado al TFM, cuyo objetivo es desarrollar y analizar modelos de machine learning para predecir la cancelación de pólizas de seguros, optimizando la retención de clientes y proporcionando interpretabilidad sobre los factores clave que influyen en estas decisiones. El código está estructurado en notebooks Jupyter (`.ipynb`) y la memoria completa se incluye en PDF.

---

## Estructura del repositorio

```
├── TFM.pdf
├── notebooks/
│ ├── 1_EDA_y_preprocesado.ipynb
│ ├── 2_Modelado.ipynb
│ ├── 3_Optimizacion.ipynb
│ └── 4_Modelo_resultante.ipynb
├── data/
│ └── datos.csv
├── requirements.txt
└── README.md
```

**Notebooks:**
- `1_EDA_y_preprocesado.ipynb`: Análisis exploratorio de datos y preprocesamiento.
- `2_Modelado.ipynb`: Entrenamiento y evaluación de modelos base. Técnicas de balanceo.
- `3_Optimizacion.ipynb`: Optimización de hiperparámetros.
- `4_Modelo_resultante.ipynb`: Evaluación final, interpretabilidad (SHAP) y conclusiones.

---

## Resumen del proyecto

- **Título:** Machine Learning para predecir cancelaciones y mejorar la retención en seguros
- **Autor:** Luis Carlos Ocaña Hoeber
- **Titulación:** Máster Universitario en Ciencia de Datos (UOC)
- **Fecha:** 06/2024
- **Palabras clave:** Machine Learning, Renovación de pólizas, Modelado predictivo, Predicción de abandono de clientes

### Objetivo

Desarrollar modelos de machine learning para predecir la cancelación de pólizas de seguros, optimizando su rendimiento y proporcionando interpretaciones claras sobre los factores que influyen en dichas predicciones.

### Metodología

- **CRISP-DM** como marco de trabajo.
- **Dataset:** Datos sintéticos de Kaggle ("Auto Insurance Churn Analysis Dataset").
- **Procesos:** EDA, preprocesado, modelado (regresión logística, SVM, KNN, árboles, Random Forest, AdaBoost, XGBoost, redes neuronales), técnicas de balanceo (oversampling, undersampling, SMOTE), optimización de hiperparámetros (GridSearchCV, Optuna) y análisis de interpretabilidad (SHAP).

### Principales resultados

- El modelo con mejor desempeño fue **Random Forest** combinado con **SMOTE** y ajuste de hiperparámetros.
- F1-Score para la clase minoritaria (churn): **0.45**.
- Variable más relevante: **Antigüedad del cliente** (`days_tenure`).
- Interpretabilidad mediante valores SHAP para identificar factores clave.

---

## Requisitos

- Python 3.8+
- Ver `requirements.txt` para dependencias específicas

Paquetes principales:
- numpy, pandas, scikit-learn, matplotlib, seaborn, xgboost, keras, optuna, shap, imbalanced-learn

---

## Instrucciones de uso

1. **Clona el repositorio**

```
git clone https://github.com/usuario/TFM-churn-seguros.git
cd TFM-churn-seguros
```

2. **Instala las dependencias**

```
pip install -r requirements.txt
```

4. **Descarga o coloca los datos**
- Los datos utilizados son sintéticos y están disponibles en [Kaggle](https://www.kaggle.com/datasets/merishnasuwal/auto-insurance-churn-analysis-dataset).

4. **Ejecuta los notebooks**
- Abre los notebooks en Google Colab o Jupyter Notebook siguiendo el orden numérico para reproducir el flujo completo: EDA → Modelado → Optimización → Modelo resultante.

---

## Contacto

- **Autor:** Luis Carlos Ocaña Hoeber
- **Email:** [luisocanahober@gmail.com]

---

> Este repositorio incluye tanto la memoria completa del TFM (`TFM.pdf`) como el código reproducible en notebooks. Se recomienda consultar el PDF para una explicación detallada de los resultados y la justificación metodológica.
