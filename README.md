<div align="center">

Impacto del uso de inteligencia artificial en estudiantes

Exploración de datos, análisis multivariado y clusterización en R



Ver informe publicado ·Dataset original ·Presentación ·Respaldo

</div>

Descripción

Este proyecto analiza el impacto del uso de inteligencia artificial generativa en estudiantes a partir del conjunto de datos Impact of AI on Students.

El estudio relaciona el uso de IA con variables académicas y personales, como el promedio antes y después del semestre, las horas de estudio tradicional, la dependencia percibida, la ansiedad durante los exámenes, la retención de habilidades y el riesgo de agotamiento.

El análisis fue desarrollado en R Markdown e incluye limpieza de datos, análisis univariado, análisis bivariado, Análisis de Componentes Principales y clusterización mediante K-means.

Los resultados son descriptivos y asociativos. No demuestran que el uso de IA cause directamente mejoras o deterioros académicos.

Objetivo general

Analizar las características académicas, los hábitos de estudio y el uso de inteligencia artificial generativa en estudiantes mediante técnicas de exploración de datos, análisis multivariado y clusterización.

Dataset

Característica

Descripción

Nombre

Impact of AI on Students

Fuente

Kaggle

Unidad de observación

Estudiante

Registros

50 000

Variables

16

Variables numéricas analizadas

8

Variables categóricas

6

Variable lógica

1

Identificador

Student_ID

El conjunto de datos incluye información sobre:

Área académica y año de estudio.

Promedio antes y después del semestre.

Horas semanales de uso de IA generativa.

Uso principal de la IA.

Habilidad para crear prompts.

Diversidad de herramientas utilizadas.

Horas de estudio tradicional.

Dependencia percibida de la IA.

Ansiedad durante los exámenes.

Retención de habilidades.

Riesgo de agotamiento académico.

Metodología

El proyecto se desarrolló mediante las siguientes etapas:

Carga y revisión inicial: estructura, dimensiones y tipos de datos.

Limpieza y preparación: normalización de textos, conversión de tipos, faltantes, duplicados, rangos y valores atípicos.

Análisis univariado: estadísticos descriptivos, histogramas, diagramas de caja, prueba de Lilliefors y gráficos Q-Q.

Análisis bivariado: correlaciones de Pearson y Spearman, chi-cuadrado, V de Cramer y Kruskal-Wallis.

Análisis multivariado: estandarización y Análisis de Componentes Principales.

Clusterización: selección del número de clústeres mediante codo y silueta, aplicación de K-means y caracterización de perfiles.

Interpretación: resultados principales, conclusiones y limitaciones.

Principales resultados

Resultado

Valor

Registros finales

50 000

Valores faltantes

0

Filas duplicadas

0

Valores fuera de rango

0

Promedio previo al semestre

3,146

Promedio posterior al semestre

3,349

Diferencia promedio

0,203

Mayor correlación de Spearman

0,917

Varianza explicada por CP1 y CP2

48,8 %

Varianza explicada por CP1, CP2 y CP3

63,6 %

Clústeres seleccionados

3

Silueta promedio final

0,187

La relación numérica más intensa se encontró entre el promedio previo y el promedio posterior al semestre.

El modelo K-means identificó tres perfiles aproximados:

Clúster

Proporción aproximada

Características principales

1

31,35 %

Menor rendimiento académico y menor retención de habilidades

2

50,90 %

Mayor rendimiento académico, mayor retención y más estudio tradicional

3

17,75 %

Uso elevado de IA, mayor dependencia percibida y mayor ansiedad

La silueta promedio de 0,187 indica una separación débil. Por esta razón, los clústeres se interpretan como perfiles generales con traslape y no como grupos completamente diferenciados.

Tecnologías utilizadas

R

R Markdown

HTML y CSS

tidyverse

ggplot2

knitr

scales

cluster

nortest

Git y GitHub

GitHub Pages

Estructura del proyecto

Proyecto/
├── Codigos/
│   ├── EDA_Impacto_IA_Estudiantes.Rmd
│   └── estilos.css
├── DataSet/
│   └── ai_student_impact_dataset.csv
├── Documentacion/
├── Iconos/
├── PPT/
└── README.md

Ejecución local

1. Clonar el repositorio

git clone https://github.com/andreyac1397/impacto-del-uso-de-inteligencia-artificial-en-estudiantes.git
cd impacto-del-uso-de-inteligencia-artificial-en-estudiantes

2. Abrir el archivo R Markdown

Abra en RStudio:

Codigos/EDA_Impacto_IA_Estudiantes.Rmd

3. Instalar las librerías necesarias

install.packages(
  c(
    "tidyverse",
    "knitr",
    "scales",
    "cluster",
    "nortest"
  )
)

4. Utilizar una ruta relativa para el dataset

Para que el proyecto funcione en cualquier computadora, se recomienda configurar el parámetro del archivo R Markdown así:

params:
  ruta_csv: "../DataSet/ai_student_impact_dataset.csv"

No se recomienda conservar una ruta absoluta como C:/Users/..., porque solo funcionaría en la computadora donde fue creada.

5. Generar el informe

En RStudio, presione Knit para crear el informe HTML.

Recursos

Recurso

Enlace

Informe interactivo

Abrir sitio publicado

Repositorio

Abrir en GitHub

Dataset

Abrir en Kaggle

Presentación

Abrir en Canva

Respaldo

Abrir en Google Drive

El informe publicado también permite abrir la impresión del navegador para guardarlo localmente en formato PDF.

Integrantes

Brandon Josué Acuña Gamboa

Desmond Akin Bermúdez Rodríguez

Andrey Calderón Vega

Erick Andrés Picado Mora

Información académica

Institución: Colegio Universitario de Cartago

Carrera: Tecnologías de Información – Big Data

Curso: BD-142 Exploración de Datos

Profesor: Ronald Córdoba Vega

Fecha de entrega: 03 de agosto de 2026

Limitaciones principales

El análisis es observacional y no permite establecer causalidad.

Algunas variables representan percepciones personales.

Las pruebas estadísticas pueden ser sensibles al tamaño de la muestra.

Los dos primeros componentes no conservan toda la variabilidad original.

K-means supone grupos compactos y utiliza distancia euclidiana.

La separación débil de los clústeres limita la definición de perfiles completamente independientes.

<div align="center">

Desarrollado como proyecto académico para el curso BD-142 Exploración de Datos.

</div>
