---
title: "Interfaces cerebro-computadora y desarrollo de aplicaciones innovadoras con IDUN Guardian"
description: Tesis de grado de Pedro Jossi y Robertino Agnone Cóccaro, dirigida por el Dr. Ignacio Larrabide
header-img: images/tesis-grado/2026-07-jossi-agnone-idun-guardian.png
categories: tesis-grado
---

<div class="image-post-container">
    <img src="/images/tesis-grado/2026-07-jossi-agnone-idun-guardian.png"/>
</div>

### Resumen

Este Proyecto Integrador evalúa la viabilidad técnica de un sistema de Interfaz Cerebro-Computadora pasiva para la estimación de la carga cognitiva, utilizando las señales de un dispositivo EEG in-ear comercial de un único canal, el IDUN Guardian. Para ello, se diseñó e implementó un pipeline de procesamiento de bioseñales y machine learning, operando sobre un conjunto de datos de 16 participantes sometidos a la tarea neuropsicológica n-back.

La metodología abarcó el filtrado digital, estrategias de segmentación temporal y la extracción de características. La fase de modelado predictivo puso en contraste el rendimiento de los algoritmos Support Vector Machine y Random Forest bajo dos esquemas distintos: intra-sujeto (Within-Subject) y entre-sujetos (Leave-One-Subject-Out).

Los resultados demostraron que Random Forest supera consistentemente a Support Vector Machine. En la evaluación intra-sujeto, el sistema logró diferenciar con éxito los estados de carga cognitiva, sin embargo, al exponer el modelo a individuos desconocidos, la precisión sufrió una degradación, convergiendo a niveles cercanos al azar. Además, el análisis de saturación dimensional evidenció que un subconjunto acotado de características es suficiente para maximizar el rendimiento, mitigando el sobrecosto computacional.
