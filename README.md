# TelecomX – Predicción de Cancelación de Clientes (Churn)

## Descripción del Proyecto

Este proyecto forma parte del **Challenge de Machine Learning del programa Oracle Next Education (ONE)** y tiene como objetivo desarrollar modelos predictivos capaces de identificar clientes con alta probabilidad de cancelar sus servicios en la empresa ficticia **TelecomX**.

La cancelación de clientes (*churn*) representa uno de los principales desafíos para empresas de telecomunicaciones. Por ello, mediante técnicas de **análisis de datos y Machine Learning**, se busca detectar patrones que permitan anticipar el abandono y diseñar estrategias de retención efectivas.

---

## Objetivo

Desarrollar un pipeline de Machine Learning que permita:

- Preparar y transformar los datos para el modelado
- Identificar variables relevantes relacionadas con la cancelación
- Entrenar y evaluar modelos predictivos
- Interpretar los factores que influyen en el churn
- Proponer estrategias de retención basadas en los resultados

---

## Proceso de Análisis

### 1. Preparación de datos

Se trabajó con un dataset previamente limpiado en la primera parte del challenge. Posteriormente se realizaron:

- Codificación de variables categóricas (*One-Hot Encoding*)
- Revisión de balance de clases
- Análisis de correlación
- Preparación del dataset final para modelado

Dataset final utilizado:

- **7032 registros**
- Variables categóricas y numéricas procesadas
- Variable objetivo: `abandono`

---

### 2. Modelos entrenados

Se implementaron dos modelos de clasificación:

- **Regresión Logística**
- **Random Forest**

Estos modelos fueron seleccionados porque permiten comparar:

- un modelo lineal interpretable
- un modelo basado en árboles más flexible

---

## Evaluación de Modelos

Los modelos fueron evaluados utilizando las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión
- Curva ROC

| Modelo | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|------|------|------|------|------|------|
| Regresión Logística | 0.80 | 0.66 | 0.54 | 0.59 | 0.84 |
| Random Forest | 0.78 | 0.61 | 0.47 | 0.53 | 0.82 |

### Modelo seleccionado

El modelo **Regresión Logística** presentó el mejor desempeño general y una mayor capacidad de interpretación de las variables.

---

## Factores que influyen en la cancelación

A partir del análisis de importancia de variables se identificaron los factores más relevantes asociados al churn.

### Variables que aumentan la probabilidad de cancelación

- Servicio de internet **Fiber optic**
- Método de pago **Electronic check**
- **Cargos elevados** asociados al servicio
- Factura digital
- Consumo de servicios de streaming

### Variables que reducen la probabilidad de cancelación

- **Antigüedad del cliente**
- Contratos de **1 o 2 años**
- Servicios adicionales como:
  - soporte técnico
  - seguridad online
  - respaldo online

---

## Principales Insights

Los resultados muestran que el churn en TelecomX está fuertemente relacionado con:

- el **tiempo de permanencia del cliente**
- el **tipo de contrato**
- el **tipo de servicio de internet**
- el **método de pago**
- el **costo del servicio**

Estos factores permiten identificar segmentos de clientes con mayor riesgo de abandono.

---

## Estrategias de Retención Propuestas

Basándose en los resultados del modelo, se proponen las siguientes acciones:

### 1. Programa de retención para clientes nuevos
Los primeros meses son críticos. Se recomienda implementar campañas de seguimiento temprano.

### 2. Incentivar contratos de mayor duración
Los contratos largos reducen significativamente la probabilidad de churn.

### 3. Revisar la experiencia del servicio de fibra óptica
Este servicio presenta una fuerte relación con la cancelación.

### 4. Promover métodos de pago automáticos
El método **Electronic Check** se asocia con mayor churn.

### 5. Potenciar servicios adicionales
Servicios como soporte técnico y seguridad online aumentan la permanencia del cliente.

---

## Tecnologías Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Google Colab
- Git & GitHub

---

## Autor

**Santiago Aparicio**

Proyecto desarrollado como parte del programa **Oracle Next Education (ONE)**.
