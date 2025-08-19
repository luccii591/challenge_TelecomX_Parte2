# 📊 Proyecto Challenge Telecom X - Parte 2

## Análisis Predictivo de Cancelación de Clientes (Churn) 

### 📌 Descripción del Proyecto

Este proyecto forma parte del **Challenge de Ciencia de Datos de Alura Latam / ONE**, cuyo objetivo es analizar y predecir la **cancelación de clientes (Churn)** en la empresa de Telecom X.

En esta segunda parte se profundiza en el análisis exploratorio, preparación de datos, entrenamiento de modelos y evaluación de resultados para desarrollar un sistema de predicción de clientes con riesgo de abandonar el servicio.

---

### 🎯 Objetivos

* Analizar los datos de clientes y servicios contratados.
* Preparar y limpiar el dataset para el modelado.
* Implementar técnicas de balanceo de clases (SMOTE).
* Entrenar y comparar diferentes modelos de clasificación.
* Evaluar el rendimiento de los modelos mediante métricas clave.
* Identificar las variables más influyentes en la predicción de churn.

---

### 🗂️ Estructura del Notebook

1. **Extracción de Datos** → Carga de información desde API/JSON.
2. **Transformación y Limpieza** → Normalización, tratamiento de columnas anidadas y diccionarios.
3. **EDA Inicial** → Exploración de variables numéricas y categóricas.
4. **Separación de Datos** → Train/Test con estratificación.
5. **Balanceo de Clases** → Uso de SMOTE para datos desbalanceados.
6. **Entrenamiento de Modelos** →

   * Regresión Logística
   * Árbol de Decisión
   * Random Forest
   * KNN (analizado pero descartado por tiempo de cómputo).
7. **Evaluación de Modelos** → Accuracy, Precision, Recall, F1, ROC-AUC.
8. **Interpretabilidad** → Permutation Importance en RF, Log y Árbol.

   * KNN documentado como **“no viable por tiempo, usar SHAP opcional”**.
9. **Informe Final ** → Conclusiones y recomendaciones

---

### 📈 Principales Resultados

* **Modelos destacados**: Random Forest y Regresión Logística (mejor equilibrio entre precisión y recall).
* **Variable más influyente**: Tipo de contrato y servicios adicionales.
* **Balanceo de datos**: SMOTE mejoró el rendimiento en la detección de clientes en riesgo.
* **KNN**: descartado por limitaciones de tiempo de cómputo, aunque podría analizarse con SHAP en un entorno de mayor capacidad.

---

### 🛠️ Tecnologías Utilizadas

* **Python 3.x**
* **Bibliotecas principales**:

  * `pandas`, `numpy` (manipulación de datos)
  * `matplotlib`, `seaborn` (visualización)
  * `scikit-learn` (modelado, métricas, SMOTE)
  * `imblearn` (técnicas de balanceo)

---

### 📌 Conclusiones

El análisis muestra que es posible predecir la cancelación de clientes con modelos de machine learning, siendo **Random Forest** el más robusto y explicativo. La empresa puede usar estas predicciones para diseñar campañas de retención y estrategias personalizadas, enfocándose en clientes con contratos mensuales y menos servicios adicionales.