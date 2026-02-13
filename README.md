# Telecom Customer Churn Prediction

Este repositorio contiene un pipeline completo de Ciencia de Datos para predecir la probabilidad de que un cliente abandone los servicios de una empresa de telecomunicaciones (Churn).

## Descripción del Proyecto

El objetivo principal es identificar patrones de comportamiento en los clientes que preceden a la cancelación del servicio.

Para ello, se implementó un modelo de **Regresión Logística**, el cual permite:

- Clasificar clientes en riesgo de churn.
- Obtener probabilidades asociadas a cada cliente.
- Interpretar la influencia de las variables en la predicción.

## Dataset

Se utilizó el dataset "Telco Customer Churn", disponible en [Kaggle](https://www.kaggle.com/).

Incluye información sobre:

- **Servicios**
  - Telefonía
  - Múltiples líneas
  - Internet
  - Seguridad online
  - Streaming
  - Soporte técnico
- **Información de la cuenta**
  - Tiempo de permanencia (tenure)
  - Tipo de contrato
  - Método de pago
  - Cargos mensuales
  - Cargos totales
- **Demografía**
  - Género
  - Adulto mayor
  - Socios (Partner)
  - Dependientes

## Tecnologías y Librerías

- **Lenguaje:** Python 3.14
- **Análisis de Datos:** Pandas, NumPy
- **Visualización:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn
  - Escalado
  - Codificación
  - Modelado

## Estructura del Pipeline

### 1. EDA (Exploratory Data Analysis)

- Distribución de la variable objetivo (Churn).
- Análisis de correlación.
- Visualización de patrones relevantes.

### 2. Preprocesamiento

- Tratamiento de valores faltantes.
- Codificación de variables categóricas (One-Hot Encoding).
- Escalado de características con StandardScaler.

### 3. Modelado

- Entrenamiento de un modelo de Regresión Logística.

### 4. Evaluación

- Matriz de confusión.
- Métricas de precisión y recall.
- Curvas de calibración.
- Accuracy global del modelo.

## Resultados

- **Exactitud (Accuracy):** ~80%
- El tipo de contrato y el tiempo de permanencia se identificaron como los predictores más relevantes para la deserción.
