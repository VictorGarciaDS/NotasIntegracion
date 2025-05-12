# 📘 Notas de Integración

Este repositorio contiene mis notas personales sobre **cálculo integral**, redactadas en **LaTeX**. Las desarrollé para un **seminario interno sobre técnicas de integración** en el Departamento de Matemáticas de la Universidad de Guanajuato.

> ✍️ Durante ese seminario, noté que incluso estudiantes avanzados —incluyendo personas en programas de doctorado— tenían dificultades con técnicas de integración básicas. Por ello decidí crear un material claro, accesible y cuidadosamente estructurado.

<div align="center">
  <img src="preview.png" alt="Vista previa del PDF" width="600"/>
</div>

## 📄 Contenido

- Notación
- Las fórmulas de derivadas
  - Las fórmulas de derivadas
    -Funciones algebráicas
    -Funciones trascendentes
- La diferencial
  - Las fórmulas de diferenciales
- Integracion de formas elementales ordinarias
  - Integrales inmediatas
  - Algunas integrales casi inmediatas
  - La importancia de la elección de dv
  - Ejercicios
  - Resumen de las fórmulas
  - Problemas
- Artificios de integración
  - Cambio de variable o sustitución algebráica
  - Sustitución trigonométricas
  - Integración por partes
  - Descomposición en fracciones parciales
  - Exponentes racionales
  - Integrales de diferencias binomias
- Algunas integrales resueltas

El archivo `NotasIntegracion.pdf` incluye hipervínculos internos y estructura clara para facilitar su consulta.

## ⚙️ Automatización con CI/CD

El desarrollo de este repositorio incluye un flujo automatizado de **CI/CD**:

- Las notas se redactan en [Overleaf](https://www.overleaf.com), conectado vía Git.
- Como Overleaf no actualiza la fecha del archivo `NotasIntegracion.pdf`, **Git no detecta cambios automáticamente de archivos que no son de texto plano**.
- Para resolverlo, GitHub ejecuta un **job que recompila el archivo PDF desde el `.tex`** cada vez que se hace `push` de archivos
  - **.tex**
  - **.bib**
  - **.sty**
  - **.cls**
  - **.png**
  - **.jpg**
  - **.pdf**
  - **.eps**
- Un segundo job **envía automáticamente el PDF generado a mi portafolio alojado en [Gitlab](https://gitlab.com/mackonde1/victorgarciads-site)**.

> ⚙️ Esto asegura que el PDF más reciente esté disponible tanto en GitHub como en mi sitio público, sin intervención manual.
