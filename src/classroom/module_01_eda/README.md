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

> **Versión 2.0 mejorada del bloque de recursos para el parcial**  
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

El recorrido recomendado para este módulo es comenzar con la explicación conceptual, continuar con la simulación interactiva, repasar con el cuestionario, consolidar vocabulario con el glosario y finalmente practicar en Colab.







