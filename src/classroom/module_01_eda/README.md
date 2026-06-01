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
* 

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

| 📄 Recurso | 📥 Acceso |
| :--- | :--- |
| **Series_de_tiempo_.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook interactivo orientado a introducir de manera aplicada los conceptos fundamentales del análisis de <strong>series de tiempo</strong> en un entorno didáctico de Google Colab. El material construye una serie temporal simulada de <strong>ventas mensuales</strong> y la utiliza como base para explicar, paso a paso, cómo identificar y separar sus componentes principales: <strong>tendencia</strong>, <strong>estacionalidad</strong> y <strong>ruido</strong>.</p><p>A lo largo del desarrollo, el notebook muestra cómo una serie temporal no debe interpretarse como una simple colección de datos, sino como una secuencia ordenada en la que el tiempo tiene un papel central en el análisis. Para ello, incorpora visualizaciones progresivas, explicaciones en HTML, tablas intermedias y gráficos que permiten observar la evolución de la serie, comparar sus movimientos y comprender la lógica del comportamiento temporal.</p><p>El ejercicio incluye además herramientas introductorias clave para el estudio del tema, como el uso de <strong>promedios móviles</strong> para suavizar fluctuaciones, el ajuste de una <strong>tendencia lineal</strong>, el cálculo de un <strong>índice estacional simple</strong>, la <strong>desestacionalización</strong> de la serie y la elaboración de un <strong>pronóstico básico</strong> para períodos futuros. También incorpora conclusiones automáticas, preguntas para discusión en clase y exportación de resultados en archivos <code>CSV</code>, lo que lo convierte en un recurso útil tanto para la enseñanza de ciencia de datos como para cursos introductorios de estadística aplicada, analítica de negocios y modelado temporal.</p><p>En conjunto, el notebook funciona como una práctica completa para comprender la estructura conceptual de una serie de tiempo y sentar las bases para análisis posteriores más avanzados.</p></details> | [![Series_de_tiempo_.ipynb](https://img.shields.io/badge/Series_de_tiempo-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1zqMbHTvyFL0kUVX9eVFWvaHyy353UOgu?usp=sharing) |

| 📄 Recurso | 📥 Acceso |
| :--- | :--- |
| **Regresion_Logistica.ipynb (Notebook Interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir)</em></summary><p>Notebook interactivo orientado a introducir de manera aplicada, visual y matemática los fundamentos de la <strong>regresión logística</strong>, uno de los modelos más importantes para problemas de clasificación binaria dentro de la estadística aplicada y el aprendizaje automático. El material parte de la pregunta central del modelo: cómo estimar la probabilidad de que ocurra un evento, es decir, cómo calcular <code>P(Y=1 &#124; X=x)</code> cuando la variable objetivo solo puede tomar dos valores posibles, como aprobar o no aprobar, comprar o no comprar, fraude o no fraude, enfermedad o ausencia de enfermedad.</p><p>A lo largo del notebook se explica por qué la regresión logística no predice directamente una clase, sino una <strong>probabilidad</strong>, y por qué esa probabilidad luego se transforma en una decisión mediante el uso de <strong>umbrales</strong>. Para ello, el recurso desarrolla la función logística o <strong>sigmoide</strong>, mostrando cómo una combinación lineal de variables puede convertirse en un valor comprendido entre 0 y 1, lo que permite interpretar el resultado como una probabilidad válida.</p><p>El material incorpora una explicación matemática progresiva de los principales componentes del modelo: la combinación lineal, la función sigmoide, los <strong>odds</strong>, el <strong>logit</strong>, la interpretación de los coeficientes, el concepto de <strong>odds ratio</strong>, la función de verosimilitud y la pérdida logística. De esta manera, el notebook no se limita a mostrar el uso operativo del algoritmo, sino que también permite comprender la lógica estadística que sostiene al modelo.</p><p>Además, el notebook incluye ejercicios didácticos para trabajar en clase, como el cálculo manual de probabilidades, la interpretación de coeficientes, el análisis del cambio de umbral y la lectura de resultados del modelo. Estos ejercicios ayudan a conectar la formulación matemática con situaciones concretas de clasificación, permitiendo que los estudiantes comprendan la diferencia entre estimar una probabilidad y tomar una decisión clasificatoria.</p><p>En su parte aplicada, el recurso utiliza Python en Google Colab para construir ejemplos reproducibles con datos sintéticos, entrenar modelos de regresión logística mediante bibliotecas de ciencia de datos, visualizar la curva sigmoide, analizar la frontera de decisión, calcular predicciones, construir una matriz de confusión y evaluar el desempeño del modelo mediante métricas como <strong>accuracy</strong>, <strong>precision</strong>, <strong>recall</strong>, <strong>F1-score</strong>, <strong>ROC-AUC</strong> y curvas de evaluación. También se incorpora la discusión sobre el impacto del umbral en los falsos positivos y falsos negativos, un aspecto clave para comprender el uso responsable del modelo en problemas reales.</p><p>El notebook también introduce extensiones importantes, como la regularización, el tratamiento de clases desbalanceadas y la generalización hacia problemas multiclase mediante la función <strong>softmax</strong>. En conjunto, funciona como una práctica completa para enseñar regresión logística desde una perspectiva conceptual, matemática, computacional y aplicada, resultando útil para cursos introductorios de machine learning, estadística aplicada, ciencia de datos, analítica de negocios y modelado predictivo.</p></details> | [![Regresion_Logistica.ipynb](https://img.shields.io/badge/Regresion_Logistica-Notebook-blue?style=for-the-badge&logo=jupyter)](https://colab.research.google.com/drive/1uLPm6Uaaba5qEnMcta2bg5SMiM-G9AeT?usp=sharing) |


# 🌲 Random Forest · Recursos interactivos de estudio

Este bloque reúne los recursos interactivos sobre **Random Forest**, organizados como una secuencia didáctica progresiva: primero la intuición de los ensambles, luego la lógica estadística del muestreo, después los criterios de división de los árboles y finalmente los materiales de consolidación: cuestionario y glosario.

---

## 🧩 Bloque · Random Forest: intuición, construcción y consolidación

| Orden | Recurso | Nivel | Función | Acceso |
| :---: | :--- | :---: | :--- | :---: |
| **1** | **Sabiduría del Ensamble**<br><br><details><summary><strong>Resumen</strong></summary><p>Recurso introductorio para explicar la intuición central detrás de los modelos de ensamble: muchas estimaciones individuales pueden combinarse para producir una decisión colectiva más estable. Conecta la idea de la “sabiduría de la multitud” con Random Forest, mostrando cómo varios árboles pueden compensar errores individuales mediante votación o promedio.</p><p>Es recomendable ubicarlo al inicio porque permite explicar Random Forest antes de entrar en fórmulas, hiperparámetros o criterios de división.</p></details> | Introductorio | Introducir la lógica colectiva de los ensambles y preparar la intuición de Random Forest. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_sabiduria_ensamble.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_sabiduria_ensamble.html) |
| **2** | **Random Forest · Ensamble**<br><br><details><summary><strong>Resumen</strong></summary><p>Recurso orientado a explicar qué es un ensamble en Machine Learning y cómo Random Forest se ubica dentro de esa familia. Presenta distintas estrategias como voting, bagging, boosting y stacking, y diferencia especialmente Random Forest como una extensión del bagging aplicada a árboles de decisión.</p><p>Incluye una visualización animada donde varios árboles producen votos y el bosque genera una predicción final. Es útil para mostrar que Random Forest no busca un árbol perfecto, sino muchos árboles diferentes que se combinan.</p></details> | Introductorio / Intermedio | Explicar los tipos de ensamble y ubicar Random Forest dentro del bagging. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_ensamble.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_ensamble.html) |
| **3** | **Random Forest · Muestreo con Reposición**<br><br><details><summary><strong>Resumen</strong></summary><p>Simulación interactiva para comprender el muestreo con reposición, base del bootstrap. El recurso muestra cómo una observación puede aparecer varias veces en una muestra y cómo otras pueden quedar afuera, permitiendo entender por qué cada árbol del bosque ve una versión distinta del dataset original.</p><p>Este recurso es clave para explicar la diversidad entre árboles, la construcción de muestras bootstrap y la idea de observaciones out-of-bag.</p></details> | Intermedio | Visualizar el mecanismo estadístico del muestreo con reposición. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_muestreo_con_reposicion.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_muestreo_con_reposicion.html) |
| **4** | **Random Forest · Gini y Entropía**<br><br><details><summary><strong>Resumen</strong></summary><p>Visualización interactiva para estudiar dos criterios fundamentales en árboles de decisión: el índice de Gini y la entropía. Explica qué mide cada criterio, cuándo un nodo es puro, cuándo hay máxima incertidumbre y cómo estos valores ayudan a elegir mejores divisiones dentro de un árbol.</p><p>Debe ubicarse antes de la construcción completa del bosque porque permite comprender cómo cada árbol decide sus cortes internos.</p></details> | Intermedio | Comparar criterios de impureza y comprender cómo se dividen los nodos. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_gini_entropia.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_gini_entropia.html) |
| **5** | **Random Forest · Bootstrap y Construcción Dinámica**<br><br><details><summary><strong>Resumen</strong></summary><p>Recurso avanzado que integra los elementos principales del algoritmo: bootstrap, selección aleatoria de variables, construcción dinámica de árboles, uso de Gini y votación final del bosque. Permite ver paso a paso cómo se genera cada árbol y cómo el conjunto produce una predicción colectiva.</p><p>Es el recurso central de síntesis visual, ideal para usar después de haber explicado muestreo con reposición, criterios de impureza y lógica de ensamble.</p></details> | Intermedio / Avanzado | Mostrar la construcción completa del árbol y del bosque de manera animada. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_boostrap.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_boostrap.html) |
| **6** | **Random Forest · Cuestionario Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Cuestionario de consolidación con preguntas desarrolladas sobre Random Forest. Incluye conceptos fundamentales, construcción interna del modelo, bootstrap, out-of-bag, Gini, entropía, clasificación, regresión, sobreajuste, sesgo-varianza, hiperparámetros, evaluación, interpretabilidad y comparación con otros métodos.</p><p>Debe ubicarse al final de la secuencia porque funciona como material de repaso, autoevaluación y cierre conceptual después de recorrer las simulaciones.</p></details> | Consolidación | Evaluar y reforzar la comprensión del algoritmo mediante preguntas desarrolladas. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_cuestionario.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_cuestionario.html) |
| **7** | **Random Forest · Glosario Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Glosario ampliado de Random Forest, pensado para estudiar el vocabulario técnico del tema de manera progresiva. Incluye términos vinculados con Machine Learning, árboles de decisión, clasificación, regresión, bootstrap, bagging, Random Forest, métricas, hiperparámetros, generalización, sesgo-varianza, interpretabilidad y herramientas prácticas.</p><p>Se ubica como cierre del bloque porque funciona como material permanente de consulta. Puede usarse antes de una clase para introducir conceptos, durante la clase para resolver dudas terminológicas o después como recurso de estudio autónomo.</p></details> | Consulta / Consolidación | Servir como diccionario técnico y guía de repaso conceptual. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_Glosario.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Random_Forest_Glosario.html) |

---

## 🧭 Secuencia sugerida de uso

```text
1. Sabiduría del Ensamble
        ↓
2. Tipos de Ensamble y Random Forest
        ↓
3. Muestreo con Reposición
        ↓
4. Gini y Entropía
        ↓
5. Bootstrap y Construcción Dinámica del Bosque
        ↓
6. Cuestionario Interactivo
        ↓
7. Glosario Interactivo

# 🧩 Clustering, K-Means y Clustering Jerárquico · Recursos interactivos de estudio

> Material organizado para estudiar **aprendizaje no supervisado**, **K-Means**, **clustering jerárquico**, **dendrogramas**, **distancias**, **escalado**, **métricas de evaluación** e **interpretación de clusters**.

---

## 🎯 Objetivo general del bloque

Este conjunto de recursos tiene como objetivo comprender el **clustering** como una técnica de **aprendizaje no supervisado** orientada a descubrir estructuras ocultas en los datos cuando no existe una etiqueta previa.

A diferencia del aprendizaje supervisado, donde el modelo aprende a predecir una respuesta conocida, el clustering busca identificar **grupos naturales** de observaciones a partir de la similitud entre ellas.

El bloque permite estudiar:

- qué es el aprendizaje no supervisado;
- qué significa agrupar observaciones sin etiquetas;
- cómo se define la similitud entre datos;
- por qué la distancia es central en clustering;
- cómo funciona K-Means;
- qué son los centroides;
- cómo se interpreta el método del codo;
- qué mide la silueta o silhouette;
- cómo funciona el clustering jerárquico;
- qué es un dendrograma;
- cómo se corta un árbol jerárquico;
- qué diferencias existen entre K-Means y clustering jerárquico;
- qué cuidados deben tenerse con escala, outliers y variables;
- cómo interpretar clusters de manera accionable.

---

## 🧭 Secuencia didáctica sugerida

```text
1. Clustering y aprendizaje no supervisado
        ↓
2. Distancia, similitud y escala
        ↓
3. K-Means y centroides
        ↓
4. Método del codo y silhouette
        ↓
5. Clustering jerárquico y dendrogramas
        ↓
6. Comparación entre métodos
        ↓
7. Cuestionario integrador
        ↓
8. Glosario interactivo

# K-Means · Recursos Interactivos para Clase

> **Versión 2.0 del bloque de recursos de K-Means**  
> Material organizado para estudiar, exponer y practicar el algoritmo **K-Means** mediante teoría visual, simulación interactiva, glosario, preguntas desarrolladas y práctica en Google Colab.

---

## Objetivo del bloque

Este bloque reúne recursos interactivos para comprender **K-Means** como algoritmo de **aprendizaje no supervisado**, mostrando cómo se forman clusters a partir de la distancia entre puntos y centroides.

La finalidad es que el estudiante pueda:

- comprender qué es clustering;
- diferenciar aprendizaje supervisado y no supervisado;
- interpretar el rol del número de clusters `K`;
- entender qué es un centroide;
- observar cómo se asignan puntos al centroide más cercano;
- visualizar cómo los centroides se recalculan;
- comprender la idea de convergencia;
- interpretar métricas como inercia y silhouette score;
- reconocer limitaciones del algoritmo;
- conectar la explicación visual con la implementación en Python.

---

## Secuencia didáctica sugerida

```text
1. Antes de la simulación
        ↓
2. Simulación interactiva
        ↓
3. Glosario de K-Means
        ↓
4. Preguntas y respuestas
        ↓
5. Práctica en Google Colab
````

---

## Recursos interactivos

| Orden | Recurso                                                        | Propósito didáctico                                                                                                                                                                                                       |                                                                                                                                                                                                                                                                                                                                     Acceso                                                                                                                                                                                                                                                                                                                                    |
| :---: | :------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| **1** | **K-Means antes de la simulación**                             | Presentar la intuición inicial del algoritmo, explicar qué se debe observar antes de ejecutar una simulación y preparar al estudiante para interpretar centroides, distancias, asignaciones y convergencia.               |                                [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-1f4e79?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20antes%20de%20la%20simulaci%C3%B3n.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20antes%20de%20la%20simulaci%C3%B3n.html)                                |
| **2** | **K-Means interactivo: centroides, asignación y convergencia** | Simulación principal para observar cómo los puntos se asignan al centroide más cercano, cómo los centroides se recalculan como promedios y cómo el algoritmo avanza hacia una solución estable.                           | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-7c3aed?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20interactivo%20centroides%2C%20asignaci%C3%B3n%20y%20convergencia.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20interactivo%20centroides%2C%20asignaci%C3%B3n%20y%20convergencia.html) |
| **3** | **K-Means Glosario**                                           | Material de consulta para consolidar los conceptos principales: cluster, K, centroide, distancia euclídea, asignación, iteración, convergencia, inercia, función objetivo, K-Means++, método del codo y silhouette score. |                                                         [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-15803d?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20Glosario.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20Glosario.html)                                                         |
| **4** | **K-Means preguntas y respuestas**                             | Guía de estudio con preguntas desarrolladas para repasar el algoritmo, verificar comprensión conceptual y preparar una explicación escrita u oral del tema.                                                               |                                               [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-f59e0b?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K_means_preguntas_respuestas.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K_means_preguntas_respuestas.html)                                               |
| **5** | **Notebook en Google Colab**                                   | Práctica complementaria para conectar la explicación conceptual y visual con código Python, experimentación y análisis de resultados.                                                                                     |                                                                                                                                                                                                                               [![Abrir Colab](https://img.shields.io/badge/Abrir%20Colab-f9ab00?style=for-the-badge\&logo=googlecolab\&logoColor=white)](https://colab.research.google.com/drive/10vG3vgMzM1C13ume1b7auFPwQRMh5uZW?usp=sharing)                                                                                                                                                                                                                               |

---

## Botones de acceso directo

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20antes%20de%20la%20simulaci%C3%B3n.html">
    <img src="https://img.shields.io/badge/1.%20Abrir%20HTML-Antes%20de%20la%20simulaci%C3%B3n-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Antes de la simulación">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20antes%20de%20la%20simulaci%C3%B3n.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20interactivo%20centroides%2C%20asignaci%C3%B3n%20y%20convergencia.html">
    <img src="https://img.shields.io/badge/2.%20Abrir%20HTML-Simulaci%C3%B3n%20interactiva-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Simulación interactiva">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20interactivo%20centroides%2C%20asignaci%C3%B3n%20y%20convergencia.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20Glosario.html">
    <img src="https://img.shields.io/badge/3.%20Abrir%20HTML-Glosario%20K--Means-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Glosario">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20Glosario.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K_means_preguntas_respuestas.html">
    <img src="https://img.shields.io/badge/4.%20Abrir%20HTML-Preguntas%20y%20respuestas-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Preguntas y respuestas">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K_means_preguntas_respuestas.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://colab.research.google.com/drive/10vG3vgMzM1C13ume1b7auFPwQRMh5uZW?usp=sharing">
    <img src="https://img.shields.io/badge/5.%20Abrir-Google%20Colab-f9ab00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Abrir Google Colab">
  </a>
</p>

---

## Resumen didáctico de cada recurso

### 1. K-Means antes de la simulación

Este recurso funciona como la **entrada conceptual al tema**. Su objetivo es preparar al estudiante para entender qué está viendo antes de ejecutar una simulación interactiva.

Permite trabajar:

* qué es clustering;
* qué significa agrupar datos sin etiquetas;
* qué representa el valor de `K`;
* qué es un centroide;
* qué significa distancia entre puntos;
* por qué los puntos se asignan al centroide más cercano;
* qué quiere decir recalcular centroides;
* qué significa que el algoritmo converge.

**Idea clave:**
Antes de mirar el algoritmo en movimiento, el estudiante necesita comprender que K-Means alterna dos operaciones principales: asignar puntos y recalcular centroides.

---

### 2. K-Means interactivo: centroides, asignación y convergencia

Este recurso funciona como el **laboratorio visual principal del módulo**. Permite observar el algoritmo funcionando paso a paso.

Permite trabajar:

* inicialización de centroides;
* asignación de puntos por cercanía;
* cambio de color de los puntos según el cluster;
* actualización de centroides;
* movimiento de los centroides;
* convergencia;
* escenarios con grupos separados;
* escenarios con grupos cercanos;
* datos desbalanceados;
* outliers;
* clusters alargados;
* datos aleatorios.

**Idea clave:**
K-Means no conoce etiquetas verdaderas. Construye grupos a partir de la cercanía geométrica entre puntos y centroides.

---

### 3. K-Means Glosario

Este recurso funciona como **material permanente de consulta**. El glosario permite ordenar el vocabulario técnico después de haber visto la explicación conceptual y la simulación.

Permite trabajar conceptos como:

* K-Means;
* cluster;
* número de clusters `K`;
* centroide;
* distancia euclídea;
* asignación de puntos;
* recalcular centroides;
* iteración;
* convergencia;
* inercia;
* función objetivo;
* inicialización;
* K-Means++;
* método del codo;
* silhouette score.

**Idea clave:**
El glosario ayuda a transformar la intuición visual en lenguaje técnico preciso.

---

### 4. K-Means preguntas y respuestas

Este recurso funciona como **guía de repaso y autoevaluación**. Está pensado para que el estudiante no solo vea la simulación, sino que pueda explicar el tema con claridad.

Permite trabajar:

* preguntas conceptuales;
* respuestas desarrolladas;
* relación entre centroides, distancias y clusters;
* diferencia entre inercia y silhouette score;
* elección de `K`;
* limitaciones del algoritmo;
* interpretación de resultados;
* preparación para exámenes o exposiciones.

**Idea clave:**
Si el estudiante puede responder estas preguntas con sus propias palabras, entonces comprendió la lógica del algoritmo y no solo memorizó sus pasos.

---

### 5. Notebook en Google Colab

El notebook permite llevar el tema a la práctica con Python.

Puede utilizarse para:

* cargar datos;
* ejecutar K-Means;
* visualizar clusters;
* calcular inercia;
* comparar distintos valores de `K`;
* analizar silhouette score;
* experimentar con escalado de variables;
* conectar teoría, simulación y código.

**Idea clave:**
Colab permite pasar de la intuición visual a la implementación práctica.

---

## Mapa conceptual del módulo

```text
K-Means
│
├── 1. Aprendizaje no supervisado
│   ├── Datos sin etiquetas
│   ├── Búsqueda de patrones
│   └── Descubrimiento de estructura
│
├── 2. Clustering
│   ├── Agrupar observaciones similares
│   ├── Medir distancia
│   ├── Comparar similitud
│   └── Interpretar grupos
│
├── 3. Componentes principales
│   ├── K
│   ├── Cluster
│   ├── Centroide
│   ├── Punto de datos
│   └── Distancia euclídea
│
├── 4. Proceso iterativo
│   ├── Inicializar centroides
│   ├── Asignar puntos al centroide más cercano
│   ├── Recalcular centroides
│   ├── Repetir
│   └── Converger
│
├── 5. Evaluación
│   ├── Inercia
│   ├── WCSS
│   ├── Método del codo
│   ├── Silhouette score
│   ├── Compactación
│   └── Separación
│
├── 6. Problemas frecuentes
│   ├── Mala elección de K
│   ├── Mala inicialización
│   ├── Variables sin escalar
│   ├── Outliers
│   ├── Clusters alargados
│   └── Clusters no esféricos
│
└── 7. Interpretación
    ├── Perfil de cada cluster
    ├── Segmentación
    ├── Comparación entre grupos
    ├── Decisión práctica
    └── Comunicación de resultados
```

---

## Guía rápida de lectura

### Para comenzar desde cero

Usar primero:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Antes%20de%20la%20simulaci%C3%B3n-1f4e79?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20antes%20de%20la%20simulaci%C3%B3n.html)

Este recurso permite presentar la intuición general del algoritmo y preparar la lectura de la simulación.

---

### Para explicar el algoritmo paso a paso

Usar después:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Simulaci%C3%B3n%20interactiva-7c3aed?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20interactivo%20centroides%2C%20asignaci%C3%B3n%20y%20convergencia.html)

La explicación puede seguir este flujo:

```text
Elegir K
        ↓
Inicializar centroides
        ↓
Asignar cada punto al centroide más cercano
        ↓
Recalcular centroides
        ↓
Repetir
        ↓
Obtener clusters finales
```

---

### Para consolidar vocabulario

Usar luego:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Glosario%20K--Means-15803d?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K-Means%20Glosario.html)

El glosario debe utilizarse después de la simulación, porque en ese momento los conceptos ya tienen una imagen mental asociada.

---

### Para repasar y evaluar

Usar al final:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Preguntas%20y%20respuestas-f59e0b?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/K_means_preguntas_respuestas.html)

Este recurso permite comprobar si el estudiante puede explicar el tema con claridad.

---

### Para practicar con Python

Usar como cierre práctico:

[![Abrir Colab](https://img.shields.io/badge/Abrir-Google%20Colab-f9ab00?style=for-the-badge\&logo=googlecolab\&logoColor=white)](https://colab.research.google.com/drive/10vG3vgMzM1C13ume1b7auFPwQRMh5uZW?usp=sharing)

---

## Desarrollo conceptual del tema

### Qué es K-Means

K-Means es un algoritmo de **aprendizaje no supervisado** que busca dividir un conjunto de datos en `K` grupos o clusters.

Cada cluster está representado por un **centroide**, que funciona como el punto promedio del grupo. El algoritmo intenta que los puntos de cada cluster estén lo más cerca posible de su centroide.

---

### Por qué se llama K-Means

El nombre tiene dos partes:

| Parte   | Significado                                       |
| :------ | :------------------------------------------------ |
| `K`     | Cantidad de clusters que se quieren formar        |
| `Means` | Medias o promedios que representan los centroides |

Por eso, K-Means puede entenderse como un algoritmo que busca formar `K` grupos alrededor de `K` promedios.

---

### Cómo funciona el algoritmo

El algoritmo sigue una lógica iterativa:

```text
1. Elegir la cantidad de clusters K.
2. Ubicar centroides iniciales.
3. Asignar cada punto al centroide más cercano.
4. Recalcular cada centroide como promedio de los puntos asignados.
5. Repetir los pasos 3 y 4 hasta que los centroides dejen de cambiar de manera significativa.
```

---

### Fórmula de asignación

Cada punto se asigna al cluster cuyo centroide esté más cerca.

```text
Asignar xᵢ al cluster Cⱼ si:

d(xᵢ, μⱼ) ≤ d(xᵢ, μₖ) para todo k
```

Donde:

* `xᵢ` es un punto del conjunto de datos.
* `μⱼ` es el centroide del cluster `j`.
* `d(xᵢ, μⱼ)` es la distancia entre el punto y el centroide.
* `k` recorre todos los centroides disponibles.

---

### Fórmula de actualización del centroide

Después de asignar los puntos, cada centroide se recalcula como el promedio de los puntos de su cluster.

```text
μⱼ = (1 / |Cⱼ|) Σ xᵢ
```

Donde:

* `μⱼ` es el nuevo centroide del cluster `j`.
* `Cⱼ` es el conjunto de puntos asignados al cluster.
* `|Cⱼ|` es la cantidad de puntos dentro del cluster.
* `Σ xᵢ` representa la suma de los puntos asignados.

---

### Función objetivo e inercia

K-Means busca minimizar la suma de las distancias cuadradas entre cada punto y el centroide de su cluster.

```text
Inercia = Σ Σ ||xᵢ - μⱼ||²
```

La inercia mide la compactación interna de los clusters.

| Valor de inercia | Interpretación                                                   |
| :--------------- | :--------------------------------------------------------------- |
| Baja             | Los puntos están cerca de sus centroides                         |
| Alta             | Los puntos están dispersos dentro de los clusters                |
| Cero             | Solo posible si cada punto coincide exactamente con su centroide |

---

### Método del codo

El método del codo ayuda a elegir un valor razonable de `K`.

La idea consiste en probar varios valores de `K` y observar cómo disminuye la inercia. Al aumentar `K`, la inercia siempre tiende a bajar, pero llega un punto donde agregar más clusters mejora poco.

Ese punto se conoce como **codo**.

```text
K aumenta
        ↓
La inercia baja
        ↓
La mejora empieza a ser menor
        ↓
Aparece el codo
        ↓
Se elige un K razonable
```

---

### Silhouette score

El silhouette score mide qué tan bien ubicado está un punto dentro de su cluster en comparación con los clusters vecinos.

```text
s(i) = (b(i) - a(i)) / max(a(i), b(i))
```

Donde:

* `a(i)` es la distancia promedio del punto `i` a los puntos de su propio cluster.
* `b(i)` es la menor distancia promedio del punto `i` a otro cluster cercano.
* `s(i)` es el silhouette score del punto.

Interpretación:

| Valor       | Interpretación                               |
| :---------- | :------------------------------------------- |
| Cercano a 1 | El punto está bien asignado                  |
| Cercano a 0 | El punto está en una frontera entre clusters |
| Negativo    | El punto podría estar mal asignado           |

---

## Comparación entre métricas

| Métrica            | Qué mide                                  | Cómo se interpreta                                |
| :----------------- | :---------------------------------------- | :------------------------------------------------ |
| Inercia            | Compactación interna                      | Cuanto menor, más compactos son los clusters      |
| Método del codo    | Cambio de la inercia al aumentar `K`      | Busca el punto donde agregar clusters mejora poco |
| Silhouette score   | Compactación interna y separación externa | Cuanto más cercano a 1, mejor es la estructura    |
| Distancia euclídea | Cercanía entre puntos                     | Define la asignación al centroide más cercano     |

---

## Limitaciones de K-Means

K-Means es muy útil, pero tiene limitaciones importantes.

Puede fallar o dar resultados poco interpretables cuando:

* los clusters tienen formas no circulares;
* los clusters son alargados;
* hay outliers;
* las variables no están escaladas;
* los grupos tienen tamaños muy desbalanceados;
* se elige mal el valor de `K`;
* la inicialización de centroides es mala;
* la distancia euclídea no representa bien la similitud real del problema.

---

## Uso sugerido para una clase

| Momento de la clase      | Recurso sugerido               | Actividad                                       |
| :----------------------- | :----------------------------- | :---------------------------------------------- |
| Inicio                   | K-Means antes de la simulación | Presentar la intuición general del algoritmo    |
| Desarrollo visual        | Simulación interactiva         | Mostrar centroides, asignaciones y convergencia |
| Consolidación conceptual | Glosario                       | Repasar términos técnicos                       |
| Repaso final             | Preguntas y respuestas         | Trabajar preguntas desarrolladas                |
| Práctica                 | Google Colab                   | Ejecutar K-Means en Python                      |

---

## Preguntas guía para trabajar en clase

1. ¿Qué significa que K-Means sea un algoritmo de aprendizaje no supervisado?
2. ¿Qué diferencia hay entre clustering y clasificación?
3. ¿Qué representa el valor `K`?
4. ¿Qué es un centroide?
5. ¿Por qué K-Means usa distancias?
6. ¿Cómo se asignan los puntos a los clusters?
7. ¿Cómo se recalcula un centroide?
8. ¿Qué significa que el algoritmo converge?
9. ¿Qué mide la inercia?
10. ¿Por qué la inercia disminuye cuando aumenta `K`?
11. ¿Qué problema intenta resolver el método del codo?
12. ¿Qué mide el silhouette score?
13. ¿Por qué es importante escalar las variables?
14. ¿Qué efecto pueden tener los outliers?
15. ¿Qué limitaciones tiene K-Means?

---

## Relación entre los recursos

| Concepto                   | Recurso principal      | Recurso complementario |
| :------------------------- | :--------------------- | :--------------------- |
| Aprendizaje no supervisado | Antes de la simulación | Glosario               |
| Clustering                 | Antes de la simulación | Preguntas y respuestas |
| K-Means                    | Simulación interactiva | Glosario               |
| Centroide                  | Simulación interactiva | Glosario               |
| Asignación de puntos       | Simulación interactiva | Preguntas y respuestas |
| Recalcular centroides      | Simulación interactiva | Glosario               |
| Convergencia               | Simulación interactiva | Preguntas y respuestas |
| Inercia                    | Glosario               | Colab                  |
| Método del codo            | Glosario               | Colab                  |
| Silhouette score           | Glosario               | Preguntas y respuestas |
| Limitaciones               | Preguntas y respuestas | Antes de la simulación |
| Implementación en Python   | Colab                  | Simulación interactiva |

---

## Guion breve para presentar el bloque

### Inicio

En este módulo vamos a estudiar **K-Means**, un algoritmo fundamental de aprendizaje no supervisado que permite descubrir grupos dentro de los datos sin partir de etiquetas previas.

La idea no es solamente memorizar los pasos del algoritmo, sino comprender su lógica geométrica: cómo se ubican los centroides, cómo los puntos se asignan por cercanía, cómo los centroides se recalculan y cómo el sistema converge hacia una partición estable.

---

### Paso 1 · Antes de la simulación

Primero vamos a revisar el recurso **K-Means antes de la simulación**, porque antes de mirar el algoritmo en movimiento necesitamos comprender qué representa cada elemento: los puntos, los centroides, la distancia, la cantidad de clusters y la convergencia.

---

### Paso 2 · Simulación interactiva

Luego vamos a trabajar con la **simulación interactiva de K-Means**, donde podremos observar el proceso paso a paso.

La simulación permite ver cómo los puntos se asignan al centroide más cercano, cómo los centroides se desplazan hacia el promedio de los puntos asignados y cómo, después de varias iteraciones, el algoritmo alcanza una configuración más estable.

---

### Paso 3 · Glosario

Después de la simulación vamos a utilizar el **glosario** para ordenar los conceptos centrales.

El objetivo del glosario es que cada estudiante pueda asociar lo que vio en la simulación con los términos técnicos del tema.

---

### Paso 4 · Preguntas y respuestas

Finalmente, vamos a cerrar con el recurso de **preguntas y respuestas**, que funciona como una guía de estudio.

Este recurso permite repasar los conceptos principales y verificar si realmente se comprendió la lógica del algoritmo, sus pasos, sus métricas y sus limitaciones.

---

### Paso 5 · Google Colab

Como cierre práctico, se puede abrir el notebook de **Google Colab** para conectar la explicación visual con código Python.

---

## Síntesis final

K-Means es una herramienta fundamental para introducir el aprendizaje no supervisado porque permite ver de manera clara cómo un algoritmo puede encontrar estructura en los datos sin necesidad de etiquetas previas.

Su valor pedagógico está en que combina:

* intuición geométrica;
* cálculo de distancias;
* actualización iterativa;
* evaluación mediante métricas;
* análisis crítico de limitaciones;
* implementación práctica en Python.

El recorrido recomendado para este módulo es comenzar con la explicación conceptual, continuar con la simulación interactiva, consolidar el vocabulario mediante el glosario, cerrar con preguntas desarrolladas y finalmente practicar en Colab.

---


## 📚 Recursos interactivos

| Orden | Recurso | Propósito didáctico | Acceso |
| :---: | :--- | :--- | :---: |
| **1** | **Clustering, K-Means y Jerárquico · Laboratorio Interactivo** | Presentar el tema completo mediante una guía visual e interactiva. Permite estudiar clustering no supervisado, K-Means, clustering jerárquico, dendrogramas, distancias, escala, método del codo y silhouette. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_Clustering_kmeans_Jerarquico.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_Clustering_kmeans_Jerarquico.html) |
| **2** | **Clustering, K-Means y Jerárquico · Cuestionario Interactivo** | Consolidar el aprendizaje mediante preguntas desarrolladas. Funciona como guía de estudio, repaso conceptual, preparación de examen o actividad de cierre. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_clustering_kmeans_jerarquico_cuestionario_v2.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_clustering_kmeans_jerarquico_cuestionario_v2.html) |
| **3** | **Clustering, K-Means y Jerárquico · Glosario Interactivo** | Servir como material permanente de consulta. Incluye conceptos sobre aprendizaje no supervisado, distancia, centroides, dendrogramas, linkage, preprocesamiento, métricas e interpretación de clusters. | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML-1f4e79?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_glosario_clustering_kmeans_jerarquico.html)<br>[![Ver código](https://img.shields.io/badge/Ver-código-0f766e?style=for-the-badge)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_glosario_clustering_kmeans_jerarquico.html) |

---

## 🧩 Resumen didáctico de cada recurso

### 1. Clustering, K-Means y Jerárquico · Laboratorio Interactivo

Este recurso funciona como el **material principal del bloque**. Presenta una guía visual e interactiva para comprender el clustering desde la intuición hasta la comparación técnica entre métodos.

Permite trabajar los conceptos centrales:

- clustering como técnica no supervisada;
- datos sin etiquetas;
- grupos naturales;
- distancia y similitud;
- K-Means;
- centroides;
- número de clusters K;
- método del codo;
- silhouette;
- clustering jerárquico;
- dendrogramas;
- linkage;
- escalado de variables;
- interpretación de resultados.

El laboratorio permite observar que **K-Means agrupa por proximidad a centros**, mientras que el **clustering jerárquico construye una historia de semejanzas entre observaciones**.

**Idea clave:**  
El clustering busca descubrir estructura latente en los datos. K-Means lo hace mediante centroides; el clustering jerárquico lo hace mediante un árbol de fusiones o separaciones.

---

### 2. Clustering, K-Means y Jerárquico · Cuestionario Interactivo

Este recurso funciona como **material de consolidación**. Está pensado para transformar la visualización y la teoría en comprensión conceptual.

Puede utilizarse para:

- repaso individual;
- actividad en clase;
- evaluación diagnóstica;
- preparación de parcial;
- discusión oral;
- cierre de unidad;
- guía de estudio autónomo.

El cuestionario permite trabajar preguntas sobre:

- qué es clustering;
- qué es aprendizaje no supervisado;
- diferencia entre clustering y clasificación;
- funcionamiento de K-Means;
- rol de los centroides;
- elección del número de clusters;
- método del codo;
- silhouette;
- clustering jerárquico;
- dendrogramas;
- criterios de linkage;
- interpretación de clusters;
- ventajas y limitaciones de cada método.

**Idea clave:**  
El cuestionario ayuda a que el estudiante no solo vea la simulación, sino que pueda explicar el tema con lenguaje técnico y ejemplos.

---

### 3. Clustering, K-Means y Jerárquico · Glosario Interactivo

Este recurso funciona como **material permanente de consulta**. El glosario organiza los conceptos del tema en categorías y permite reforzar el vocabulario técnico necesario para estudiar clustering.

Incluye conceptos relacionados con:

- aprendizaje automático;
- aprendizaje supervisado;
- aprendizaje no supervisado;
- clustering;
- observaciones;
- variables;
- espacio de características;
- distancia;
- similitud;
- K-Means;
- centroides;
- inicialización;
- K-Means++;
- WCSS;
- método del codo;
- silhouette;
- clustering jerárquico;
- dendrograma;
- linkage;
- single linkage;
- complete linkage;
- average linkage;
- Ward;
- escalado;
- normalización;
- estandarización;
- outliers;
- reducción de dimensionalidad;
- PCA;
- interpretación de clusters.

**Idea clave:**  
El glosario permite que el estudiante conecte términos técnicos con intuiciones, ejemplos y usos prácticos.

---

## 🧠 Mapa conceptual del bloque

```text
Clustering
│
├── 1. Aprendizaje automático
│   ├── Aprendizaje supervisado
│   ├── Aprendizaje no supervisado
│   └── Descubrimiento de patrones
│
├── 2. Problema central
│   ├── Datos sin etiquetas
│   ├── Observaciones
│   ├── Variables
│   ├── Similitud
│   └── Distancia
│
├── 3. K-Means
│   ├── Elegir K
│   ├── Inicializar centroides
│   ├── Asignar puntos al centro más cercano
│   ├── Recalcular centroides
│   ├── Repetir hasta converger
│   └── Interpretar clusters
│
├── 4. Evaluación de K-Means
│   ├── WCSS
│   ├── Método del codo
│   ├── Silhouette
│   ├── Compactación
│   └── Separación
│
├── 5. Clustering jerárquico
│   ├── Enfoque aglomerativo
│   ├── Enfoque divisivo
│   ├── Dendrograma
│   ├── Altura de corte
│   └── Número de clusters
│
├── 6. Linkage
│   ├── Single linkage
│   ├── Complete linkage
│   ├── Average linkage
│   └── Ward
│
├── 7. Preprocesamiento
│   ├── Escalado
│   ├── Normalización
│   ├── Estandarización
│   ├── Outliers
│   └── Variables irrelevantes
│
└── 8. Interpretación
    ├── Perfil de cluster
    ├── Segmentos accionables
    ├── Visualización
    ├── Validación
    └── Decisión práctica
```

---

## 🔎 Guía rápida de lectura

### Para comenzar desde cero

Usar primero:

1. **Clustering, K-Means y Jerárquico · Laboratorio Interactivo**

Este recurso permite presentar la intuición general del tema. Es recomendable comenzar mostrando que el clustering busca descubrir grupos sin una etiqueta previa.

---

### Para explicar K-Means

Dentro del laboratorio principal, trabajar especialmente:

- centroides;
- elección de K;
- asignación de puntos;
- actualización de centroides;
- convergencia;
- método del codo;
- silhouette.

La explicación puede seguir este flujo:

```text
Elegir K
        ↓
Inicializar centroides
        ↓
Asignar cada punto al centroide más cercano
        ↓
Recalcular centroides
        ↓
Repetir
        ↓
Obtener clusters finales
```

---

### Para explicar clustering jerárquico

Dentro del laboratorio principal, trabajar:

- dendrograma;
- fusión de observaciones;
- altura de unión;
- criterio de linkage;
- corte del árbol;
- interpretación del número de clusters.

La explicación puede seguir este flujo:

```text
Calcular distancias
        ↓
Unir observaciones o grupos más parecidos
        ↓
Actualizar distancias entre grupos
        ↓
Repetir fusiones
        ↓
Construir dendrograma
        ↓
Cortar el árbol para definir clusters
```

---

### Para repasar y evaluar

Usar al final:

2. **Cuestionario Interactivo**
3. **Glosario Interactivo**

El cuestionario sirve para consolidar comprensión.  
El glosario sirve como material de consulta y repaso conceptual.

---

## 🧩 Comparación entre K-Means y Clustering Jerárquico

| Criterio | K-Means | Clustering jerárquico |
| :--- | :--- | :--- |
| Tipo de método | Particional | Jerárquico |
| Idea central | Agrupar puntos alrededor de centroides | Construir una estructura de semejanzas |
| Resultado principal | K clusters y sus centroides | Dendrograma |
| Necesita elegir K al inicio | Sí | No necesariamente |
| Representación visual | Centros y grupos en el espacio | Árbol de fusiones o divisiones |
| Sensibilidad a la escala | Alta | Alta |
| Sensibilidad a outliers | Alta | Depende del linkage |
| Interpretabilidad | Buena si los clusters son compactos | Muy buena por el dendrograma |
| Costo computacional | Más eficiente en datasets grandes | Más costoso en datasets grandes |
| Mejor uso | Segmentación rápida con muchos datos | Exploración e interpretación de estructura |
| Limitación típica | Puede fallar con clusters no esféricos | Puede ser costoso y sensible al criterio de linkage |

---

## 🧪 Preguntas guía para trabajar en clase

1. ¿Qué significa que el clustering sea una técnica de aprendizaje no supervisado?
2. ¿Cuál es la diferencia entre clasificación y clustering?
3. ¿Por qué la distancia es tan importante para agrupar datos?
4. ¿Qué ocurre si las variables están en escalas muy diferentes?
5. ¿Qué es un centroide en K-Means?
6. ¿Por qué K-Means necesita definir K antes de entrenar?
7. ¿Qué problema intenta resolver el método del codo?
8. ¿Qué mide el coeficiente silhouette?
9. ¿Qué es un dendrograma?
10. ¿Cómo se decide el número de clusters en clustering jerárquico?
11. ¿Qué diferencia hay entre single linkage y complete linkage?
12. ¿Por qué los outliers pueden afectar el resultado?
13. ¿Qué significa que un cluster sea compacto?
14. ¿Qué significa que dos clusters estén bien separados?
15. ¿Cómo se interpreta un cluster en un problema real?
16. ¿Por qué clustering no debe confundirse con predicción supervisada?
17. ¿Qué ventajas tiene K-Means?
18. ¿Qué ventajas tiene el clustering jerárquico?
19. ¿Cuándo conviene usar K-Means?
20. ¿Cuándo conviene usar clustering jerárquico?

---

## 🧑‍🏫 Uso sugerido para una clase

| Momento de la clase | Recurso sugerido | Actividad |
| :--- | :--- | :--- |
| Inicio | Laboratorio Interactivo | Presentar la idea de agrupar sin etiquetas. |
| Desarrollo conceptual | Laboratorio Interactivo | Explicar distancia, similitud y clusters. |
| Desarrollo técnico I | Laboratorio Interactivo | Mostrar el funcionamiento de K-Means. |
| Desarrollo técnico II | Laboratorio Interactivo | Explicar dendrogramas y clustering jerárquico. |
| Comparación | Laboratorio Interactivo | Comparar ventajas y limitaciones de cada método. |
| Cierre | Cuestionario Interactivo | Repasar con preguntas desarrolladas. |
| Estudio autónomo | Glosario Interactivo | Consultar definiciones y reforzar vocabulario técnico. |

---

## 🧩 Relación entre los recursos

| Concepto | Recurso principal | Recurso complementario |
| :--- | :--- | :--- |
| Aprendizaje no supervisado | Laboratorio Interactivo | Glosario |
| Clustering | Laboratorio Interactivo | Cuestionario |
| Distancia | Laboratorio Interactivo | Glosario |
| Similitud | Laboratorio Interactivo | Glosario |
| K-Means | Laboratorio Interactivo | Cuestionario |
| Centroide | Laboratorio Interactivo | Glosario |
| Número de clusters K | Laboratorio Interactivo | Cuestionario |
| Método del codo | Laboratorio Interactivo | Glosario |
| Silhouette | Laboratorio Interactivo | Cuestionario |
| Clustering jerárquico | Laboratorio Interactivo | Cuestionario |
| Dendrograma | Laboratorio Interactivo | Glosario |
| Linkage | Laboratorio Interactivo | Glosario |
| Escalado | Glosario | Cuestionario |
| Outliers | Glosario | Cuestionario |
| Interpretación de clusters | Cuestionario | Glosario |
| Repaso conceptual | Cuestionario | Glosario |

---

## 🧠 Síntesis conceptual

### Clustering

El clustering es una técnica que busca agrupar observaciones parecidas entre sí. No parte de etiquetas conocidas, sino que intenta descubrir una estructura latente dentro de los datos.

---

### K-Means

K-Means agrupa observaciones alrededor de centroides. El algoritmo necesita que se defina previamente el número de clusters K. Luego asigna puntos al centroide más cercano, recalcula los centroides y repite el proceso hasta estabilizar los grupos.

---

### Clustering jerárquico

El clustering jerárquico construye una estructura en forma de árbol. Esa estructura se representa mediante un dendrograma, que permite observar en qué orden se fusionan las observaciones o grupos y a qué distancia ocurre cada unión.

---

### Dendrograma

El dendrograma es una representación visual de las relaciones jerárquicas entre observaciones o grupos. Permite decidir el número de clusters cortando el árbol a una determinada altura.

---

### Distancia

La distancia define qué tan parecidas o diferentes son dos observaciones. En clustering, elegir una medida de distancia adecuada es fundamental, porque el algoritmo agrupa según esa noción de cercanía.

---

### Escalado

El escalado evita que una variable domine artificialmente el cálculo de distancias por estar medida en unidades mayores. En clustering, escalar las variables suele ser una práctica necesaria.

---

## 📌 Tabla de links directos

| Archivo | Abrir en HTML | Ver código en GitHub |
| :--- | :---: | :---: |
| `KNN_Clustering_kmeans_Jerarquico.html` | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-1f4e79?style=for-the-badge&logo=html5&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_Clustering_kmeans_Jerarquico.html) | [![Ver código](https://img.shields.io/badge/Ver%20código-0f766e?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_Clustering_kmeans_Jerarquico.html) |
| `KNN_clustering_kmeans_jerarquico_cuestionario_v2.html` | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-1f4e79?style=for-the-badge&logo=html5&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_clustering_kmeans_jerarquico_cuestionario_v2.html) | [![Ver código](https://img.shields.io/badge/Ver%20código-0f766e?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_clustering_kmeans_jerarquico_cuestionario_v2.html) |
| `KNN_glosario_clustering_kmeans_jerarquico.html` | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-1f4e79?style=for-the-badge&logo=html5&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_glosario_clustering_kmeans_jerarquico.html) | [![Ver código](https://img.shields.io/badge/Ver%20código-0f766e?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/KNN_glosario_clustering_kmeans_jerarquico.html) |

---

# 📘 Parcial Ciencia de Datos · Banco de Preguntas y Glosario Interactivo

> Material organizado para estudiar, repasar y consolidar los conceptos principales de Ciencia de Datos mediante un **banco de preguntas** y un **glosario interactivo**.

---

## 🎯 Objetivo general del bloque

Este bloque reúne dos recursos centrales para preparar el parcial de Ciencia de Datos:

1. **Banco de preguntas del parcial**, orientado a practicar respuestas completas, desarrollar argumentos técnicos y revisar conceptos clave.
2. **Glosario del parcial**, pensado como material permanente de consulta para reforzar vocabulario, definiciones y relaciones entre conceptos.

La finalidad es que el estudiante no solo memorice términos, sino que pueda:

- explicar conceptos con claridad;
- relacionar ideas entre sí;
- responder preguntas de examen con desarrollo;
- diferenciar técnicas, modelos y enfoques;
- reconocer aplicaciones prácticas;
- preparar una respuesta escrita más sólida;
- usar el glosario como guía de repaso rápido.

---

## 🧭 Secuencia didáctica sugerida

```text
1. Revisar el glosario
        ↓
2. Identificar conceptos centrales
        ↓
3. Resolver preguntas del banco
        ↓
4. Comparar respuestas con definiciones
        ↓
5. Reforzar conceptos débiles
        ↓
6. Repasar antes del parcial
```

---

## 📚 Recursos interactivos

| Orden | Recurso | Propósito didáctico | Acceso |
| :---: | :--- | :--- | :---: |
| **1** | **Banco de Preguntas · Parcial Ciencia de Datos** | Practicar preguntas posibles del parcial con respuestas desarrolladas, orientadas a consolidar comprensión conceptual y capacidad de explicación. | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-1f4e79?style=for-the-badge&logo=html5&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Banco_preguntas_parcial_ciencia_datos.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20código-0f766e?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Banco_preguntas_parcial_ciencia_datos.html) |
| **2** | **Glosario · Parcial Ciencia de Datos** | Consultar definiciones, términos técnicos y relaciones conceptuales fundamentales para estudiar el parcial. | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-7c3aed?style=for-the-badge&logo=html5&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Glosario_parcial_ciencia_datos.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20código-f59e0b?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Glosario_parcial_ciencia_datos.html) |

---

## 🧩 Resumen didáctico de cada recurso

### 1. Banco de Preguntas · Parcial Ciencia de Datos

Este recurso funciona como una **guía de práctica para el parcial**. Su objetivo principal es ayudar al estudiante a entrenar la capacidad de responder preguntas con desarrollo, precisión conceptual y ejemplos.

Puede utilizarse para:

- repasar antes del examen;
- practicar respuestas escritas;
- identificar temas que necesitan refuerzo;
- preparar explicaciones orales;
- construir una guía de estudio personal;
- simular una instancia de parcial;
- comparar conceptos relacionados.

El banco de preguntas permite transformar el estudio pasivo en una práctica activa. En lugar de solo leer definiciones, el estudiante debe explicar, conectar, justificar y aplicar conceptos.

**Idea clave:**  
El banco de preguntas sirve para comprobar si el estudiante realmente puede expresar lo que entiende.

---

### 2. Glosario · Parcial Ciencia de Datos

Este recurso funciona como **material de consulta permanente**. Reúne conceptos centrales que pueden aparecer en el parcial y permite revisar definiciones de manera rápida y ordenada.

Puede utilizarse para:

- repasar vocabulario técnico;
- aclarar dudas conceptuales;
- estudiar antes de responder preguntas;
- revisar diferencias entre términos;
- construir mapas conceptuales;
- preparar explicaciones más precisas;
- reforzar temas antes del examen.

El glosario es especialmente útil porque en Ciencia de Datos muchos conceptos están conectados: datos, variables, modelos, entrenamiento, evaluación, overfitting, métricas, clasificación, regresión, clustering y validación.

**Idea clave:**  
El glosario permite estudiar los conceptos como una red de ideas, no como definiciones aisladas.

---

## 🧠 Mapa conceptual del bloque

```text
Parcial Ciencia de Datos
│
├── 1. Conceptos fundamentales
│   ├── Ciencia de Datos
│   ├── Datos
│   ├── Dataset
│   ├── Variables
│   ├── Observaciones
│   └── Problema de negocio
│
├── 2. Aprendizaje automático
│   ├── Machine Learning
│   ├── Aprendizaje supervisado
│   ├── Aprendizaje no supervisado
│   ├── Clasificación
│   ├── Regresión
│   └── Clustering
│
├── 3. Modelos y entrenamiento
│   ├── Entrenamiento
│   ├── Test
│   ├── Validación
│   ├── Generalización
│   ├── Overfitting
│   └── Underfitting
│
├── 4. Evaluación
│   ├── Accuracy
│   ├── Precision
│   ├── Recall
│   ├── F1-score
│   ├── Matriz de confusión
│   └── Métricas de error
│
├── 5. Modelos frecuentes
│   ├── Árboles de decisión
│   ├── Random Forest
│   ├── KNN
│   ├── K-Means
│   └── Clustering jerárquico
│
└── 6. Preparación del parcial
    ├── Glosario
    ├── Banco de preguntas
    ├── Respuestas desarrolladas
    ├── Comparación de conceptos
    └── Repaso final
```

---

## 🔎 Guía rápida de uso

### Para estudiar desde cero

Usar primero:

1. **Glosario · Parcial Ciencia de Datos**
2. **Banco de Preguntas · Parcial Ciencia de Datos**

Primero conviene revisar los términos principales y luego practicar las preguntas.

---

### Para preparar el parcial

La secuencia recomendada es:

```text
Leer definición
        ↓
Explicar con tus palabras
        ↓
Resolver una pregunta relacionada
        ↓
Comparar con el glosario
        ↓
Corregir y ampliar la respuesta
```

---

### Para repasar el día anterior

Usar el siguiente recorrido:

```text
1. Revisar conceptos débiles
2. Leer preguntas clave
3. Practicar respuestas cortas
4. Repasar diferencias entre modelos
5. Revisar métricas de evaluación
6. Cerrar con el mapa conceptual
```

---

## 🧩 Relación entre los recursos

| Necesidad de estudio | Recurso recomendado | Uso sugerido |
| :--- | :--- | :--- |
| Entender conceptos básicos | Glosario | Leer definiciones y conectar conceptos. |
| Practicar respuestas | Banco de preguntas | Responder sin mirar y luego revisar. |
| Preparar examen escrito | Banco de preguntas | Desarrollar respuestas completas. |
| Repasar vocabulario técnico | Glosario | Usar como diccionario conceptual. |
| Identificar temas débiles | Banco de preguntas | Marcar preguntas difíciles. |
| Mejorar precisión conceptual | Glosario | Revisar definiciones exactas. |
| Hacer repaso final | Ambos recursos | Alternar preguntas y definiciones. |

---

## 🧪 Preguntas guía para trabajar en clase

1. ¿Qué diferencia hay entre datos, información y conocimiento?
2. ¿Qué es un dataset?
3. ¿Qué diferencia hay entre variable y observación?
4. ¿Qué es Ciencia de Datos?
5. ¿Qué relación existe entre Ciencia de Datos, Estadística y Machine Learning?
6. ¿Qué es aprendizaje supervisado?
7. ¿Qué es aprendizaje no supervisado?
8. ¿Cuál es la diferencia entre clasificación y regresión?
9. ¿Qué es clustering?
10. ¿Qué significa entrenar un modelo?
11. ¿Por qué se divide un dataset en entrenamiento y prueba?
12. ¿Qué significa que un modelo generalice bien?
13. ¿Qué es overfitting?
14. ¿Qué es underfitting?
15. ¿Qué es una matriz de confusión?
16. ¿Qué mide accuracy?
17. ¿Qué mide precision?
18. ¿Qué mide recall?
19. ¿Qué mide F1-score?
20. ¿Por qué no alcanza con mirar una sola métrica?

---

## 🧑‍🏫 Uso sugerido para una clase

| Momento de la clase | Recurso sugerido | Actividad |
| :--- | :--- | :--- |
| Inicio | Glosario | Repasar conceptos centrales del parcial. |
| Desarrollo | Banco de preguntas | Resolver preguntas seleccionadas. |
| Discusión | Banco de preguntas | Comparar respuestas entre estudiantes. |
| Corrección | Glosario | Ajustar vocabulario y precisión conceptual. |
| Cierre | Ambos recursos | Armar mapa de temas prioritarios. |
| Estudio autónomo | Glosario | Repasar definiciones antes del examen. |
| Preparación final | Banco de preguntas | Simular respuestas de parcial. |

---

## 🧠 Estrategia de estudio recomendada

### Paso 1 · Lectura del glosario

Leer primero las definiciones generales para construir una base conceptual.

```text
Concepto
        ↓
Definición
        ↓
Ejemplo
        ↓
Relación con otros conceptos
```

---

### Paso 2 · Resolución del banco de preguntas

Responder las preguntas sin mirar el glosario. Luego revisar si la respuesta fue clara, completa y técnicamente correcta.

```text
Pregunta
        ↓
Respuesta propia
        ↓
Comparación con el material
        ↓
Corrección
        ↓
Versión final
```

---

### Paso 3 · Repaso cruzado

Relacionar cada pregunta con uno o más términos del glosario.

| Pregunta | Conceptos que conviene revisar |
| :--- | :--- |
| Preguntas sobre modelos | Machine Learning, entrenamiento, validación, generalización |
| Preguntas sobre clasificación | Variable objetivo, clases, accuracy, matriz de confusión |
| Preguntas sobre regresión | Variable numérica, error, predicción, evaluación |
| Preguntas sobre clustering | Aprendizaje no supervisado, distancia, grupos, similitud |
| Preguntas sobre métricas | Accuracy, precision, recall, F1-score |
| Preguntas sobre sobreajuste | Overfitting, underfitting, sesgo, varianza |

---

## 📌 Tabla de links directos

| Archivo | Abrir en HTML | Ver código en GitHub |
| :--- | :---: | :---: |
| `Banco_preguntas_parcial_ciencia_datos.html` | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-1f4e79?style=for-the-badge&logo=html5&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Banco_preguntas_parcial_ciencia_datos.html) | [![Ver código](https://img.shields.io/badge/Ver%20código-0f766e?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Banco_preguntas_parcial_ciencia_datos.html) |
| `Glosario_parcial_ciencia_datos.html` | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-7c3aed?style=for-the-badge&logo=html5&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Glosario_parcial_ciencia_datos.html) | [![Ver código](https://img.shields.io/badge/Ver%20código-f59e0b?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Glosario_parcial_ciencia_datos.html) |

---

## 🧠 Frase síntesis

> El glosario permite comprender los conceptos; el banco de preguntas permite comprobar si realmente podemos explicarlos.

---

## ⚠️ Nota sobre los archivos

Los archivos incluidos en este bloque son:

```text
Banco_preguntas_parcial_ciencia_datos.html
Glosario_parcial_ciencia_datos.html
```
Tomé el modelo que pasaste y lo adapté al bloque de **Clustering Jerárquico**, dejando los botones directos a **HTML renderizado**, **código en GitHub** y **Google Colab**, con una estructura más parecida al ejemplo que compartiste. 

````markdown
# Clustering Jerárquico · Recursos Interactivos para Clase

> Material elaborado por el profesor Sergio Gevatschnaider

Este bloque reúne recursos interactivos para comprender **Clustering Jerárquico** como técnica de **aprendizaje no supervisado**, mostrando cómo se forman grupos a partir de distancias, fusiones sucesivas, matriz linkage, dendrogramas y corte del árbol.

La finalidad es que el estudiante pueda:

- comprender qué es clustering jerárquico;
- diferenciarlo de K-Means;
- interpretar la lógica de las fusiones;
- entender qué representa una matriz linkage;
- leer un dendrograma completo y truncado;
- comprender los métodos de linkage;
- interpretar el método Ward;
- decidir dónde cortar el dendrograma;
- reconocer ventajas, limitaciones y cuidados del método;
- conectar la explicación visual con una implementación en Python mediante Google Colab.

---

## Objetivo general del bloque

Este conjunto de recursos tiene como objetivo comprender el **clustering jerárquico aglomerativo** como un método que construye una estructura progresiva de agrupamiento.

A diferencia de K-Means, donde se define previamente una cantidad de clusters `K` y se trabaja con centroides, el clustering jerárquico comienza considerando que cada observación es su propio cluster y luego va fusionando puntos o grupos hasta construir un árbol completo.

El bloque permite estudiar:

- qué es el aprendizaje no supervisado;
- qué significa agrupar observaciones sin etiquetas;
- por qué la distancia es central en clustering;
- qué son las fusiones;
- qué es la matriz linkage;
- cómo se interpreta un dendrograma;
- qué diferencia hay entre dendrograma completo y truncado;
- qué significa cortar el árbol;
- cómo funcionan single linkage, complete linkage, average linkage y Ward;
- qué diferencias existen entre K-Means y clustering jerárquico;
- qué cuidados deben tenerse con escala, outliers y variables;
- cómo aplicar el método en Python.

---

## Secuencia didáctica sugerida

```text
1. Clase teórica visual
        ↓
2. Simulación interactiva de fusiones
        ↓
3. Cuestionario desarrollado
        ↓
4. Glosario interactivo
        ↓
5. Práctica en Google Colab
````

---

## Recursos interactivos

| Orden | Recurso                                                                               | Propósito didáctico                                                                                                                                                                                                                                      |                                                                                                                                                                                                                                                                                                                                                                 Acceso                                                                                                                                                                                                                                                                                                                                                                 |
| :---: | :------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| **1** | **Clustering Jerárquico · Clase teórica visual**                                      | Presentar la intuición inicial del método antes de ejecutar una simulación. Explica qué es clustering jerárquico, qué son las distancias, las fusiones, la matriz linkage, el dendrograma y el corte del árbol.                                          |                              [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Clase%20te%C3%B3rica-1f4e79?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Clase%20te%C3%B3rica%20visual.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Clase%20te%C3%B3rica%20visual.html)                             |
| **2** | **Clustering Jerárquico · Simulación interactiva de fusiones, linkage y dendrograma** | Simulación principal para observar cómo cada punto comienza como un cluster individual, cómo se realizan fusiones, cómo se registra la matriz linkage y cómo se construye el dendrograma.                                                                | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Simulaci%C3%B3n%20interactiva-7c3aed?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Interactivo%20fusiones%2C%20linkage%20y%20dendrograma.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Interactivo%20fusiones%2C%20linkage%20y%20dendrograma.html) |
| **3** | **Clustering Jerárquico · Cuestionario interactivo**                                  | Consolidar el aprendizaje mediante preguntas desarrolladas. Funciona como guía de estudio, repaso conceptual, preparación de examen o actividad de cierre.                                                                                               |                                                     [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Cuestionario-f59e0b?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Cuestionario.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Cuestionario.html)                                                    |
| **4** | **Clustering Jerárquico · Glosario interactivo**                                      | Servir como material permanente de consulta. Incluye conceptos sobre aprendizaje no supervisado, distancia, matriz de distancias, fusión, linkage, Ward, matriz linkage, dendrograma, altura de fusión, corte del árbol, estandarización y limitaciones. |                                                           [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Glosario-15803d?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Glosario.html)<br>[![Ver código](https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Glosario.html)                                                          |
| **5** | **Notebook en Google Colab**                                                          | Práctica complementaria para conectar la explicación conceptual y visual con código Python, experimentación, dendrogramas, corte del árbol y análisis de resultados.                                                                                     |                                                                                                                                                                                                                                                            [![Abrir Colab](https://img.shields.io/badge/Abrir%20Colab-f9ab00?style=for-the-badge\&logo=googlecolab\&logoColor=white)](https://colab.research.google.com/drive/1CiEih8HEVCWCQHWoBQnRGfosDcfiINFi?usp=sharing)                                                                                                                                                                                                                                                           |

---

## Botones de acceso directo

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Clase%20te%C3%B3rica%20visual.html">
    <img src="https://img.shields.io/badge/1.%20Abrir%20HTML-Clase%20te%C3%B3rica%20visual-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Clase teórica visual">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Clase%20te%C3%B3rica%20visual.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Interactivo%20fusiones%2C%20linkage%20y%20dendrograma.html">
    <img src="https://img.shields.io/badge/2.%20Abrir%20HTML-Simulaci%C3%B3n%20interactiva-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Simulación interactiva">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Interactivo%20fusiones%2C%20linkage%20y%20dendrograma.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Cuestionario.html">
    <img src="https://img.shields.io/badge/3.%20Abrir%20HTML-Cuestionario-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Cuestionario">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Cuestionario.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Glosario.html">
    <img src="https://img.shields.io/badge/4.%20Abrir%20HTML-Glosario-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir HTML Glosario">
  </a>
  <a href="https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Glosario.html">
    <img src="https://img.shields.io/badge/Ver%20c%C3%B3digo-GitHub-0f766e?style=for-the-badge&logo=github&logoColor=white" alt="Ver código en GitHub">
  </a>
</p>

<p align="center">
  <a href="https://colab.research.google.com/drive/1CiEih8HEVCWCQHWoBQnRGfosDcfiINFi?usp=sharing">
    <img src="https://img.shields.io/badge/5.%20Abrir-Google%20Colab-f9ab00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Abrir Google Colab">
  </a>
</p>

---

## Resumen didáctico de cada recurso

### 1. Clustering Jerárquico · Clase teórica visual

Este recurso funciona como la **entrada conceptual al tema**. Su objetivo es preparar al estudiante para entender qué está viendo antes de ejecutar una simulación interactiva.

Permite trabajar:

* qué es clustering jerárquico;
* qué significa agrupar datos sin etiquetas;
* qué representa una distancia;
* qué significa fusionar puntos o grupos;
* qué es una matriz linkage;
* cómo se interpreta un dendrograma;
* cómo se decide dónde cortar el árbol.

**Idea clave:**
Antes de mirar el algoritmo en movimiento, el estudiante necesita comprender que el clustering jerárquico no mueve centroides, sino que construye una historia de fusiones.

---

### 2. Clustering Jerárquico · Simulación interactiva

Este recurso funciona como el **laboratorio visual principal del módulo**. Permite observar el algoritmo funcionando paso a paso.

Permite trabajar:

* puntos iniciales como clusters individuales;
* fusiones sucesivas;
* reducción progresiva del número de clusters;
* comparación de métodos de linkage;
* matriz linkage;
* dendrograma;
* línea de corte;
* cantidad de clusters resultantes;
* escenarios con grupos separados, grupos cercanos, outliers, clusters alargados y datos aleatorios.

**Idea clave:**
El clustering jerárquico no conoce etiquetas verdaderas. Construye una estructura de agrupamiento a partir de distancias y criterios de enlace.

---

### 3. Clustering Jerárquico · Cuestionario interactivo

Este recurso funciona como **guía de repaso y autoevaluación**. Está pensado para que el estudiante no solo vea la simulación, sino que pueda explicar el tema con claridad.

Permite trabajar:

* preguntas conceptuales;
* respuestas desarrolladas;
* aprendizaje no supervisado;
* distancias;
* fusiones;
* linkage;
* Ward;
* matriz linkage;
* dendrograma;
* corte del árbol;
* ventajas y limitaciones;
* comparación con K-Means.

**Idea clave:**
Si el estudiante puede responder estas preguntas con sus propias palabras, entonces comprendió la lógica del algoritmo y no solo memorizó sus pasos.

---

### 4. Clustering Jerárquico · Glosario interactivo

Este recurso funciona como **material permanente de consulta**. El glosario permite ordenar el vocabulario técnico después de haber visto la explicación conceptual y la simulación.

Permite trabajar conceptos como:

* clustering jerárquico;
* aprendizaje no supervisado;
* observación;
* cluster;
* distancia;
* matriz de distancias;
* fusión;
* linkage;
* single linkage;
* complete linkage;
* average linkage;
* método Ward;
* matriz linkage;
* dendrograma;
* altura de fusión;
* corte del árbol;
* estandarización;
* outliers;
* limitaciones del método.

**Idea clave:**
El glosario ayuda a transformar la intuición visual en lenguaje técnico preciso.

---

### 5. Notebook en Google Colab

El notebook permite llevar el tema a la práctica con Python.

Puede utilizarse para:

* generar datos sintéticos;
* estandarizar variables;
* calcular distancias;
* construir la matriz linkage;
* graficar dendrogramas completos;
* graficar dendrogramas truncados;
* cortar el árbol;
* asignar clusters;
* calcular silhouette score;
* comparar métodos de linkage;
* interpretar resultados.

**Idea clave:**
Colab permite pasar de la intuición visual a la implementación práctica.

---

## Mapa conceptual del módulo

```text
Clustering Jerárquico
│
├── 1. Aprendizaje no supervisado
│   ├── Datos sin etiquetas
│   ├── Búsqueda de patrones
│   └── Descubrimiento de estructura
│
├── 2. Distancia y similitud
│   ├── Distancia euclídea
│   ├── Distancia Manhattan
│   ├── Distancia coseno
│   ├── Escala de variables
│   └── Estandarización
│
├── 3. Proceso aglomerativo
│   ├── Cada punto empieza como cluster
│   ├── Se calculan distancias
│   ├── Se elige una fusión
│   ├── Se crea un nuevo cluster
│   └── Se repite hasta formar un árbol
│
├── 4. Linkage
│   ├── Single linkage
│   ├── Complete linkage
│   ├── Average linkage
│   └── Ward
│
├── 5. Matriz linkage
│   ├── Primer elemento fusionado
│   ├── Segundo elemento fusionado
│   ├── Distancia de fusión
│   └── Tamaño del nuevo cluster
│
├── 6. Dendrograma
│   ├── Ramas
│   ├── Altura de fusión
│   ├── Fusiones bajas
│   ├── Fusiones altas
│   └── Corte del árbol
│
├── 7. Evaluación e interpretación
│   ├── Cantidad de clusters
│   ├── Silhouette score
│   ├── Subgrupos
│   ├── Outliers
│   └── Lectura contextual
│
└── 8. Comparación con K-Means
    ├── Centroides vs fusiones
    ├── K fijo vs corte posterior
    ├── Plano de clusters vs dendrograma
    └── Escalabilidad e interpretación
```

---

## Guía rápida de lectura

### Para comenzar desde cero

Usar primero:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Clase%20te%C3%B3rica%20visual-1f4e79?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Clase%20te%C3%B3rica%20visual.html)

Este recurso permite presentar la intuición general del algoritmo y preparar la lectura de la simulación.

---

### Para explicar el algoritmo paso a paso

Usar después:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Simulaci%C3%B3n%20interactiva-7c3aed?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico%20Interactivo%20fusiones%2C%20linkage%20y%20dendrograma.html)

La explicación puede seguir este flujo:

```text
Cada punto es un cluster
        ↓
Calcular distancias
        ↓
Elegir la fusión más conveniente
        ↓
Registrar la fusión en la matriz linkage
        ↓
Construir el dendrograma
        ↓
Cortar el árbol
        ↓
Obtener clusters finales
```

---

### Para repasar y evaluar

Usar luego:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Cuestionario-f59e0b?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Cuestionario.html)

Este recurso permite comprobar si el estudiante puede explicar el tema con claridad.

---

### Para consolidar vocabulario

Usar después:

[![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Glosario-15803d?style=for-the-badge\&logo=html5\&logoColor=white)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Clustering%20Jer%C3%A1rquico_Glosario.html)

El glosario debe utilizarse después de la simulación, porque en ese momento los conceptos ya tienen una imagen mental asociada.

---

### Para practicar con Python

Usar como cierre práctico:

[![Abrir Colab](https://img.shields.io/badge/Abrir-Google%20Colab-f9ab00?style=for-the-badge\&logo=googlecolab\&logoColor=white)](https://colab.research.google.com/drive/1CiEih8HEVCWCQHWoBQnRGfosDcfiINFi?usp=sharing)

---

## Desarrollo conceptual del tema

### Qué es clustering jerárquico

El clustering jerárquico es una técnica de **aprendizaje no supervisado** que busca agrupar observaciones similares construyendo una estructura en forma de árbol.

En la versión aglomerativa, el algoritmo comienza con cada observación como un cluster individual y luego va fusionando los grupos más parecidos hasta formar una jerarquía completa.

---

### Por qué se llama jerárquico

Se llama jerárquico porque permite ver distintos niveles de agrupamiento.

```text
Nivel bajo  → muchos grupos pequeños
Nivel medio → grupos principales
Nivel alto  → pocos grupos grandes
```

El dendrograma permite observar esos niveles y decidir cuál es el nivel más útil para el análisis.

---

### Qué es una fusión

Una fusión es el momento en que el algoritmo une dos elementos.

```text
punto + punto
punto + cluster
cluster + cluster
```

Cada fusión crea un nuevo cluster y reduce en uno la cantidad total de clusters.

---

### Qué es la matriz linkage

La matriz linkage es la tabla que guarda la historia completa de las fusiones.

Cada fila tiene esta estructura:

```text
[cluster_1, cluster_2, distancia_de_fusión, cantidad_de_observaciones]
```

Ejemplo:

```text
[107, 114, 0.00228, 2]
```

Lectura:

```text
La observación 107 se fusionó con la observación 114
a una distancia de 0.00228
y formaron un nuevo cluster con 2 observaciones.
```

---

### Qué es un dendrograma

El dendrograma es el gráfico que representa visualmente la matriz linkage.

```text
Fusión baja  → grupos muy parecidos
Fusión alta  → grupos más diferentes
```

El dendrograma permite observar qué observaciones se unen primero, qué subgrupos aparecen y qué grandes ramas se mantienen separadas hasta el final.

---

### Cómo se corta el dendrograma

Cortar el dendrograma significa trazar una línea horizontal para obtener clusters finales.

```text
Corte bajo  → muchos clusters pequeños
Corte medio → clusters principales
Corte alto  → pocos clusters grandes
```

Una estrategia habitual es cortar antes de las fusiones muy altas, porque esas fusiones suelen indicar que el algoritmo está uniendo grupos bastante diferentes.

---

### Métodos de linkage

| Método           | Qué mide                                                     | Efecto típico                    |
| :--------------- | :----------------------------------------------------------- | :------------------------------- |
| Single linkage   | La menor distancia entre puntos de ambos clusters            | Puede formar cadenas             |
| Complete linkage | La mayor distancia entre puntos de ambos clusters            | Tiende a formar grupos compactos |
| Average linkage  | El promedio de las distancias entre puntos de ambos clusters | Busca un equilibrio              |
| Ward             | La fusión que menos aumenta la dispersión interna            | Suele generar clusters compactos |

---

## Comparación entre K-Means y Clustering Jerárquico

| Aspecto              | K-Means                                     | Clustering Jerárquico                    |
| :------------------- | :------------------------------------------ | :--------------------------------------- |
| Idea central         | Agrupar alrededor de centroides             | Construir un árbol de fusiones           |
| Cantidad de clusters | Se define K antes de ejecutar               | Puede decidirse cortando el dendrograma  |
| Resultado visual     | Puntos y centroides                         | Dendrograma                              |
| Proceso              | Asignar puntos y recalcular centroides      | Fusionar puntos o clusters               |
| Interpretación       | Compactación alrededor de centros           | Historia de similitudes y subgrupos      |
| Escalabilidad        | Suele ser más eficiente en datasets grandes | Puede ser más costoso computacionalmente |

---

## Limitaciones del clustering jerárquico

El clustering jerárquico es muy útil, pero tiene limitaciones importantes.

Puede fallar o dar resultados poco interpretables cuando:

* hay muchos datos y el dendrograma se vuelve difícil de leer;
* existen outliers;
* las variables no están escaladas;
* se elige una distancia poco adecuada;
* se usa un método de linkage que no representa bien el problema;
* se interpreta el dendrograma de manera automática sin analizar el contexto.

---

## Uso sugerido para una clase

| Momento de la clase      | Recurso sugerido       | Actividad                                    |
| :----------------------- | :--------------------- | :------------------------------------------- |
| Inicio                   | Clase teórica visual   | Presentar la intuición general del algoritmo |
| Desarrollo visual        | Simulación interactiva | Mostrar fusiones, linkage y dendrograma      |
| Repaso                   | Cuestionario           | Trabajar preguntas desarrolladas             |
| Consolidación conceptual | Glosario               | Repasar términos técnicos                    |
| Práctica                 | Google Colab           | Ejecutar clustering jerárquico en Python     |

---

## Preguntas guía para trabajar en clase

1. ¿Qué significa que clustering jerárquico sea un método de aprendizaje no supervisado?
2. ¿Qué diferencia hay entre clustering y clasificación?
3. ¿Qué es una observación?
4. ¿Qué es un cluster?
5. ¿Qué papel cumple la distancia?
6. ¿Qué es una fusión?
7. ¿Por qué se necesitan `n - 1` fusiones?
8. ¿Qué es el linkage?
9. ¿Qué diferencia hay entre single, complete, average y Ward?
10. ¿Qué es la matriz linkage?
11. ¿Qué representa cada fila de la matriz linkage?
12. ¿Qué es un dendrograma?
13. ¿Qué significa una fusión baja?
14. ¿Qué significa una fusión alta?
15. ¿Cómo se decide dónde cortar el dendrograma?
16. ¿Por qué es importante estandarizar las variables?
17. ¿Qué efecto pueden tener los outliers?
18. ¿En qué se diferencia clustering jerárquico de K-Means?

---

## Relación entre los recursos

| Concepto                   | Recurso principal      | Recurso complementario |
| :------------------------- | :--------------------- | :--------------------- |
| Aprendizaje no supervisado | Clase teórica visual   | Glosario               |
| Distancia                  | Clase teórica visual   | Colab                  |
| Fusión                     | Simulación interactiva | Cuestionario           |
| Linkage                    | Simulación interactiva | Glosario               |
| Ward                       | Simulación interactiva | Colab                  |
| Matriz linkage             | Clase teórica visual   | Colab                  |
| Dendrograma                | Simulación interactiva | Colab                  |
| Corte del árbol            | Simulación interactiva | Cuestionario           |
| Limitaciones               | Cuestionario           | Glosario               |
| Implementación en Python   | Colab                  | Simulación interactiva |

---

## Guion breve para presentar el bloque

### Inicio

En este módulo vamos a estudiar **clustering jerárquico**, una técnica fundamental de aprendizaje no supervisado que permite descubrir grupos dentro de los datos sin partir de etiquetas previas.

La idea no es solamente memorizar los pasos del algoritmo, sino comprender su lógica: cómo se miden las distancias, cómo se eligen las fusiones, cómo se registra la matriz linkage y cómo se interpreta el dendrograma.

---

### Paso 1 · Clase teórica visual

Primero vamos a revisar el recurso **Clustering Jerárquico · Clase teórica visual**, porque antes de mirar el algoritmo en movimiento necesitamos comprender qué representa cada elemento: los puntos, las distancias, las fusiones, la matriz linkage, la altura de fusión y el corte del árbol.

---

### Paso 2 · Simulación interactiva

Luego vamos a trabajar con la **simulación interactiva de clustering jerárquico**, donde podremos observar el proceso paso a paso.

La simulación permite ver cómo cada punto empieza como un cluster individual, cómo se realizan fusiones sucesivas, cómo se construye la matriz linkage y cómo aparece el dendrograma.

---

### Paso 3 · Cuestionario

Después de la simulación vamos a utilizar el **cuestionario** para repasar los conceptos centrales.

El objetivo es que cada estudiante pueda explicar con sus propias palabras qué está haciendo el algoritmo y cómo se interpreta el resultado.

---

### Paso 4 · Glosario

Luego vamos a utilizar el **glosario** para ordenar el vocabulario técnico del tema.

El glosario ayuda a convertir la intuición visual en lenguaje preciso.

---

### Paso 5 · Google Colab

Como cierre práctico, se puede abrir el notebook de **Google Colab** para conectar la explicación visual con código Python.

---

## Síntesis final

El clustering jerárquico es una herramienta fundamental para introducir el aprendizaje no supervisado porque permite ver de manera clara cómo un algoritmo puede encontrar estructura en los datos sin necesidad de etiquetas previas.

Su valor pedagógico está en que combina:

* intuición geométrica;
* cálculo de distancias;
* construcción progresiva de grupos;
* matriz linkage;
* dendrograma;
* decisión de corte;
* análisis crítico de limitaciones;
* implementación práctica en Python.

  ## 🎯 Objetivo general del bloque

Este conjunto de recursos tiene como objetivo comprender la **regresión lineal** como uno de los modelos fundamentales del aprendizaje automático supervisado y, al mismo tiempo, utilizarla como base conceptual para introducir la estructura de una **neurona artificial**.

El bloque parte de la idea de que un modelo lineal aprende una relación entre variables de entrada y una salida numérica mediante una combinación de pesos, sesgo y predicción. A partir de esa intuición inicial, se avanza hacia el entrenamiento del modelo, el ajuste de parámetros, el cálculo del error, la función de pérdida, el descenso por gradiente, la validación y la conexión conceptual con una neurona artificial.

La finalidad es que el estudiante pueda comprender que la regresión lineal no es solamente una técnica estadística clásica, sino también una puerta de entrada para entender cómo aprenden modelos más complejos. En particular, permite visualizar con claridad los conceptos de entrada, peso, sesgo, predicción, error, pérdida y actualización iterativa de parámetros, que luego reaparecen en redes neuronales artificiales.

---

## 🧭 Secuencia didáctica sugerida

```text
1. Índice general del paquete
        ↓
2. Introducción a regresión lineal
        ↓
3. Teoría y simulación de regresión lineal
        ↓
4. Regresión lineal como base de la neurona artificial
        ↓
5. Glosario completo de regresión lineal
        ↓
6. Cuestionario interactivo de integración
```

---

## 📚 Recursos interactivos

<table>
  <thead>
    <tr>
      <th align="center">Orden</th>
      <th align="left">Recurso</th>
      <th align="left">Propósito didáctico</th>
      <th align="center">Abrir HTML</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>0</strong></td>
      <td><strong>Índice general del paquete</strong></td>
      <td>Presentar la estructura completa del bloque, ordenar los recursos y facilitar el acceso a cada HTML desde un punto central de navegación.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_indice.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-%C3%8Dndice%20general-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir índice general">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>1</strong></td>
      <td><strong>Introducción a regresión lineal</strong></td>
      <td>Introducir el modelo lineal básico, su ecuación principal, la relación entre variables, la idea de predicción y la interpretación inicial de pendiente e intercepto.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/regresion_lineal.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Regresi%C3%B3n%20lineal-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regresión lineal">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>2</strong></td>
      <td><strong>Regresión lineal: teoría y simulación</strong></td>
      <td>Comprender cómo un modelo lineal aprende una recta, cómo se ajustan la pendiente y el intercepto, cómo se calcula el error y por qué se separan datos de entrenamiento y validación.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_teoria_simulacion.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Teor%C3%ADa%20y%20simulaci%C3%B3n-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir teoría y simulación">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>3</strong></td>
      <td><strong>Regresión lineal y neurona artificial</strong></td>
      <td>Mostrar la conexión entre regresión lineal y neurona artificial mediante entradas, pesos, sesgo, combinación lineal, predicción, error, función de pérdida y activación.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_neurona_artificial_interactiva.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Neurona%20artificial-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regresión lineal y neurona artificial">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>4</strong></td>
      <td><strong>Glosario completo de regresión lineal</strong></td>
      <td>Reunir y desarrollar los conceptos centrales del bloque, incluyendo modelo lineal, pesos, sesgo, predicción, error, MSE, R², entrenamiento, validación, generalización y métricas.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_glosario.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Glosario%20completo-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir glosario completo">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>5</strong></td>
      <td><strong>Cuestionario interactivo</strong></td>
      <td>Integrar los contenidos mediante preguntas desarrolladas sobre regresión lineal, pesos, sesgo, función de pérdida, descenso por gradiente, neurona artificial y redes neuronales.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_Cuestionario_regresion_neurona_interactivo.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Cuestionario%20interactivo-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir cuestionario interactivo">
        </a>
      </td>
    </tr>
  </tbody>
</table>

---

## 🔗 Acceso directo a los recursos

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_indice.html">
    <img src="https://img.shields.io/badge/0.%20Abrir%20HTML-%C3%8Dndice%20general-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir índice general">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/regresion_lineal.html">
    <img src="https://img.shields.io/badge/1.%20Abrir%20HTML-Regresi%C3%B3n%20lineal-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regresión lineal">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_teoria_simulacion.html">
    <img src="https://img.shields.io/badge/2.%20Abrir%20HTML-Teor%C3%ADa%20y%20simulaci%C3%B3n-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir teoría y simulación">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_neurona_artificial_interactiva.html">
    <img src="https://img.shields.io/badge/3.%20Abrir%20HTML-Regresi%C3%B3n%20y%20neurona%20artificial-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regresión lineal y neurona artificial">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_glosario.html">
    <img src="https://img.shields.io/badge/4.%20Abrir%20HTML-Glosario%20completo-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir glosario completo">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_Cuestionario_regresion_neurona_interactivo.html">
    <img src="https://img.shields.io/badge/5.%20Abrir%20HTML-Cuestionario%20interactivo-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir cuestionario interactivo">
  </a>
</p>

---

## 🧩 Resumen didáctico de cada recurso

### 0. Índice general del paquete

El índice funciona como la **puerta de entrada al bloque completo**. Permite ordenar los materiales, acceder rápidamente a cada HTML y presentar una secuencia clara para el estudio de la regresión lineal y su conexión con la neurona artificial.

Su utilidad principal es transformar varios archivos separados en una experiencia de aprendizaje organizada. Desde este recurso, el estudiante puede iniciar el recorrido, acceder a las simulaciones, consultar el glosario y cerrar con el cuestionario interactivo.

**Idea clave:** el índice convierte el paquete en un recorrido didáctico navegable.

---

### 1. Introducción a regresión lineal

Este recurso introduce la regresión lineal como modelo supervisado orientado a predecir una variable numérica a partir de una o más variables de entrada.

La idea central es comprender que el modelo intenta representar una relación entre variables mediante una función lineal. En el caso más simple, esa función se expresa como una recta:

```text
ŷ = wx + b
```

Donde:

- `x` representa la entrada;
- `w` representa el peso o pendiente;
- `b` representa el sesgo o intercepto;
- `ŷ` representa la predicción del modelo.

Este recurso permite trabajar la intuición inicial del modelo, la interpretación de sus parámetros y la diferencia entre valor observado y valor predicho.

**Idea clave:** la regresión lineal aprende una relación aproximada entre datos de entrada y una salida numérica.

---

### 2. Regresión lineal: teoría y simulación

Este recurso profundiza en el proceso de aprendizaje de un modelo lineal. Permite visualizar cómo se ajustan los parámetros del modelo, cómo cambia la recta de predicción y cómo se reduce el error durante el entrenamiento.

También introduce una distinción fundamental para Machine Learning: la separación entre datos de entrenamiento y datos de validación. Esta diferencia permite comprender que un modelo no solo debe ajustarse a los datos conocidos, sino también funcionar razonablemente bien sobre datos nuevos.

Permite trabajar:

- pendiente;
- intercepto;
- predicción;
- error;
- función de pérdida;
- MSE;
- entrenamiento;
- validación;
- epochs;
- descenso por gradiente;
- ajuste iterativo de parámetros.

**Idea clave:** entrenar un modelo lineal significa ajustar sus parámetros para reducir el error de predicción.

---

### 3. Regresión lineal y neurona artificial

Este recurso muestra que la estructura matemática de la regresión lineal permite comprender la base de una neurona artificial.

Una neurona artificial recibe entradas, multiplica cada entrada por un peso, suma esos productos, incorpora un sesgo y genera una salida. Esta estructura coincide con la combinación lineal que aparece en la regresión:

```text
z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b
```

La diferencia central es que, en una neurona artificial, luego puede aplicarse una función de activación:

```text
a = f(z)
```

Esto permite pasar de un modelo puramente lineal a modelos capaces de representar relaciones no lineales cuando se combinan muchas neuronas y capas.

Permite trabajar:

- entradas;
- pesos;
- sesgo;
- producto ponderado;
- combinación lineal;
- predicción;
- activación;
- error;
- función de pérdida;
- aprendizaje;
- conexión entre regresión lineal y redes neuronales.

**Idea clave:** la regresión lineal permite entender la operación matemática básica de una neurona artificial.

---

### 4. Glosario completo de regresión lineal

El glosario funciona como recurso de consulta y consolidación conceptual. Reúne los términos centrales del bloque y los desarrolla de manera explicativa para que el estudiante pueda repasar antes, durante o después de la clase.

Incluye conceptos fundamentales del modelo lineal, del entrenamiento, de la evaluación y de la interpretación de resultados.

Permite trabajar:

- regresión lineal;
- variable independiente;
- variable dependiente;
- peso;
- sesgo;
- pendiente;
- intercepto;
- predicción;
- residuo;
- error;
- MSE;
- MAE;
- RMSE;
- R²;
- entrenamiento;
- validación;
- sobreajuste;
- subajuste;
- generalización.

**Idea clave:** el glosario permite transformar conceptos técnicos en una guía de estudio clara, ordenada y consultable.

---

### 5. Cuestionario interactivo

El cuestionario interactivo funciona como cierre del bloque. Permite repasar los conceptos centrales mediante preguntas desarrolladas y orientadas a la comprensión, no solo a la memorización.

Su valor didáctico está en conectar regresión lineal, neurona artificial, pesos, sesgo, función de pérdida, descenso por gradiente y redes neuronales dentro de un mismo recorrido conceptual.

Permite trabajar:

- preguntas conceptuales;
- respuestas desarrolladas;
- interpretación de fórmulas;
- explicación del entrenamiento;
- relación entre regresión lineal y neurona artificial;
- función de pérdida;
- descenso por gradiente;
- activación;
- límites del modelo lineal;
- preparación para evaluación.

**Idea clave:** el cuestionario consolida el aprendizaje al exigir que el estudiante explique cómo se conectan los conceptos del bloque.

---

## 🗺️ Mapa conceptual del módulo

```text
Regresión lineal
│
├── 1. Modelo lineal
│   ├── Entrada x
│   ├── Peso w
│   ├── Sesgo b
│   ├── Predicción ŷ
│   └── Recta de ajuste
│
├── 2. Interpretación de parámetros
│   ├── Pendiente
│   ├── Intercepto
│   ├── Cambio esperado en la salida
│   └── Relación entre variables
│
├── 3. Error y pérdida
│   ├── Valor real y
│   ├── Valor predicho ŷ
│   ├── Residuo
│   ├── Error cuadrático
│   ├── MSE
│   ├── MAE
│   └── RMSE
│
├── 4. Entrenamiento
│   ├── Ajuste de parámetros
│   ├── Descenso por gradiente
│   ├── Learning rate
│   ├── Epochs
│   └── Reducción de la pérdida
│
├── 5. Evaluación
│   ├── Datos de entrenamiento
│   ├── Datos de validación
│   ├── Generalización
│   ├── Overfitting
│   ├── Underfitting
│   └── R²
│
├── 6. Conexión con neurona artificial
│   ├── Entradas
│   ├── Pesos
│   ├── Sesgo
│   ├── Combinación lineal
│   ├── Activación
│   └── Salida
│
└── 7. Integración
    ├── Simulación
    ├── Glosario
    ├── Preguntas desarrolladas
    ├── Interpretación conceptual
    └── Aplicación en clase
```

---

## 📖 Guía rápida de uso

### Para comenzar el recorrido

Usar primero el índice general del paquete.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_indice.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-%C3%8Dndice%20general-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir índice general">
</a>

Este recurso permite presentar la estructura del bloque y orientar al estudiante en el recorrido completo.

---

### Para introducir la regresión lineal

Usar el recurso introductorio de regresión lineal.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/regresion_lineal.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Regresi%C3%B3n%20lineal-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regresión lineal">
</a>

Flujo sugerido:

```text
Variable de entrada
        ↓
Peso
        ↓
Sesgo
        ↓
Predicción
        ↓
Comparación con el valor real
```

---

### Para explicar entrenamiento y validación

Usar el recurso de teoría y simulación.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_teoria_simulacion.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Teor%C3%ADa%20y%20simulaci%C3%B3n-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir teoría y simulación">
</a>

Este recurso permite mostrar cómo un modelo aprende de forma iterativa ajustando sus parámetros para reducir el error.

---

### Para conectar regresión lineal con neurona artificial

Usar el recurso de regresión lineal y neurona artificial.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_neurona_artificial_interactiva.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Regresi%C3%B3n%20y%20neurona%20artificial-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regresión lineal y neurona artificial">
</a>

Flujo sugerido:

```text
Regresión lineal
        ↓
Combinación lineal
        ↓
Entradas, pesos y sesgo
        ↓
Neurona artificial
        ↓
Función de activación
```

---

### Para repasar conceptos clave

Usar el glosario completo.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_glosario.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Glosario%20completo-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir glosario completo">
</a>

Este recurso permite consolidar el vocabulario técnico y funciona como guía de estudio.

---

### Para evaluar e integrar

Usar el cuestionario interactivo.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/Regresion_lineal_Cuestionario_regresion_neurona_interactivo.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Cuestionario%20interactivo-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir cuestionario interactivo">
</a>

Este recurso permite verificar comprensión conceptual y preparar al estudiante para explicar el tema con sus propias palabras.

---

## 🧠 Desarrollo conceptual del tema

### Qué es la regresión lineal

La regresión lineal es un modelo de aprendizaje supervisado utilizado para predecir una variable numérica a partir de una o más variables de entrada.

En su forma más simple, el modelo busca ajustar una recta que represente la relación entre una entrada y una salida.

```text
ŷ = wx + b
```

Donde:

- `x` es la variable de entrada;
- `w` es el peso o coeficiente;
- `b` es el sesgo o intercepto;
- `ŷ` es la predicción del modelo.

---

### Qué representa el peso

El peso indica cuánto cambia la predicción cuando cambia la variable de entrada. En una regresión lineal simple, el peso coincide con la pendiente de la recta.

Si el peso es positivo, la predicción tiende a aumentar cuando aumenta la entrada. Si el peso es negativo, la predicción tiende a disminuir cuando aumenta la entrada.

```text
ŷ = wx + b
```

En esta expresión, `w` controla la inclinación de la recta.

---

### Qué representa el sesgo

El sesgo o intercepto indica el valor de la predicción cuando la entrada vale cero.

También permite desplazar la recta hacia arriba o hacia abajo sin cambiar su inclinación.

```text
ŷ = wx + b
```

En esta expresión, `b` controla el desplazamiento vertical del modelo.

---

### Qué es una predicción

Una predicción es el valor que genera el modelo a partir de una entrada.

El modelo recibe `x`, aplica la ecuación aprendida y produce `ŷ`.

```text
Entrada x
        ↓
Modelo lineal
        ↓
Predicción ŷ
```

La predicción luego se compara con el valor real `y` para calcular el error.

---

### Qué es el error

El error mide la diferencia entre el valor real y el valor predicho.

```text
error = y - ŷ
```

Si el error es grande, el modelo está prediciendo mal. Si el error es pequeño, el modelo está más cerca del valor real.

---

### Qué es una función de pérdida

Una función de pérdida resume qué tan mal está prediciendo el modelo. En regresión lineal, una de las funciones más utilizadas es el error cuadrático medio.

```text
MSE = promedio de (y - ŷ)²
```

El objetivo del entrenamiento es reducir esta pérdida.

---

### Qué es el descenso por gradiente

El descenso por gradiente es un método de optimización que permite ajustar los parámetros del modelo para reducir la función de pérdida.

La idea es modificar los pesos y el sesgo en la dirección que disminuye el error.

```text
w ← w - η · ∂L/∂w
b ← b - η · ∂L/∂b
```

Donde:

- `η` es el learning rate;
- `L` es la función de pérdida;
- `∂L/∂w` indica cómo cambia la pérdida respecto del peso;
- `∂L/∂b` indica cómo cambia la pérdida respecto del sesgo.

---

### Qué es entrenamiento

Entrenar un modelo significa ajustar sus parámetros usando datos conocidos.

En regresión lineal, el entrenamiento consiste en encontrar valores adecuados para `w` y `b` de modo que las predicciones se acerquen lo más posible a los valores reales.

```text
Datos
        ↓
Predicción
        ↓
Error
        ↓
Pérdida
        ↓
Actualización de parámetros
        ↓
Nueva predicción
```

---

### Qué es validación

La validación consiste en evaluar el modelo con datos que no fueron usados directamente para entrenarlo.

Esto permite analizar si el modelo aprendió una relación general o si simplemente se ajustó demasiado a los datos de entrenamiento.

```text
Datos de entrenamiento → ajustar el modelo
Datos de validación    → evaluar generalización
```

---

### Qué es overfitting

El overfitting o sobreajuste ocurre cuando un modelo aprende demasiado bien los datos de entrenamiento, incluyendo ruido o particularidades que no se repiten en nuevos datos.

Un modelo sobreajustado puede tener bajo error de entrenamiento, pero alto error de validación.

```text
Buen desempeño en entrenamiento
        ↓
Mal desempeño en datos nuevos
        ↓
Sobreajuste
```

---

### Qué es underfitting

El underfitting o subajuste ocurre cuando el modelo es demasiado simple o no logra capturar la relación presente en los datos.

En ese caso, el error suele ser alto tanto en entrenamiento como en validación.

```text
Mal desempeño en entrenamiento
        ↓
Mal desempeño en validación
        ↓
Subajuste
```

---

### Qué es R²

El coeficiente de determinación `R²` mide qué proporción de la variabilidad de la variable objetivo puede ser explicada por el modelo.

Un valor de `R²` más alto indica que el modelo explica mejor la variabilidad de los datos, aunque siempre debe interpretarse junto con otras métricas y con el contexto del problema.

---

### Cómo se conecta la regresión lineal con una neurona artificial

La regresión lineal y una neurona artificial comparten una estructura matemática básica: ambas combinan entradas con pesos y agregan un sesgo.

En una regresión lineal múltiple:

```text
ŷ = w₁x₁ + w₂x₂ + ... + wₙxₙ + b
```

En una neurona artificial:

```text
z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b
a = f(z)
```

La diferencia es que la neurona puede aplicar una función de activación `f`, lo que permite introducir no linealidad y construir modelos más complejos cuando se combinan muchas neuronas.

---

## ✅ Preguntas orientadoras para estudiantes

1. ¿Qué problema busca resolver la regresión lineal?
2. ¿Qué representa la variable de entrada en un modelo lineal?
3. ¿Qué representa la variable objetivo?
4. ¿Qué significa la predicción `ŷ`?
5. ¿Qué representa el peso `w`?
6. ¿Qué representa el sesgo `b`?
7. ¿Qué diferencia hay entre valor real y valor predicho?
8. ¿Qué mide el error?
9. ¿Por qué se utiliza una función de pérdida?
10. ¿Qué significa minimizar el MSE?
11. ¿Qué es el descenso por gradiente?
12. ¿Qué función cumple el learning rate?
13. ¿Qué es una epoch?
14. ¿Por qué se separan datos de entrenamiento y validación?
15. ¿Qué diferencia hay entre overfitting y underfitting?
16. ¿Qué mide el coeficiente R²?
17. ¿Por qué la regresión lineal es interpretable?
18. ¿Qué relación existe entre regresión lineal y una neurona artificial?
19. ¿Qué agrega una función de activación a una neurona?
20. ¿Por qué este tema sirve como base para estudiar redes neuronales?

---

## 🧾 Síntesis final

La regresión lineal es uno de los modelos más importantes para iniciar el estudio del aprendizaje automático porque permite comprender, de manera clara e interpretable, cómo un modelo transforma datos de entrada en predicciones.

Su estructura se basa en pesos, sesgo, predicción, error y ajuste de parámetros. Estos mismos elementos aparecen luego en modelos más complejos, como las neuronas artificiales y las redes neuronales.

Por eso, estudiar regresión lineal no solo permite aprender una técnica útil para problemas de predicción numérica, sino también construir una base conceptual sólida para comprender cómo aprenden los modelos de Machine Learning.

El recorrido propuesto integra teoría, simulación, conexión con neuronas artificiales, glosario y cuestionario. De esta manera, el estudiante puede avanzar desde la intuición básica hasta una comprensión más profunda del entrenamiento y la evaluación de modelos.

---

# 🧠 Redes Neuronales · Recursos interactivos de estudio

> Material organizado para estudiar **redes neuronales artificiales**, **perceptrón**, **funciones de activación**, **descenso por gradiente**, **forward propagation**, **backpropagation**, **regularización** y **actividad integradora** mediante teoría visual, simulaciones interactivas y recursos didácticos para clase.

---

## 🎯 Objetivo general del bloque

Este conjunto de recursos tiene como objetivo comprender las **redes neuronales artificiales** desde una perspectiva conceptual, visual y práctica.

El bloque parte de la idea de una neurona artificial como una unidad que recibe entradas, calcula una combinación ponderada, aplica una función de activación y produce una salida. A partir de esa intuición inicial, se avanza hacia el perceptrón, las fronteras de decisión, las funciones de activación, el proceso de entrenamiento, el descenso por gradiente, la propagación hacia adelante, la retropropagación del error y las técnicas de regularización.

La finalidad es que el estudiante pueda comprender que una red neuronal no es una “caja mágica”, sino un sistema matemático entrenable que transforma datos mediante pesos, sesgos, activaciones y actualizaciones iterativas.

---

## 🧭 Secuencia didáctica sugerida

```text
1. Teoría completa de redes neuronales
        ↓
2. Perceptrón y fronteras de decisión
        ↓
3. Funciones de activación
        ↓
4. Descenso por gradiente
        ↓
5. Forward propagation y backpropagation paso a paso
        ↓
6. Forward propagation y backpropagation con teoría dinámica
        ↓
7. Regularización y generalización
        ↓
8. Actividad integrada
```

---

## 📚 Recursos interactivos

<table>
  <thead>
    <tr>
      <th align="center">Orden</th>
      <th align="left">Recurso</th>
      <th align="left">Propósito didáctico</th>
      <th align="center">Abrir HTML</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>0</strong></td>
      <td><strong>Índice de la clase</strong></td>
      <td>Presentar la estructura general del bloque, ordenar los recursos y facilitar el acceso a cada HTML desde un punto central.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/00_indice_clase_redes_neuronales.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-%C3%8Dndice-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir índice">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>1</strong></td>
      <td><strong>Teoría completa de redes neuronales</strong></td>
      <td>Introducir el marco conceptual del tema: neurona artificial, pesos, sesgo, activaciones, capas, entrenamiento, error y aprendizaje.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_teoria_completa_redes_neuronales.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Teor%C3%ADa%20completa-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir teoría completa">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>2</strong></td>
      <td><strong>Perceptrón y fronteras de decisión</strong></td>
      <td>Visualizar cómo un perceptrón construye fronteras lineales para resolver problemas lógicos como AND, OR, NAND y NOR, y por qué XOR requiere mayor complejidad.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/02_simulacion_perceptron_fronteras.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Perceptr%C3%B3n-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir perceptrón">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>3</strong></td>
      <td><strong>Funciones de activación</strong></td>
      <td>Comparar identidad, escalón, sigmoide, tangente hiperbólica, ReLU y variantes, observando forma, derivada, saturación y uso práctico.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/03_simulacion_activaciones.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Activaciones-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir activaciones">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>4</strong></td>
      <td><strong>Descenso por gradiente</strong></td>
      <td>Mostrar cómo un modelo reduce el error moviéndose en la dirección opuesta al gradiente, y cómo el learning rate afecta la convergencia.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/04_simulacion_descenso_gradiente.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Gradiente-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir descenso por gradiente">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>5</strong></td>
      <td><strong>Forward y backpropagation paso a paso</strong></td>
      <td>Explicar el flujo de cálculo de una red pequeña: entradas, pesos, activaciones, predicción, error, gradientes y actualización de parámetros.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_forward_backprop_paso_a_paso.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Backprop%20paso%20a%20paso-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir backprop paso a paso">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>6</strong></td>
      <td><strong>Forward y backpropagation con teoría dinámica</strong></td>
      <td>Reforzar la comprensión conceptual del aprendizaje de una red neuronal mediante explicaciones dinámicas, métricas y visualización del proceso de ajuste.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_forward_backprop_teoria_dinamica.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Backprop%20din%C3%A1mico-9333ea?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir backprop dinámico">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>7</strong></td>
      <td><strong>Regularización en redes neuronales</strong></td>
      <td>Comprender el sobreajuste y estudiar técnicas para mejorar la generalización, como penalización L2, dropout, early stopping y control de complejidad.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/06_regularizacion_teoria_practica_interactiva.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Regularizaci%C3%B3n-0891b2?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regularización">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>8</strong></td>
      <td><strong>Actividad integrada</strong></td>
      <td>Integrar los conceptos del bloque mediante preguntas, ejercicios guiados, interpretación de resultados y consignas para discusión en clase.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/07_actividad_integrada_redes_neuronales.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Actividad%20integrada-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir actividad integrada">
        </a>
      </td>
    </tr>
  </tbody>
</table>

---

## 🔗 Acceso directo a los recursos

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/00_indice_clase_redes_neuronales.html">
    <img src="https://img.shields.io/badge/0.%20Abrir%20HTML-%C3%8Dndice-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir índice">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_teoria_completa_redes_neuronales.html">
    <img src="https://img.shields.io/badge/1.%20Abrir%20HTML-Teor%C3%ADa%20completa-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir teoría completa">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/02_simulacion_perceptron_fronteras.html">
    <img src="https://img.shields.io/badge/2.%20Abrir%20HTML-Perceptr%C3%B3n%20y%20fronteras-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir perceptrón y fronteras">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/03_simulacion_activaciones.html">
    <img src="https://img.shields.io/badge/3.%20Abrir%20HTML-Funciones%20de%20activaci%C3%B3n-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir funciones de activación">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/04_simulacion_descenso_gradiente.html">
    <img src="https://img.shields.io/badge/4.%20Abrir%20HTML-Descenso%20por%20gradiente-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir descenso por gradiente">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_forward_backprop_paso_a_paso.html">
    <img src="https://img.shields.io/badge/5.%20Abrir%20HTML-Forward%20y%20Backprop%20paso%20a%20paso-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir forward y backprop paso a paso">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_forward_backprop_teoria_dinamica.html">
    <img src="https://img.shields.io/badge/6.%20Abrir%20HTML-Backprop%20teor%C3%ADa%20din%C3%A1mica-9333ea?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir backprop teoría dinámica">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/06_regularizacion_teoria_practica_interactiva.html">
    <img src="https://img.shields.io/badge/7.%20Abrir%20HTML-Regularizaci%C3%B3n-0891b2?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regularización">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/07_actividad_integrada_redes_neuronales.html">
    <img src="https://img.shields.io/badge/8.%20Abrir%20HTML-Actividad%20integrada-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir actividad integrada">
  </a>
</p>

---

## 🧩 Resumen didáctico de cada recurso

### 0. Índice de la clase

El índice funciona como la **puerta de entrada al bloque completo**. Permite ordenar los materiales, acceder rápidamente a cada HTML y presentar una secuencia clara para el estudio de redes neuronales.

Su utilidad principal es transformar varios archivos separados en una experiencia de aprendizaje organizada. Desde este recurso, el estudiante puede iniciar la clase, recorrer las simulaciones y volver al punto central cuando lo necesite.

**Idea clave:** el índice convierte el paquete en un recorrido didáctico navegable.

---

### 1. Teoría completa de redes neuronales

Este recurso introduce el marco conceptual del tema. Presenta la neurona artificial como una unidad matemática que recibe entradas, las combina con pesos, incorpora un sesgo, aplica una función de activación y produce una salida.

También permite comprender que una red neuronal aprende ajustando parámetros. Es decir, no memoriza reglas escritas manualmente, sino que modifica pesos y sesgos a partir del error observado durante el entrenamiento.

Permite trabajar:

- neurona artificial;
- entradas;
- pesos;
- sesgo;
- combinación lineal;
- función de activación;
- capas;
- predicción;
- error;
- entrenamiento;
- aprendizaje supervisado.

**Idea clave:** una red neuronal aprende ajustando pesos y sesgos para transformar entradas en salidas cada vez más cercanas al objetivo.

---

### 2. Perceptrón y fronteras de decisión

Este recurso funciona como el primer laboratorio visual del bloque. Permite observar cómo una neurona simple puede resolver problemas de clasificación binaria cuando las clases son linealmente separables.

A través de ejemplos como AND, OR, NAND y NOR, el estudiante puede ver cómo una frontera de decisión separa regiones del espacio. El caso XOR permite mostrar el límite del perceptrón simple y justificar la necesidad de redes con capas ocultas.

Permite trabajar:

- perceptrón;
- clasificación binaria;
- tabla de verdad;
- funciones lógicas;
- AND;
- OR;
- NAND;
- NOR;
- XOR;
- pesos y sesgo;
- frontera de decisión;
- separación lineal.

**Idea clave:** el perceptrón puede resolver problemas linealmente separables, pero necesita mayor arquitectura para representar patrones no lineales como XOR.

---

### 3. Funciones de activación

Este recurso permite comprender por qué las redes neuronales necesitan funciones de activación. Sin activaciones no lineales, una red profunda equivaldría a una transformación lineal más grande, pero no ganaría verdadera capacidad de representación.

La comparación entre identidad, escalón, sigmoide, tangente hiperbólica, ReLU y Leaky ReLU ayuda a visualizar forma, rango, derivada, saturación y utilidad práctica de cada función.

Permite trabajar:

- función identidad;
- función escalón;
- sigmoide;
- tangente hiperbólica;
- ReLU;
- Leaky ReLU;
- derivadas;
- saturación;
- gradientes;
- no linealidad.

**Idea clave:** las funciones de activación permiten que la red modele relaciones no lineales.

---

### 4. Descenso por gradiente

Este recurso muestra el motor del aprendizaje en redes neuronales. Permite visualizar cómo un modelo reduce su error moviéndose en la dirección opuesta al gradiente de la función de pérdida.

El estudiante puede analizar qué ocurre cuando el learning rate es muy pequeño, adecuado o demasiado grande. Esto permite comprender por qué el entrenamiento puede ser lento, estable, oscilante o incluso divergente.

Permite trabajar:

- función de pérdida;
- costo;
- gradiente;
- pendiente;
- mínimo;
- learning rate;
- trayectoria de optimización;
- convergencia;
- oscilación;
- divergencia.

**Idea clave:** entrenar una red significa ajustar parámetros en la dirección que reduce la pérdida.

---

### 5. Forward y backpropagation paso a paso

Este recurso permite observar el ciclo completo de aprendizaje en una red pequeña. Primero se calcula una predicción hacia adelante y luego se calcula cómo debe ajustarse cada peso para reducir el error.

Es especialmente útil para mostrar que el entrenamiento no ocurre de manera intuitiva o arbitraria, sino mediante una cadena de cálculos ordenados.

Permite trabajar:

- entrada de datos;
- cálculo de activaciones;
- propagación hacia adelante;
- predicción;
- cálculo del error;
- pérdida;
- gradientes;
- retropropagación;
- actualización de pesos.

**Idea clave:** forward propagation calcula la predicción, mientras que backpropagation calcula cómo debe modificarse cada peso.

---

### 6. Forward y backpropagation con teoría dinámica

Este recurso complementa el anterior con una explicación más conceptual del proceso de aprendizaje. Su valor didáctico está en conectar el flujo visual de la red con la interpretación del error y la responsabilidad de cada parámetro.

Permite reforzar que backpropagation no distribuye el error de forma uniforme, sino de acuerdo con la contribución de cada peso dentro de la cadena de operaciones.

Permite trabajar:

- flujo de información;
- relación entre capas;
- interpretación del error;
- propagación del error hacia atrás;
- sensibilidad de los pesos;
- efecto de cada actualización;
- aprendizaje como proceso iterativo.

**Idea clave:** backpropagation distribuye responsabilidad sobre el error según la contribución de cada parámetro.

---

### 7. Regularización en redes neuronales

Este recurso introduce el problema del sobreajuste y la necesidad de construir modelos que generalicen. El objetivo no es solamente reducir el error de entrenamiento, sino lograr buen desempeño sobre datos nuevos.

La simulación permite distinguir entre memorizar ruido y aprender patrones relevantes. También permite estudiar técnicas como L1, L2, dropout, early stopping y control de complejidad.

Permite trabajar:

- overfitting;
- underfitting;
- generalización;
- complejidad del modelo;
- entrenamiento;
- validación;
- penalización L2;
- penalización L1;
- dropout;
- early stopping.

**Idea clave:** una red útil no debe memorizar los datos de entrenamiento, sino aprender patrones que funcionen sobre datos nuevos.

---

### 8. Actividad integrada

La actividad integrada funciona como cierre del bloque. Permite repasar, ordenar y aplicar los conceptos centrales mediante preguntas, consignas y ejercicios de interpretación.

Es útil para verificar si el estudiante puede explicar cómo se conectan neurona, activación, pérdida, gradiente, backpropagation y regularización en un mismo proceso de aprendizaje.

Permite trabajar:

- preguntas conceptuales;
- lectura de simulaciones;
- interpretación de resultados;
- comparación entre técnicas;
- errores frecuentes;
- explicación oral o escrita;
- preparación para evaluación.

**Idea clave:** el aprendizaje se consolida cuando el estudiante puede explicar el flujo completo de una red neuronal.

---

## 🗺️ Mapa conceptual del módulo

```text
Redes Neuronales
│
├── 1. Neurona artificial
│   ├── Entradas
│   ├── Pesos
│   ├── Sesgo
│   ├── Combinación lineal
│   └── Salida
│
├── 2. Funciones de activación
│   ├── Identidad
│   ├── Escalón
│   ├── Sigmoide
│   ├── Tanh
│   ├── ReLU
│   └── Leaky ReLU
│
├── 3. Perceptrón
│   ├── Clasificación binaria
│   ├── Tabla de verdad
│   ├── Frontera de decisión
│   ├── Separación lineal
│   └── Limitaciones con XOR
│
├── 4. Entrenamiento
│   ├── Predicción
│   ├── Error
│   ├── Función de pérdida
│   ├── Gradiente
│   └── Actualización de pesos
│
├── 5. Descenso por gradiente
│   ├── Learning rate
│   ├── Dirección de descenso
│   ├── Convergencia
│   ├── Oscilación
│   └── Divergencia
│
├── 6. Propagación
│   ├── Forward propagation
│   ├── Cálculo de activaciones
│   ├── Backpropagation
│   ├── Regla de la cadena
│   └── Gradientes por parámetro
│
├── 7. Regularización
│   ├── Overfitting
│   ├── Underfitting
│   ├── L1
│   ├── L2
│   ├── Dropout
│   ├── Early stopping
│   └── Generalización
│
└── 8. Integración
    ├── Interpretación
    ├── Diagnóstico de errores
    ├── Comparación de métodos
    ├── Explicación conceptual
    └── Aplicación en clase
```

---

## 📖 Guía rápida de uso

### Para comenzar desde cero

Usar primero la teoría completa.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_teoria_completa_redes_neuronales.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Teor%C3%ADa%20completa-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir teoría completa">
</a>

Este recurso permite presentar la intuición general: una red neuronal recibe datos, los transforma mediante pesos y activaciones, produce una predicción y aprende a partir del error.

---

### Para explicar la primera neurona clasificadora

Usar el recurso de perceptrón y fronteras de decisión.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/02_simulacion_perceptron_fronteras.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Perceptr%C3%B3n-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir perceptrón">
</a>

Flujo sugerido:

```text
Entradas
        ↓
Pesos y sesgo
        ↓
Combinación lineal
        ↓
Activación
        ↓
Clasificación
        ↓
Frontera de decisión
```

---

### Para explicar por qué una red necesita no linealidad

Usar el recurso de funciones de activación.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/03_simulacion_activaciones.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Activaciones-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir activaciones">
</a>

Este recurso permite mostrar que las funciones de activación no solo transforman valores, sino que permiten que la red modele relaciones no lineales.

---

### Para explicar cómo aprende el modelo

Usar el recurso de descenso por gradiente.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/04_simulacion_descenso_gradiente.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Gradiente-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir gradiente">
</a>

Flujo sugerido:

```text
Predicción
        ↓
Error
        ↓
Función de pérdida
        ↓
Gradiente
        ↓
Actualización
        ↓
Nueva predicción
```

---

### Para explicar el ciclo completo de entrenamiento

Usar primero forward y backpropagation paso a paso.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_forward_backprop_paso_a_paso.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Backprop%20paso%20a%20paso-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir backprop paso a paso">
</a>

Luego complementar con la explicación dinámica.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_forward_backprop_teoria_dinamica.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Backprop%20din%C3%A1mico-9333ea?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir backprop dinámico">
</a>

---

### Para cerrar con generalización

Usar el recurso de regularización.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/06_regularizacion_teoria_practica_interactiva.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Regularizaci%C3%B3n-0891b2?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir regularización">
</a>

Este recurso permite explicar que entrenar bien no significa solamente reducir el error de entrenamiento, sino lograr que el modelo funcione con datos nuevos.

---

### Para repasar y evaluar

Usar la actividad integrada.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/07_actividad_integrada_redes_neuronales.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Actividad%20integrada-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir actividad integrada">
</a>

---

## 🧠 Desarrollo conceptual del tema

### Qué es una red neuronal artificial

Una red neuronal artificial es un modelo computacional inspirado de manera abstracta en la idea de neuronas conectadas. No reproduce el cerebro humano de forma biológica, sino que utiliza unidades matemáticas que reciben entradas, las ponderan, aplican transformaciones y producen salidas.

En términos simples, una red neuronal aprende una función que relaciona datos de entrada con una salida esperada.

```text
Datos de entrada
        ↓
Transformaciones internas
        ↓
Predicción
        ↓
Comparación con el valor real
        ↓
Ajuste de parámetros
```

---

### Qué es una neurona artificial

Una neurona artificial recibe valores de entrada, multiplica cada uno por un peso, suma esos resultados, agrega un sesgo y aplica una función de activación.

```text
z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b
```

Donde:

- `x₁, x₂, ..., xₙ` son las entradas;
- `w₁, w₂, ..., wₙ` son los pesos;
- `b` es el sesgo;
- `z` es la combinación lineal previa a la activación.

Luego se aplica una función de activación:

```text
a = f(z)
```

Donde:

- `f` es la función de activación;
- `a` es la salida de la neurona.

---

### Qué es una función de activación

Una función de activación transforma el valor `z` calculado por la neurona.

Su función principal es introducir no linealidad. Esto permite que una red neuronal pueda aprender patrones complejos que no pueden representarse con una simple recta o plano.

| Función | Uso habitual | Idea principal |
| :------ | :----------- | :------------- |
| Identidad | Regresión lineal o salida continua | No cambia el valor |
| Escalón | Perceptrón clásico | Produce una salida binaria |
| Sigmoide | Probabilidad binaria | Comprime valores entre 0 y 1 |
| Tanh | Representaciones centradas | Comprime valores entre -1 y 1 |
| ReLU | Capas ocultas profundas | Activa valores positivos y anula negativos |
| Leaky ReLU | Variante de ReLU | Evita que neuronas queden completamente inactivas |

---

### Qué es el perceptrón

El perceptrón es una de las formas más simples de red neuronal. Puede entenderse como una neurona artificial utilizada para clasificación binaria.

Recibe entradas, calcula una combinación lineal, aplica una función de activación y decide entre dos clases.

```text
Entrada
   ↓
Suma ponderada
   ↓
Función de activación
   ↓
Clase 0 o clase 1
```

---

### Qué es una frontera de decisión

Una frontera de decisión es la línea, plano o superficie que separa clases en el espacio de datos.

En dos dimensiones, un perceptrón genera una recta:

```text
w₁x₁ + w₂x₂ + b = 0
```

Los puntos que quedan de un lado se clasifican como una clase, y los puntos que quedan del otro lado se clasifican como la otra clase.

---

### Por qué XOR es importante

XOR es un ejemplo clásico porque no puede separarse con una sola recta.

Esto muestra una limitación del perceptrón simple y permite introducir la necesidad de redes con capas ocultas.

```text
AND, OR, NAND, NOR → pueden separarse linealmente
XOR → no puede separarse linealmente con una sola neurona
```

---

### Qué es una función de pérdida

Una función de pérdida mide qué tan lejos está la predicción del modelo respecto del valor verdadero.

Si la pérdida es alta, el modelo está prediciendo mal. Si la pérdida baja, el modelo está mejorando.

```text
L = (y - ŷ)²
```

---

### Qué es el descenso por gradiente

El descenso por gradiente es un método de optimización que permite ajustar los parámetros del modelo para reducir la pérdida.

La idea es moverse en la dirección contraria al gradiente, porque el gradiente indica hacia dónde aumenta más rápido la pérdida.

```text
w ← w - η · ∂L/∂w
```

Donde:

- `w` es el peso;
- `η` es el learning rate;
- `∂L/∂w` es la derivada de la pérdida respecto del peso.

---

### Qué es forward propagation

Forward propagation es el proceso mediante el cual la información avanza desde las entradas hasta la salida de la red.

```text
Entrada
   ↓
Capa oculta
   ↓
Activación
   ↓
Capa de salida
   ↓
Predicción
```

Durante este proceso, la red calcula una predicción usando los pesos y sesgos actuales.

---

### Qué es backpropagation

Backpropagation es el proceso mediante el cual la red calcula cómo debe modificar sus pesos para reducir el error.

Primero se calcula la pérdida. Luego se calcula cómo cambia esa pérdida respecto de cada parámetro. Finalmente, los pesos se actualizan usando descenso por gradiente.

```text
Error en la salida
        ↓
Cálculo de gradientes
        ↓
Propagación hacia atrás
        ↓
Actualización de pesos
```

---

### Qué es regularización

La regularización agrupa técnicas orientadas a reducir el sobreajuste y mejorar la capacidad de generalización del modelo.

| Técnica | Idea principal |
| :------ | :------------- |
| L1 | Favorece pesos exactamente cero |
| L2 | Penaliza pesos grandes |
| Dropout | Desactiva neuronas durante entrenamiento |
| Early stopping | Detiene el entrenamiento cuando empeora la validación |
| Menor complejidad | Reduce cantidad de parámetros |
| Más datos | Mejora la capacidad de generalizar |

---

## ✅ Preguntas orientadoras para estudiantes

1. ¿Qué representa un peso en una neurona artificial?
2. ¿Qué función cumple el sesgo?
3. ¿Por qué una función de activación es necesaria?
4. ¿Qué diferencia hay entre una función lineal y una no lineal?
5. ¿Qué es una frontera de decisión?
6. ¿Por qué XOR no puede resolverse con un perceptrón simple?
7. ¿Qué mide una función de pérdida?
8. ¿Qué indica el gradiente?
9. ¿Qué ocurre si el learning rate es demasiado alto?
10. ¿Qué calcula forward propagation?
11. ¿Qué calcula backpropagation?
12. ¿Por qué se usa la regla de la cadena?
13. ¿Qué es overfitting?
14. ¿Qué diferencia hay entre error de entrenamiento y error de validación?
15. ¿Cómo ayuda la regularización a mejorar la generalización?

---

## 🧾 Síntesis final

Una red neuronal puede entenderse como una composición de funciones parametrizadas. Cada neurona transforma entradas mediante pesos, sesgo y activación. Al combinar muchas neuronas en capas, la red puede representar patrones complejos.

El entrenamiento consiste en comparar predicciones con valores reales, calcular una pérdida, estimar gradientes y actualizar pesos para reducir el error.

Sin embargo, reducir el error de entrenamiento no es suficiente. Un modelo útil debe generalizar. Por eso, técnicas como regularización, dropout, early stopping y control de complejidad son fundamentales para construir redes neuronales más robustas.

---

# 🧠 Autoencoders · Recursos interactivos de estudio

> Material organizado para estudiar **autoencoders**, **espacio latente**, **manifold**, **embeddings**, **arquitectura encoder-decoder**, **bottleneck**, **denoising**, **detección de anomalías**, **Variational Autoencoders** y práctica en **Google Colab** mediante teoría visual, simulaciones interactivas y recursos didácticos para clase.

---

## 🎯 Objetivo general del bloque

Este conjunto de recursos tiene como objetivo comprender los **autoencoders** desde una perspectiva conceptual, visual y práctica.

El bloque parte de la idea de una red que aprende a reconstruir su propia entrada, pero avanza hacia una interpretación más profunda: el modelo aprende una representación interna comprimida que puede servir para reducir dimensionalidad, extraer patrones, limpiar ruido, detectar anomalías y construir espacios latentes útiles para generación.

La finalidad es que el estudiante pueda comprender que un autoencoder no es una copia mecánica de la entrada, sino un sistema entrenable que transforma datos mediante encoder, bottleneck, espacio latente, decoder y función de reconstrucción.

---

## 🧭 Secuencia didáctica sugerida

```text
1. Espacio latente, manifold y embeddings
        ↓
2. Aplicaciones de los autoencoders
        ↓
3. Teoría completa de autoencoders
        ↓
4. Arquitectura encoder-decoder y bottleneck
        ↓
5. Espacio latente y manifold interactivo
        ↓
6. Denoising autoencoder
        ↓
7. Anomalías y error de reconstrucción
        ↓
8. Variational Autoencoder interactivo
        ↓
9. Guía práctica en Colab
        ↓
10. Simulación fija 784 → z=32
```

---

## 📚 Recursos interactivos

<table>
  <thead>
    <tr>
      <th align="center">Orden</th>
      <th align="left">Recurso</th>
      <th align="left">Propósito didáctico</th>
      <th align="center">Abrir HTML</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><strong>0</strong></td>
      <td><strong>Índice de la clase</strong></td>
      <td>Organiza el bloque completo y permite navegar todos los HTML desde un punto central.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/00_indice_clase_autoencoders.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-%C3%8Dndice-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Índice de la clase">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>1.1</strong></td>
      <td><strong>Espacio latente, manifold y embeddings</strong></td>
      <td>Desarrolla los conceptos de representación interna, manifold, embeddings y reducción semántica de dimensionalidad.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_1_espacio_latente_manifold_embeddings_teoria.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Teor%C3%ADa%20latente-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Espacio latente, manifold y embeddings">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>1.2</strong></td>
      <td><strong>Aplicaciones de los autoencoders</strong></td>
      <td>Presenta usos concretos: compresión, denoising, anomalías, embeddings, representación y modelos generativos.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_2_aplicaciones_autoencoders.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Aplicaciones-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Aplicaciones de los autoencoders">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>1</strong></td>
      <td><strong>Teoría completa de autoencoders</strong></td>
      <td>Explica arquitectura encoder-decoder, bottleneck, reconstrucción, pérdida, entrenamiento y usos principales.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_teoria_completa_autoencoders.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Teor%C3%ADa%20completa-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Teoría completa de autoencoders">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>2</strong></td>
      <td><strong>Arquitectura y bottleneck</strong></td>
      <td>Simula la compresión desde la entrada hacia el espacio latente y la reconstrucción posterior.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/02_simulacion_arquitectura_bottleneck.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Bottleneck-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Arquitectura y bottleneck">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>3</strong></td>
      <td><strong>Espacio latente y manifold</strong></td>
      <td>Permite mover coordenadas latentes y observar cómo cambia una representación reconstruida.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/03_simulacion_espacio_latente_manifold.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Manifold-0891b2?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Espacio latente y manifold">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>4</strong></td>
      <td><strong>Denoising autoencoder</strong></td>
      <td>Muestra cómo un autoencoder aprende a recuperar una señal limpia desde una entrada con ruido.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/04_simulacion_denoising_autoencoder.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Denoising-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Denoising autoencoder">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>5</strong></td>
      <td><strong>Anomalías y error de reconstrucción</strong></td>
      <td>Explica la detección de anomalías mediante umbrales de error de reconstrucción.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_anomalias_error_reconstruccion.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Anomal%C3%ADas-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Anomalías y error de reconstrucción">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>6</strong></td>
      <td><strong>Variational Autoencoder interactivo</strong></td>
      <td>Introduce la lógica probabilística del VAE: media, varianza, muestreo y regularización latente.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/06_variational_autoencoder_interactivo.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-VAE-9333ea?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Variational Autoencoder interactivo">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>7</strong></td>
      <td><strong>Guía práctica en Colab</strong></td>
      <td>Ordena el flujo práctico para implementar autoencoders en Google Colab.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/07_guia_practica_colab_autoencoders.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Colab-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Guía práctica en Colab">
        </a>
      </td>
    </tr>
    <tr>
      <td align="center"><strong>8</strong></td>
      <td><strong>Autoencoder fijo 784 → z=32</strong></td>
      <td>Versión fija para clase: entrada 784, espacio latente 32 y visualización estable de compresión.</td>
      <td align="center">
        <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/08_Simulacion_autoencoder_fija_entrada_784_z32.html">
          <img src="https://img.shields.io/badge/Abrir%20HTML-Fijo%20784%20z32-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Autoencoder fijo 784 → z=32">
        </a>
      </td>
    </tr>
  </tbody>
</table>

---

## 🔗 Acceso directo a los recursos

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/00_indice_clase_autoencoders.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-0.%20%C3%8Dndice-1f4e79?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Índice de la clase">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_1_espacio_latente_manifold_embeddings_teoria.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-1.1.%20Teor%C3%ADa%20latente-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Espacio latente, manifold y embeddings">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_2_aplicaciones_autoencoders.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-1.2.%20Aplicaciones-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Aplicaciones de los autoencoders">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_teoria_completa_autoencoders.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-1.%20Teor%C3%ADa%20completa-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Teoría completa de autoencoders">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/02_simulacion_arquitectura_bottleneck.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-2.%20Bottleneck-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Arquitectura y bottleneck">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/03_simulacion_espacio_latente_manifold.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-3.%20Manifold-0891b2?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Espacio latente y manifold">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/04_simulacion_denoising_autoencoder.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-4.%20Denoising-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Denoising autoencoder">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_anomalias_error_reconstruccion.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-5.%20Anomal%C3%ADas-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Anomalías y error de reconstrucción">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/06_variational_autoencoder_interactivo.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-6.%20VAE-9333ea?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Variational Autoencoder interactivo">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/07_guia_practica_colab_autoencoders.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-7.%20Colab-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Guía práctica en Colab">
  </a>
</p>

<p align="center">
  <a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/08_Simulacion_autoencoder_fija_entrada_784_z32.html">
    <img src="https://img.shields.io/badge/Abrir%20HTML-8.%20Fijo%20784%20z32-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Autoencoder fijo 784 → z=32">
  </a>
</p>

---

## 🧩 Resumen didáctico de cada recurso

### 0. Índice de la clase

El índice funciona como la puerta de entrada al bloque completo. Permite ordenar los materiales, acceder rápidamente a cada HTML y presentar una secuencia clara para estudiar autoencoders.

Su utilidad principal es transformar varios archivos separados en una experiencia de aprendizaje organizada. Desde este recurso, el estudiante puede iniciar la clase, recorrer las simulaciones y volver al punto central cuando lo necesite.

**Idea clave:** el índice convierte varios archivos separados en un recorrido didáctico navegable.

---

### 1.1. Espacio latente, manifold y embeddings

Este recurso presenta los conceptos de representación interna. Permite comprender que el autoencoder no trabaja solamente con datos originales, sino con coordenadas latentes que condensan patrones relevantes.

El espacio latente puede pensarse como una zona de representación donde datos similares tienden a quedar cerca. La noción de manifold ayuda a explicar por qué muchos datos de alta dimensión, como imágenes o señales, pueden estar organizados sobre estructuras de menor dimensión.

Permite trabajar:

- espacio latente;
- manifold;
- embeddings;
- representación interna;
- reducción de dimensionalidad;
- vecindad semántica;
- interpolación;
- geometría de datos.

**Idea clave:** el espacio latente es una representación comprimida donde la cercanía puede tener significado semántico o estructural.

---

### 1.2. Aplicaciones de los autoencoders

Este recurso conecta la arquitectura con problemas reales. Permite mostrar que los autoencoders no son solamente una curiosidad académica, sino una familia de modelos con aplicaciones prácticas en ciencia de datos, inteligencia artificial, visión por computadora, análisis de señales, detección de anomalías y modelos generativos.

Permite trabajar:

- compresión;
- reducción de dimensionalidad;
- limpieza de ruido;
- detección de anomalías;
- embeddings;
- recuperación de información;
- representación de imágenes;
- generación de datos;
- preentrenamiento;
- visualización de datos.

**Idea clave:** los autoencoders son útiles porque aprenden representaciones, no solo porque reconstruyen entradas.

---

### 1. Teoría completa de autoencoders

Este recurso introduce la arquitectura encoder-decoder, el bottleneck, la reconstrucción, la función de pérdida y el aprendizaje por optimización.

El estudiante puede comprender que el modelo recibe una entrada, la comprime en una representación latente y luego intenta reconstruirla. Si la reconstrucción mejora durante el entrenamiento, significa que el modelo está aprendiendo patrones relevantes de los datos.

Permite trabajar:

- encoder;
- decoder;
- bottleneck;
- reconstrucción;
- función de pérdida;
- error de reconstrucción;
- entrenamiento;
- aprendizaje no supervisado;
- reducción de dimensionalidad;
- generalización.

**Idea clave:** un autoencoder aprende a reconstruir bien al mismo tiempo que reduce la información a una representación interna útil.

---

### 2. Arquitectura y bottleneck

Este recurso permite visualizar cómo una entrada de alta dimensión se comprime en un cuello de botella y luego se reconstruye.

El bottleneck es central porque obliga al modelo a sintetizar información. Si el espacio latente es demasiado grande, el modelo puede copiar; si es demasiado pequeño, puede perder información relevante. Por eso, la arquitectura define una tensión entre compresión y fidelidad de reconstrucción.

Permite trabajar:

- entrada de alta dimensión;
- capas del encoder;
- compresión progresiva;
- bottleneck;
- vector latente;
- decoder;
- reconstrucción;
- pérdida de información;
- capacidad del modelo.

**Idea clave:** el bottleneck obliga al modelo a conservar lo importante y descartar redundancia.

---

### 3. Espacio latente y manifold

Este recurso muestra cómo cambiar coordenadas latentes modifica la reconstrucción. Sirve para explicar interpolación, continuidad y estructura geométrica.

La simulación permite observar que una modificación en el espacio latente no equivale a cambiar un píxel aislado, sino a modificar una representación aprendida. Esto ayuda a comprender por qué los espacios latentes son importantes para generación, búsqueda de similitud y representación semántica.

Permite trabajar:

- coordenadas latentes;
- interpolación;
- continuidad;
- manifold;
- reconstrucción;
- vecindad;
- representación semántica;
- geometría de datos.

**Idea clave:** moverse en el espacio latente no modifica píxeles aislados, modifica una representación aprendida.

---

### 4. Denoising autoencoder

Este recurso explica cómo entrenar con entradas ruidosas y salidas limpias permite aprender patrones robustos.

El modelo no debe copiar el ruido, sino recuperar la estructura subyacente. Por eso, el denoising autoencoder es útil para explicar la diferencia entre memorizar datos y aprender regularidades.

Permite trabajar:

- ruido;
- señal limpia;
- entrada corrupta;
- reconstrucción limpia;
- robustez;
- patrones relevantes;
- generalización;
- aprendizaje de estructura.

**Idea clave:** el modelo aprende estructura, no simplemente copia ruido.

---

### 5. Anomalías y error de reconstrucción

Este recurso permite estudiar cómo un modelo entrenado con patrones normales puede detectar casos raros por alto error de reconstrucción.

La idea central es que un autoencoder reconstruye bien aquello que se parece a lo que vio durante el entrenamiento. Cuando aparece una observación diferente, extraña o atípica, la reconstrucción suele ser peor y el error aumenta.

Permite trabajar:

- normalidad;
- anomalía;
- error de reconstrucción;
- umbral;
- detección;
- falsos positivos;
- falsos negativos;
- monitoreo;
- scoring de anomalía.

**Idea clave:** una anomalía suele reconstruirse peor porque no pertenece al patrón aprendido.

---

### 6. Variational Autoencoder interactivo

Este recurso introduce la lógica probabilística del VAE mediante media, varianza, muestreo y regularización del espacio latente.

A diferencia de un autoencoder clásico, el VAE no codifica cada entrada como un punto fijo, sino como una distribución. Esto permite generar nuevas muestras y construir un espacio latente más regular.

Permite trabajar:

- encoder probabilístico;
- media;
- varianza;
- desviación estándar;
- muestreo;
- truco de reparametrización;
- pérdida de reconstrucción;
- divergencia KL;
- generación;
- regularización latente.

**Idea clave:** un VAE aprende una distribución latente desde la cual se pueden generar nuevas muestras.

---

### 7. Guía práctica en Colab

Este recurso organiza el flujo para implementar un autoencoder en Python: datos, arquitectura, entrenamiento, reconstrucción y evaluación.

Es especialmente útil para pasar de la explicación conceptual a una práctica reproducible. Puede utilizarse como puente entre la clase teórica y el trabajo con código en Google Colab.

Permite trabajar:

- carga de datos;
- preprocesamiento;
- definición del encoder;
- definición del decoder;
- entrenamiento;
- validación;
- visualización de reconstrucciones;
- análisis del error;
- comparación de modelos.

**Idea clave:** la teoría se consolida cuando el estudiante puede pasar del concepto al código.

---

### 8. Simulación fija 784 → z=32

Esta simulación presenta una entrada fija de 784 dimensiones, como una imagen tipo 28 x 28, y un espacio latente de 32 dimensiones.

Es útil para clase porque evita que demasiados controles distraigan del concepto principal. El foco está en mostrar la relación entre una entrada de alta dimensión, una compresión fuerte y una reconstrucción aproximada.

Permite trabajar:

- entrada 784;
- imagen 28 x 28;
- vector latente z=32;
- compresión;
- reconstrucción;
- pérdida informacional;
- representación compacta;
- explicación visual estable.

**Idea clave:** una imagen de 784 dimensiones puede comprimirse en un vector latente mucho menor y luego reconstruirse aproximadamente.

---

## 🗺️ Mapa conceptual del módulo

```text
Autoencoders
│
├── Entrada
│   ├── Imagen
│   ├── Señal
│   ├── Texto vectorizado
│   └── Datos tabulares
│
├── Encoder
│   ├── Compresión
│   ├── Extracción de características
│   └── Proyección latente
│
├── Bottleneck
│   ├── Reducción de dimensionalidad
│   ├── Restricción informacional
│   └── Representación comprimida
│
├── Espacio latente
│   ├── Manifold
│   ├── Embeddings
│   ├── Vecindad semántica
│   └── Interpolación
│
├── Decoder
│   ├── Reconstrucción
│   ├── Recuperación aproximada
│   └── Generación
│
├── Función de pérdida
│   ├── Error de reconstrucción
│   ├── MSE
│   ├── BCE
│   └── Regularización
│
├── Variantes
│   ├── Denoising autoencoder
│   ├── Sparse autoencoder
│   ├── Convolutional autoencoder
│   └── Variational autoencoder
│
└── Aplicaciones
    ├── Compresión
    ├── Reducción de dimensionalidad
    ├── Detección de anomalías
    ├── Limpieza de ruido
    ├── Representaciones latentes
    └── Generación de datos
```

---

## 📖 Guía rápida de uso

### Para comenzar desde cero

Usar primero el recurso de teoría completa.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_teoria_completa_autoencoders.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Teor%C3%ADa%20completa-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir teoría completa">
</a>

Este recurso permite presentar la intuición general: un autoencoder recibe datos, los comprime, los reconstruye y aprende a partir del error de reconstrucción.

---

### Para explicar espacio latente, manifold y embeddings

Usar el recurso teórico específico.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_1_espacio_latente_manifold_embeddings_teoria.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Espacio%20latente-2563eb?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir espacio latente">
</a>

Flujo sugerido:

```text
Datos de alta dimensión
        ↓
Encoder
        ↓
Representación latente
        ↓
Manifold
        ↓
Vecindad semántica
        ↓
Reconstrucción o uso posterior
```

---

### Para explicar aplicaciones concretas

Usar el recurso de aplicaciones.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/01_2_aplicaciones_autoencoders.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Aplicaciones-0f766e?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir aplicaciones">
</a>

Este recurso permite conectar la arquitectura con usos reales en ciencia de datos, visión por computadora, anomalías, reducción de dimensionalidad y generación.

---

### Para explicar arquitectura y compresión

Usar el recurso de arquitectura y bottleneck.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/02_simulacion_arquitectura_bottleneck.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Bottleneck-7c3aed?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir bottleneck">
</a>

Flujo sugerido:

```text
Entrada
        ↓
Encoder
        ↓
Bottleneck
        ↓
Decoder
        ↓
Reconstrucción
        ↓
Error de reconstrucción
```

---

### Para explicar limpieza de ruido

Usar el recurso de denoising autoencoder.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/04_simulacion_denoising_autoencoder.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Denoising-15803d?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir denoising">
</a>

Este recurso permite mostrar que el modelo aprende estructura subyacente y no solo copia la entrada.

---

### Para explicar detección de anomalías

Usar el recurso de anomalías y error de reconstrucción.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/05_simulacion_anomalias_error_reconstruccion.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Anomal%C3%ADas-dc2626?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir anomalías">
</a>

Flujo sugerido:

```text
Entrenar con datos normales
        ↓
Reconstruir observaciones nuevas
        ↓
Medir error de reconstrucción
        ↓
Comparar contra umbral
        ↓
Clasificar como normal o anómalo
```

---

### Para explicar VAE y generación

Usar el recurso de Variational Autoencoder.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/06_variational_autoencoder_interactivo.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-VAE-9333ea?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir VAE">
</a>

Este recurso permite introducir la diferencia entre representar una entrada como punto fijo y representarla como distribución latente.

---

### Para cerrar con práctica

Usar la guía de Colab.

<a href="https://htmlpreview.github.io/?https://github.com/sgevatschnaider/data-science-for-business-models/blob/main/src/classroom/module_01_eda/html/07_guia_practica_colab_autoencoders.html">
  <img src="https://img.shields.io/badge/Abrir%20HTML-Colab-f59e0b?style=for-the-badge&logo=html5&logoColor=white" alt="Abrir Colab">
</a>

---

## 🧠 Desarrollo conceptual del tema

### Qué es un autoencoder

Un autoencoder es una red neuronal entrenada para reconstruir su propia entrada. Aunque parezca una tarea trivial, su valor aparece cuando se obliga al modelo a pasar por una representación interna comprimida o estructurada.

```text
Entrada original
        ↓
Encoder
        ↓
Espacio latente
        ↓
Decoder
        ↓
Reconstrucción
```

El objetivo no es copiar mecánicamente, sino aprender una transformación que conserve la información más relevante.

---

### Qué es el encoder

El encoder es la parte de la red que transforma la entrada original en una representación más compacta.

```text
x → encoder(x) → z
```

Donde:

- `x` es la entrada original;
- `z` es la representación latente.

---

### Qué es el bottleneck

El bottleneck es el cuello de botella de la arquitectura. Es la zona donde la información queda comprimida.

Si el bottleneck es muy amplio, el modelo puede copiar. Si es muy estrecho, puede perder demasiada información.

```text
Entrada 784 dimensiones → Bottleneck 32 dimensiones
```

---

### Qué es el decoder

El decoder toma el vector latente y trata de reconstruir la entrada original.

```text
z → decoder(z) → x reconstruida
```

---

### Qué es el error de reconstrucción

El error de reconstrucción mide la diferencia entre la entrada original y la reconstrucción generada por el modelo.

```text
Error = diferencia entre x y x̂
```

Una reconstrucción buena tiene bajo error. Una reconstrucción mala tiene alto error.

---

### Qué es el espacio latente

El espacio latente es el espacio donde viven las representaciones comprimidas aprendidas por el encoder.

En lugar de trabajar con todos los datos originales, el modelo trabaja con una versión más compacta y organizada.

```text
Datos originales → Representación latente → Reconstrucción o análisis
```

---

### Qué es un manifold

Un manifold puede entenderse como una estructura de menor dimensión dentro de un espacio de mayor dimensión.

Por ejemplo, aunque una imagen tenga miles de píxeles, las variaciones significativas pueden depender de menos factores: forma, orientación, intensidad, textura o clase.

---

### Qué es un embedding

Un embedding es una representación vectorial de un objeto.

En autoencoders, el vector latente puede funcionar como embedding porque resume información relevante de la entrada en pocas dimensiones.

---

### Qué es un denoising autoencoder

Un denoising autoencoder se entrena con entradas ruidosas, pero intenta reconstruir versiones limpias.

```text
Entrada con ruido
        ↓
Autoencoder
        ↓
Reconstrucción limpia
```

Esto obliga al modelo a aprender patrones estructurales y no simplemente a copiar el ruido.

---

### Qué es la detección de anomalías con autoencoders

Si un autoencoder fue entrenado con datos normales, aprende a reconstruir bien ese tipo de datos.

Cuando recibe una observación anómala, puede reconstruirla mal. Esa diferencia se mide con el error de reconstrucción.

```text
Error bajo → observación normal
Error alto → posible anomalía
```

---

### Qué es un Variational Autoencoder

Un Variational Autoencoder, o VAE, es una variante probabilística del autoencoder.

En lugar de codificar una entrada como un único punto latente, la codifica como una distribución.

```text
Entrada
        ↓
Encoder
        ↓
Media y varianza
        ↓
Muestreo de z
        ↓
Decoder
        ↓
Reconstrucción o generación
```

Esto permite generar nuevas muestras desde el espacio latente.

---

## ✅ Preguntas orientadoras para estudiantes

1. ¿Qué aprende realmente un autoencoder?
2. ¿Por qué el bottleneck es importante?
3. ¿Qué diferencia hay entre copiar la entrada y reconstruirla después de comprimirla?
4. ¿Qué representa el espacio latente?
5. ¿Cómo se relacionan espacio latente, manifold y embeddings?
6. ¿Por qué un denoising autoencoder puede limpiar ruido?
7. ¿Cómo se usa el error de reconstrucción para detectar anomalías?
8. ¿Qué cambia cuando pasamos de un autoencoder clásico a un VAE?
9. ¿Por qué el VAE introduce una dimensión probabilística?
10. ¿Qué aplicaciones prácticas justifican estudiar autoencoders?
11. ¿Qué ocurre si el espacio latente es demasiado grande?
12. ¿Qué ocurre si el espacio latente es demasiado pequeño?
13. ¿Cómo se interpreta un vector latente?
14. ¿Por qué la reconstrucción perfecta no siempre es el objetivo más importante?
15. ¿Cómo se puede usar un autoencoder para reducción de dimensionalidad?

---

## 🧾 Síntesis final

Un autoencoder puede entenderse como una red que aprende una representación comprimida de los datos. El encoder transforma la entrada en un espacio latente, el bottleneck obliga a sintetizar información y el decoder intenta reconstruir la entrada original.

La potencia del modelo no está solo en reconstruir, sino en aprender representaciones útiles. Por eso los autoencoders son relevantes para reducción de dimensionalidad, limpieza de ruido, detección de anomalías, embeddings y modelos generativos como los Variational Autoencoders.

---

**Material elaborado por el profesor Sergio Gevatschnaider**
