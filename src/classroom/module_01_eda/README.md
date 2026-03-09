# Módulo 1 — Paradigma EDA  
## Exploratory Data Analysis para decisiones de negocio

> El análisis exploratorio de datos no es un paso “previo” al modelado: es el proceso mediante el cual una base de datos empieza a volverse inteligible para el negocio.  
> En este módulo, EDA se aborda como un **paradigma de lectura, diagnóstico y formulación de hipótesis**.

---

## 🎯 Propósito del módulo

Este módulo introduce el **Paradigma EDA (Exploratory Data Analysis)** como la primera capa de trabajo en ciencia de datos aplicada a negocios. La idea central no es solamente producir gráficos o estadísticas descriptivas, sino aprender a mirar un dataset como un sistema con estructura, sesgos, anomalías, segmentos y señales relevantes para la toma de decisiones.

Desde esta perspectiva, EDA cumple varias funciones simultáneas: permite entender la calidad real de los datos, detectar patrones dominantes, identificar comportamientos atípicos y formular hipótesis iniciales. Prepara el terreno para etapas posteriores como forecasting, machine learning, optimización o automatización. 

En resumen: **antes de predecir, optimizar o automatizar, hay que comprender**.

---

## 🧠 ¿Qué significa “Paradigma EDA”?

En este repositorio, EDA se entiende como un paradigma porque no se limita a una lista de técnicas; es una forma de pensar el análisis. Implica asumir que un dataset no es una tabla neutra lista para un algoritmo, sino una representación parcial e imperfecta de un proceso real. 

Este enfoque se apoya en cinco preguntas rectoras:

1. **¿Qué estoy mirando realmente?** Entender la unidad de análisis, el nivel de agregación, el período temporal y el contexto de negocio.
2. **¿Qué tan confiable es este dato?** Evaluar valores faltantes, duplicados, errores de carga, codificaciones inconsistentes y posibles sesgos de captura.
3. **¿Qué patrones dominan la estructura?** Identificar distribuciones, asimetrías, concentraciones y relaciones entre variables.
4. **¿Qué señales podrían transformarse en decisiones?** Conectar los datos con pricing, riesgo, churn, demanda, operación o marketing.
5. **¿Qué hipótesis vale la pena investigar después?** Orientar los siguientes pasos del proyecto basados en el diagnóstico.

---

## 📚 Objetivos de aprendizaje

Al finalizar este módulo, el estudiante debería poder:

* Comprender el rol estratégico del análisis exploratorio dentro del flujo de ciencia de datos.
* Distinguir entre inspección superficial y exploración analítica rigurosa.
* Evaluar calidad, consistencia y estructura de un dataset.
* Identificar distribuciones relevantes, valores extremos, relaciones y segmentos.
* Traducir hallazgos exploratorios en preguntas de negocio.
* Construir un diagnóstico inicial reproducible y claro.
* Preparar datasets para etapas posteriores de modelado.
* Comunicar hallazgos de forma comprensible para audiencias técnicas y no técnicas.

---

## 🧭 Enfoque del módulo

Este módulo combina tres niveles de lectura de datos para construir un puente entre el dato bruto y la inteligencia accionable:

* **Estructural:** ¿Cómo está formado el dataset? (filas, columnas, tipos de variables, granularidad, consistencia).
* **Estadístico:** ¿Cómo se comportan las variables? (distribuciones, dispersión, asociaciones, outliers, segmentación).
* **Estratégico:** ¿Qué implican esos patrones para el negocio, un producto, una operación o una decisión futura?

---

## 🧱 Estructura conceptual del módulo

### 1. El dato como representación de un proceso
Los datos son el resultado de un proceso de captura y medición. Entender el dataset exige entender el proceso que lo genera (unidad de observación, sesgos de selección, representación de eventos vs. estados).

### 2. Calidad del dato y diagnóstico inicial
Antes de graficar, hay que diagnosticar. Se evalúan valores faltantes, duplicados, tipos incorrectos, valores imposibles y escalas heterogéneas para entender su impacto en el análisis.

### 3. Distribuciones y forma de las variables
Toda variable tiene una forma que condiciona su modelado. Se analiza tendencia central, dispersión, asimetría, colas y concentración para detectar regímenes distintos dentro del negocio.

### 4. Outliers, anomalías y observaciones influyentes
Distinguir entre anomalía estadística y anomalía de negocio. Los extremos pueden ser ruido, fraude, clientes premium o fallas del sistema que merecen atención estratégica.

### 5. Relaciones entre variables
Examinar cómo interactúan las variables bajo diferentes contextos (asociaciones lineales/no lineales, dependencias ocultas). El promedio global suele ocultar estructuras internas clave.

### 6. Segmentación y heterogeneidad
Detectar grupos de comportamiento dispar dentro de un dataset aparentemente homogéneo (análisis por cohortes, canales, productos o segmentos de valor).

### 7. EDA como generador de hipótesis
El objetivo final: formular mejores preguntas. ¿Por qué un segmento tiene más churn? ¿Por qué la demanda es más volátil en ciertas regiones? El siguiente paso nace del diagnóstico, no del azar.

---

## 🚀 Recursos y Material Interactivo

En esta sección encontrarás dashboards, simulaciones y recursos aplicados para experimentar visualmente con los conceptos del módulo.

| 📄 Recurso | 📥 Acceso |
| :--- | :--- |
| **Business EDA Lab (Dashboard Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Dashboard interactivo orientado al análisis exploratorio de datos aplicado a negocio, marketing y comportamiento del cliente. Complementa el trabajo en notebook y permite explorar visualmente segmentación, gasto, canales de compra, respuesta a campañas y correlaciones con fines pedagógicos.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Dashboard-Interactivo-green?style=for-the-badge&logo=google-chrome)](https://business-eda-dashboard.lovable.app) |
---

## 💼 Aplicaciones en negocios

El paradigma EDA tiene aplicaciones directas y tangibles:
* **Marketing:** Comportamiento de clientes, respuesta a campañas, canales de conversión.
* **Finanzas:** Concentración de riesgo, anomalías transaccionales, perfiles de morosidad.
* **Operaciones:** Cuellos de botella, variabilidad en tiempos, patrones de demanda.
* **Producto:** Uso, retención, comportamiento por cohortes, señales de abandono.
* **Ventas:** Dispersión comercial, performance por equipo, ticket promedio.

---

## 🛠️ Herramientas y técnicas habituales

* **Manipulación:** `pandas` (limpieza y transformación inicial), `numpy` (operaciones numéricas).
* **Visualización:** `matplotlib`, `seaborn` (histogramas, boxplots, scatter plots, heatmaps).
* **Análisis:** Tablas de frecuencia, profiling inicial, matrices de correlación, agrupaciones.

---

## 📂 Estructura sugerida del módulo

```text
module_01_eda/
├── README.md
├── notebooks/
│   ├── 01_dataset_overview.ipynb
│   ├── 02_data_quality.ipynb
│   ├── 03_distributions.ipynb
│   ├── 04_outliers_and_anomalies.ipynb
│   ├── 05_relationships_and_segments.ipynb
│   └── 06_business_insights.ipynb
├── data/
│   └── sample_dataset.csv
├── assets/
│   ├── charts/
│   └── diagrams/
└── docs/
    └── notes.md

