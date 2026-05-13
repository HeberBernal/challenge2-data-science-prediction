# challenge2-data-science-prediction
"Modelado Predictivo de Churn: Implementación de Random Forest con balanceo de clases (SMOTE) para la optimización del Recall y detección proactiva de fuga de clientes."
# 🤖 Predicción de Churn: Pipeline de Data Science con Random Forest

Este proyecto desarrolla un ecosistema completo de ciencia de datos para predecir la fuga de clientes (Churn) en una empresa de telecomunicaciones. El enfoque principal radica en transformar datos complejos y resolver el desbalance de clases para mejorar la detección proactiva de bajas.

## 🎯 Objetivo del Proyecto
Construir y optimizar un modelo de clasificación capaz de identificar clientes con alta probabilidad de abandono, permitiendo estrategias de retención basadas en datos.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python 3.x
* **Librerías Principales:** * `Pandas` y `NumPy` para manipulación de datos.
  * `Scikit-Learn` para modelado predictivo.
  * `Imbalanced-learn (SMOTE)` para balanceo de clases.
  * `Matplotlib` y `Seaborn` para visualización.

## 🚀 Fases del Proyecto

### 1. Ingeniería de Datos (ETL)
* **Procesamiento de JSON:** Descomposición de estructuras anidadas en un formato tabular limpio.
* **Limpieza Técnica:** Tratamiento de datos faltantes en cargos totales y corrección de tipos de variables.
* **Feature Engineering:** Creación de la métrica `CARGO_DIARIO` para capturar patrones de consumo de manera más precisa.

### 2. Modelado y Optimización
Se implementó un algoritmo de **Random Forest**, enfrentando un dataset desbalanceado (solo el 26.5% representaba fuga).

* **Modelo Base:** Logró una precisión del 83% en clientes leales, pero una detección baja (Recall 0.48) en clientes en riesgo.
* **Optimización con SMOTE:** Se aplicó sobremuestreo sintético para balancear las clases, logrando **elevar el Recall de la clase Churn de 0.48 a 0.61**.

## 📊 Resultados Finales
El modelo optimizado permite identificar a **6 de cada 10 clientes** que planean dejar la compañía, proporcionando una herramienta de prevención con un desempeño equilibrado (F1-Score: 0.60).

| Métrica | Modelo Base | Modelo con SMOTE |
| :--- | :---: | :---: |
| **Recall (Churn)** | 0.48 | **0.61** |
| **F1-Score** | 0.54 | **0.60** |
| **Accuracy** | 0.78 | 0.78 |

## 📂 Estructura del Repositorio
* `Churn_Prediction_Model_SMOTE.ipynb`: Notebook principal con el flujo completo de limpieza, análisis y modelado.
* `README.md`: Descripción general del proyecto.

---
**Autor:** [Heber Job Bernal Monarrez](https://github.com/HeberBernal)  
*Data Analyst & Biomedical Researcher*
