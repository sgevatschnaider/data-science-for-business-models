# Módulo 1 — Paradigma EDA  
## Exploratory Data Analysis para decisiones de negocio

> El análisis exploratorio de datos no es un paso “previo” al modelado: es el proceso mediante el cual una base de datos empieza a volverse inteligible para el negocio.  
> En este módulo, EDA se aborda como un **paradigma de lectura, diagnóstico y formulación de hipótesis**.

---

##  Propósito del módulo

Este módulo introduce el **Paradigma EDA (Exploratory Data Analysis)** como la primera capa de trabajo en ciencia de datos aplicada a negocios. La idea central no es solamente producir gráficos o estadísticas descriptivas, sino aprender a mirar un dataset como un sistema con estructura, sesgos, anomalías, segmentos y señales relevantes para la toma de decisiones.

Desde esta perspectiva, EDA cumple varias funciones simultáneas: permite entender la calidad real de los datos, detectar patrones dominantes, identificar comportamientos atípicos y formular hipótesis iniciales. Prepara el terreno para etapas posteriores como forecasting, machine learning, optimización o automatización. 

En resumen: **antes de predecir, optimizar o automatizar, hay que comprender**.

---

##  ¿Qué significa “Paradigma EDA”?

En este repositorio, EDA se entiende como un paradigma porque no se limita a una lista de técnicas; es una forma de pensar el análisis. Implica asumir que un dataset no es una tabla neutra lista para un algoritmo, sino una representación parcial e imperfecta de un proceso real. 

Este enfoque se apoya en cinco preguntas rectoras:

1. **¿Qué estoy mirando realmente?** Entender la unidad de análisis, el nivel de agregación, el período temporal y el contexto de negocio.
2. **¿Qué tan confiable es este dato?** Evaluar valores faltantes, duplicados, errores de carga, codificaciones inconsistentes y posibles sesgos de captura.
3. **¿Qué patrones dominan la estructura?** Identificar distribuciones, asimetrías, concentraciones y relaciones entre variables.
4. **¿Qué señales podrían transformarse en decisiones?** Conectar los datos con pricing, riesgo, churn, demanda, operación o marketing.
5. **¿Qué hipótesis vale la pena investigar después?** Orientar los siguientes pasos del proyecto basados en el diagnóstico.

---

##  Objetivos de aprendizaje

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

## Enfoque del módulo

Este módulo combina tres niveles de lectura de datos para construir un puente entre el dato bruto y la inteligencia accionable:

* **Estructural:** ¿Cómo está formado el dataset? (filas, columnas, tipos de variables, granularidad, consistencia).
* **Estadístico:** ¿Cómo se comportan las variables? (distribuciones, dispersión, asociaciones, outliers, segmentación).
* **Estratégico:** ¿Qué implican esos patrones para el negocio, un producto, una operación o una decisión futura?

---

## Estructura conceptual del módulo

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

## Recursos y Material Interactivo

En esta sección encontrarás dashboards, simulaciones y recursos aplicados para experimentar visualmente con los conceptos del módulo.

| 📄 Recurso | 📥 Acceso |
| :--- | :--- |
| **EDA_Notebook_Introduccion.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook introductorio dedicado a presentar el paradigma del <strong>Exploratory Data Analysis (EDA)</strong> como primera etapa fundamental en todo proyecto de ciencia de datos. El material explica el rol del análisis exploratorio para comprender la estructura de los datos antes del modelado, incluyendo inspección del dataset, identificación de tipos de variables, análisis descriptivo, estudio de distribuciones y exploración de relaciones entre variables.</p><p>A través de ejemplos en Python se ilustran herramientas básicas de análisis como estadística descriptiva, visualización de distribuciones, análisis univariado y bivariado, correlación entre variables y detección inicial de patrones relevantes para la toma de decisiones.</p><p>El notebook utiliza el dataset <code>tips</code> de <code>seaborn</code> como caso práctico para mostrar cómo aplicar EDA en un contexto real, analizando comportamiento de clientes, patrones de gasto y variables explicativas que permiten generar intuiciones analíticas antes de construir modelos predictivos.</p></details> | [![EDA_Notebook_Introduccion.ipynb](https://img.shields.io/badge/EDA_Notebook_Introduccion-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/14Vm6DoayZcSnJLpkQpJ_YVciStuR7k5F#scrollTo=46z-kLbfn4Gq) |

| 📄 Recurso | 📥 Acceso |
| :--- | :--- |
| **Customer Personality Analysis (Dashboard Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Dashboard interactivo orientado al análisis exploratorio de datos aplicado a negocio, marketing y comportamiento del cliente. Complementa el trabajo en notebook y permite explorar visualmente segmentación, gasto, canales de compra, respuesta a campañas y correlaciones con fines pedagógicos.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Dashboard-orange?style=for-the-badge&logo=google-chrome)](https://69af9194a879a100089acc27--clinquant-meringue-3930c2.netlify.app/src/classroom/graphs/recursos/eda_dashboard) <br><br> [![Customer%20Personality%20Analysis](https://img.shields.io/badge/Customer%20Personality%20Analysis-Dashboard-green?style=for-the-badge&logo=google-chrome)](https://business-eda-dashboard.lovable.app) |
---
| 📄 Recurso | 📥 Acceso |
| :--- | :--- |
| **Glosario del Paradigma EDA (HTML Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Glosario interactivo orientado a consolidar los conceptos fundamentales del paradigma EDA. Reúne definiciones clave, lenguaje técnico y nociones analíticas necesarias para comprender con mayor precisión el análisis exploratorio de datos en contextos académicos y aplicados.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Glosario-blue?style=for-the-badge&logo=google-chrome)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/data-science-for-business-models/b7f8849b5b88795e5cc8513bfa74db314063b54b/src/classroom/module_01_eda/html/EDA_%20Glosario.html) |
| **Cuestionario del Paradigma EDA (HTML Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Cuestionario interactivo diseñado para repasar y afianzar los ejes centrales del paradigma EDA. Integra preguntas conceptuales con desarrollo explicativo sobre variables, distribuciones, valores atípicos, datos faltantes, correlación, calidad del dato y decisiones de preprocesamiento.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Cuestionario-green?style=for-the-badge&logo=google-chrome)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/data-science-for-business-models/b7f8849b5b88795e5cc8513bfa74db314063b54b/src/classroom/module_01_eda/html/EDA_Cuestionario.html) |

| 📄 Recurso | 📥 Acceso |
| :--- | :--- |
| **Missing_Data_Marco_Conceptual.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook teórico–conceptual dedicado a desarrollar de manera integral el problema de los <strong>missing data</strong> desde una perspectiva estadística, organizacional y económica. El material presenta los datos faltantes no solo como un inconveniente técnico de limpieza de bases, sino como una manifestación de fricciones informacionales, fallas de captura, asimetrías de información y limitaciones en los procesos de decisión dentro de una organización.</p><p>A lo largo del desarrollo se explican los principales marcos conceptuales para comprender el fenómeno, incluyendo la definición de datos faltantes, sus causas más frecuentes en contextos empresariales, la diferencia entre ausencia estructural y omisión problemática, y la tipología clásica <code>MCAR</code>, <code>MAR</code> y <code>MNAR</code>. Además, se vincula el tratamiento de missing data con la calidad de datos, la gobernanza de la información, la analítica de negocios y el impacto sobre métricas, segmentaciones, modelos predictivos y decisiones estratégicas.</p><p>El notebook funciona como base teórica para cursos de ciencia de datos, estadística aplicada y analítica de negocios, permitiendo comprender por qué los datos faltantes deben interpretarse en su contexto y no resolverse de manera automática o mecánica.</p></details> | [![Missing_Data_Marco_Conceptual.ipynb](https://img.shields.io/badge/Missing_Data_Marco_Conceptual-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1_ldjrvEBsIlo3_GvoKJ3tUXdmjG_Nvq2?usp=sharing) |
| **Missing_Data_House_Prices.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook práctico orientado al análisis aplicado de <strong>missing data</strong> utilizando el dataset <strong>House Prices</strong> como caso de estudio real. El material muestra paso a paso cómo detectar, cuantificar, visualizar e interpretar datos faltantes en una base compleja, destacando que no toda ausencia de información implica error, ya que en muchos casos el valor faltante expresa la inexistencia real de un atributo.</p><p>Mediante herramientas de Python y librerías especializadas se desarrollan procedimientos de inspección inicial, medición del porcentaje de faltantes por variable y por observación, visualización con <code>missingno</code>, análisis de variables numéricas y categóricas, e identificación de patrones de ausencia estructural en atributos vinculados, por ejemplo, a garaje, pileta, sótano, cercos o chimeneas. El notebook también compara distintas estrategias de tratamiento, desde enfoques simples de imputación hasta aproximaciones más interpretativas basadas en el significado del dato faltante.</p><p>Como parte del cierre analítico, el recurso incorpora pipelines de preprocesamiento y modelado con algoritmos como <code>Ridge</code> y <code>Random Forest</code>, permitiendo evaluar cómo diferentes decisiones sobre imputación y creación de indicadores de ausencia impactan en el desempeño predictivo. De este modo, el notebook no solo enseña a tratar missing data, sino también a comprender su relevancia estadística y su valor informacional en problemas reales de ciencia de datos.</p></details> | [![Missing_Data_House_Prices.ipynb](https://img.shields.io/badge/Missing_Data_House_Prices-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1YUFaKt8HslnUmE9_2pyjtxg3Lt5k5HYn?usp=sharing) |

| Recurso | Enlace |
| :--- | :---: |
| **Outliers_Deteccion_Tratamiento.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook teórico-práctico enfocado en los fundamentos estadísticos y metodológicos para la <strong>Detección y Tratamiento de Outliers</strong> (valores atípicos). El material presenta un marco analítico integral para comprender qué es un outlier, por qué se produce y cómo gestionarlo adecuadamente para no sesgar los modelos predictivos o el análisis exploratorio.</p><p>A través de explicaciones estructuradas y visualizaciones, se exploran a fondo los métodos estadísticos clásicos para la detección, tales como el Rango Intercuartílico (IQR) y el Z-Score. Asimismo, se enseñan técnicas avanzadas de mitigación de impacto, contrastando enfoques de <em>capping</em> o recorte (como la Winsorización) frente a técnicas de transformación matemática (como la transformación logarítmica). </p><p>El notebook funciona como una guía esencial para estudiantes de ciencia de datos, haciendo hincapié en un concepto fundamental: no todo valor atípico es necesariamente un error de carga. En muchas ocasiones, un outlier contiene información altamente valiosa sobre la naturaleza subyacente del problema de negocio, y su tratamiento debe ser una decisión analítica consciente, no una automatización ciega.</p></details> | [![Outliers_Teoria.ipynb](https://img.shields.io/badge/Outliers_Teoria-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1C9k3F2sWIGx8ORQRN6HCB0V70z-r_Bia?usp=sharing) |
| **Hotel_Booking_EDA_Modelado.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook práctico orientado a la aplicación de técnicas de preprocesamiento, clasificación y Análisis Exploratorio de Datos (EDA) utilizando el reconocido dataset transaccional <strong>Hotel Booking Demand</strong>. Este recurso actúa como la bajada a la práctica de la teoría estadística, trabajando con datos extraídos directamente de Sistemas de Gestión de Propiedades (PMS) reales de la industria hotelera.</p><p>El material muestra paso a paso cómo lidiar con la suciedad inherente a los datos del mundo real. Se abordan desafíos críticos como el <em>Feature Engineering</em> (creación de nuevas variables de valor a partir de las existentes) y el manejo en vivo de valores atípicos extremos, tales como tarifas diarias irrazonables o reservas efectuadas con años de antelación.</p><p>De manera muy especial, este caso de estudio se centra en ilustrar el peligroso concepto de <strong>Fuga de Datos (Data Leakage)</strong>, enseñando a los analistas a no utilizar variables que revelen el futuro (como el estado final de la reserva) para predecir si un cliente cancelará o no. El notebook conecta directamente el modelado de Machine Learning con el razonamiento económico, demostrando cómo predecir cancelaciones es la base para estrategias de <em>Revenue Management</em> y sobreventa estratégica.</p></details> | [![Hotel_Booking.ipynb](https://img.shields.io/badge/Hotel_Booking-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1BJU3zTYvxerrVwQDhyz3v2ZU113cp3Dp?usp=sharing) |
---

| Recurso | Enlace |
| :--- | :---: |
| **Correlacion_Regresion_Transformaciones.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook teórico-práctico orientado al análisis de la relación entre variables mediante los coeficientes de <strong>Pearson</strong> y <strong>Spearman</strong>, destacando cómo la presencia de valores atípicos puede alterar la interpretación estadística de las asociaciones.</p><p>El material desarrolla además una <strong>regresión lineal</strong> con evaluación de capacidad predictiva a partir de una partición <em>train/test</em>, permitiendo comprender no solo el ajuste del modelo, sino también su desempeño fuera de la muestra de entrenamiento.</p><p>Como complemento metodológico, el notebook explica la preparación de datos a través de <strong>transformaciones</strong> como <em>Box-Cox</em> y el <em>logaritmo</em>, junto con técnicas de <strong>escalado</strong> como <em>Min-Max</em> y <em>Z-score</em>. La idea central que articula todo el recorrido es que transformar los datos no implica únicamente “modificar valores”, sino <strong>reorganizar el problema matemático</strong> de una manera que puede optimizar significativamente el rendimiento de los modelos de <em>machine learning</em>.</p></details> | [![Correlacion_Regresion_Transformaciones.ipynb](https://img.shields.io/badge/Correlaci%C3%B3n%20y%20Regresi%C3%B3n-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1k0PS6YHCdmXCOMuKZMrKGOPqbYcp-Wur?usp=sharing) |


| Recurso | Enlace |
| :--- | :---: |
| **Regresion_Lineal_Multivariada_y_Validacion_Cruzada.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook teórico-práctico orientado al análisis de la <strong>regresión lineal multivariada</strong>, enfatizando la interpretación econométrica de los coeficientes, la evaluación del ajuste y el estudio de los supuestos clásicos del modelo lineal.</p><p>El material incorpora además herramientas de <strong>validación cruzada</strong> para examinar la capacidad predictiva del modelo fuera de muestra, permitiendo comparar el desempeño observado en entrenamiento con la estabilidad de los resultados en particiones sucesivas de los datos.</p><p>Como complemento metodológico, el notebook desarrolla una <strong>aplicación empírica completa</strong> con exploración inicial, selección de variables, diagnóstico de residuos, análisis de multicolinealidad y visualizaciones explicativas. La idea central que articula todo el recorrido es que <strong>un buen modelo no solo debe ajustarse correctamente, sino también generalizar de manera razonable e interpretable</strong>.</p></details> | [![Regresión lineal multivariada y validación cruzada](https://img.shields.io/badge/Regresi%C3%B3n%20Lineal%20Multivariada-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1YkDgjBnu_d1aSGdozvsE1n7TEzimXOPt?usp=sharing) |

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

