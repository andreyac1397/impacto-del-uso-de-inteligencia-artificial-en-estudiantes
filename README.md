<div align="center">

<h1>🤖 Impacto del uso de inteligencia artificial en estudiantes</h1>

<p><strong>Exploración de datos · Análisis multivariado · ACP · K-means</strong></p>

<p>
  <img src="https://img.shields.io/badge/R-4.x-276DC3?style=for-the-badge&logo=r&logoColor=white" alt="R">
  <img src="https://img.shields.io/badge/R%20Markdown-Informe-1F65CC?style=for-the-badge&logo=rstudio&logoColor=white" alt="R Markdown">
  <img src="https://img.shields.io/badge/Estado-Completado-2E8B57?style=for-the-badge" alt="Estado completado">
  <img src="https://img.shields.io/badge/Curso-BD--142-17365D?style=for-the-badge" alt="Curso BD-142">
</p>

<p>
  <a href="https://andreyac1397.github.io/impacto-del-uso-de-inteligencia-artificial-en-estudiantes/">
    <img src="https://img.shields.io/badge/Ver_informe-225EA8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Ver informe">
  </a>
  <a href="https://www.kaggle.com/datasets/laveshjadon/ai-impact-on-students">
    <img src="https://img.shields.io/badge/Dataset-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Dataset">
  </a>
  <a href="https://canva.link/1fp54yzyha6ejyq">
    <img src="https://img.shields.io/badge/Presentación-7D2AE8?style=for-the-badge&logo=canva&logoColor=white" alt="Presentación">
  </a>
</p>

</div>

📌 Descripción

Este proyecto analiza el impacto del uso de inteligencia artificial generativa en estudiantes utilizando un conjunto de datos de 50 000 registros y 16 variables.

El estudio relaciona el uso de IA con el rendimiento académico, las horas de estudio, la dependencia percibida, la ansiedad durante los exámenes, la retención de habilidades y el riesgo de agotamiento.

[!IMPORTANT]Los resultados son descriptivos y asociativos. No demuestran que el uso de IA cause directamente mejoras o deterioros académicos.

🎯 Objetivo

Analizar las características académicas, los hábitos de estudio y el uso de inteligencia artificial generativa mediante técnicas de exploración de datos, análisis multivariado y clusterización.

🔎 Contenido del análisis

Etapa

Técnicas aplicadas

Preparación

Normalización, conversión de tipos, faltantes, duplicados y rangos

Análisis univariado

Estadísticos descriptivos, histogramas, boxplots, Lilliefors y Q-Q

Análisis bivariado

Pearson, Spearman, chi-cuadrado, V de Cramer y Kruskal-Wallis

Análisis multivariado

Estandarización y Análisis de Componentes Principales

Clusterización

Método del codo, silueta y K-means

Interpretación

Perfiles numéricos, perfiles categóricos, conclusiones y limitaciones

📊 Dataset

Característica

Resultado

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

Valores faltantes

0

Registros duplicados

0

Valores fuera de rango

0

Fuente: Impact of AI on Students — Kaggle

✨ Resultados principales

<table>
  <tr>
    <td align="center"><strong>3,146</strong><br>Promedio previo</td>
    <td align="center"><strong>3,349</strong><br>Promedio posterior</td>
    <td align="center"><strong>0,917</strong><br>Mayor Spearman</td>
    <td align="center"><strong>3</strong><br>Clústeres</td>
  </tr>
  <tr>
    <td align="center"><strong>48,8 %</strong><br>Varianza CP1 + CP2</td>
    <td align="center"><strong>63,6 %</strong><br>Varianza CP1–CP3</td>
    <td align="center"><strong>0,187</strong><br>Silueta final</td>
    <td align="center"><strong>Débil</strong><br>Separación</td>
  </tr>
</table>

Hallazgos destacados

La relación numérica más intensa se encontró entre el promedio previo y el promedio posterior al semestre.

Las horas semanales de uso de IA presentan una distribución asimétrica, con muchos valores bajos y algunos casos elevados.

Los primeros tres componentes principales concentran aproximadamente 63,6 % de la variabilidad.

K-means identificó tres perfiles aproximados, aunque existe traslape entre ellos.

👥 Perfiles identificados

Clúster

Tamaño aproximado

Características principales

1

31,35 %

Menor rendimiento académico y menor retención de habilidades

2

50,90 %

Mayor rendimiento, mayor retención y más estudio tradicional

3

17,75 %

Uso elevado de IA, mayor dependencia percibida y mayor ansiedad

[!NOTE]La silueta promedio fue de 0,187, por lo que estos clústeres deben interpretarse como perfiles generales y no como grupos completamente separados.

🛠️ Tecnologías

<p>
  <img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R">
  <img src="https://img.shields.io/badge/RStudio-75AADB?style=flat-square&logo=rstudio&logoColor=white" alt="RStudio">
  <img src="https://img.shields.io/badge/R_Markdown-1F65CC?style=flat-square&logo=rstudio&logoColor=white" alt="R Markdown">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub">
</p>

Paquetes de R

tidyverse · ggplot2 · knitr · scales · cluster · nortest

📁 Estructura del proyecto

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

▶️ Ejecución local

1. Clonar el repositorio

git clone https://github.com/andreyac1397/impacto-del-uso-de-inteligencia-artificial-en-estudiantes.git
cd impacto-del-uso-de-inteligencia-artificial-en-estudiantes

2. Instalar las dependencias

install.packages(
  c(
    "tidyverse",
    "knitr",
    "scales",
    "cluster",
    "nortest"
  )
)

3. Configurar la ruta del dataset

En el encabezado del archivo R Markdown utilice una ruta relativa:

params:
  ruta_csv: "../DataSet/ai_student_impact_dataset.csv"

4. Generar el informe

Abra Codigos/EDA_Impacto_IA_Estudiantes.Rmd en RStudio y presione Knit.

🔗 Recursos

Recurso

Acceso

🌐 Informe interactivo

Abrir informe

💻 Repositorio

Abrir GitHub

📊 Dataset original

Abrir Kaggle

🎞️ Presentación

Abrir Canva

💾 Respaldo

Abrir Google Drive

👨‍💻 Integrantes

<table>
  <tr>
    <td align="center"><strong>Brandon Josué<br>Acuña Gamboa</strong></td>
    <td align="center"><strong>Desmond Akin<br>Bermúdez Rodríguez</strong></td>
    <td align="center"><strong>Andrey<br>Calderón Vega</strong></td>
    <td align="center"><strong>Erick Andrés<br>Picado Mora</strong></td>
  </tr>
</table>

🎓 Información académica

Campo

Información

Institución

Colegio Universitario de Cartago

Carrera

Tecnologías de Información – Big Data

Curso

BD-142 Exploración de Datos

Profesor

Ronald Córdoba Vega

Fecha de entrega

03 de agosto de 2026

<details>
<summary><strong>⚠️ Ver limitaciones del análisis</strong></summary>

<br>

El análisis es observacional y no permite establecer causalidad.

Algunas variables representan percepciones personales.

Las pruebas estadísticas pueden ser sensibles al tamaño de la muestra.

Los dos primeros componentes no conservan toda la variabilidad original.

K-means supone grupos compactos y utiliza distancia euclidiana.

La separación débil limita la definición de perfiles completamente independientes.

</details>

<div align="center">

<p>Proyecto académico desarrollado para <strong>BD-142 Exploración de Datos</strong>.</p>

<p>
  <a href="https://andreyac1397.github.io/impacto-del-uso-de-inteligencia-artificial-en-estudiantes/">
    <strong>Consultar el informe completo →</strong>
  </a>
</p>

</div>
