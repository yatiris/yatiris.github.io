---
title:  Adecuaciones experimentales y nuevos enfoques de aprendizaje automático para aplicaciones en estudios de sueño y detección de glaucoma
description: Tesis doctoral de Eugenia Moris, dirigida por los Doctores Ignacio Larrabide y José Ignacio Orlando 
header-img: images/tesis-grado/2024_moris.png
categories: tesis-doctorado
---

*Podés acceder al documento de la tesis (proximamente)

<div class="image-post-container">
    <img src="/images/tesis-grado/2024_moris.png"/>
</div>


## Resumen

Las señales biomédicas desempeñan un papel fundamental en el diagnóstico y tratamiento médico, aunque su interpretación está limitada por la subjetividad, el ruido y la variabilidad entre pacientes. Esta tesis doctoral aborda dos problemas cruciales en el ámbito de la salud mediante el desarrollo de soluciones basadas en aprendizaje automático: **la clasificación automática de etapas de sueño** a partir de señales de polisomnografía (PSG) y **la segmentación del disco óptico (OD) y la copa óptica (OC)** en imágenes de fondo de ojo para la detección temprana de glaucoma.

### Contribución 1: Clasificación de Etapas de Sueño

En el ámbito de la medicina del sueño, la clasificación manual de etapas de sueño es un proceso tedioso y subjetivo que requiere la experiencia de especialistas. Esta tesis evalúa cómo diferentes factores metodológicos y clínicos influyen en el rendimiento de modelos de aprendizaje automático para esta tarea.

**Aspectos clave investigados:**

- **Uso de múltiples canales:** Se demostró que incorporar señales de electroencefalografía (EEG), electrooculografía (EOG) y electromiografía (EMG) mejora significativamente la precisión en comparación con el enfoque común de utilizar un solo canal de EEG.

- **Efecto de la edad:** La edad del paciente es un factor crucial que afecta las características de las señales de sueño. Se incorporó la edad como variable demográfica en los modelos, demostrando mejoras en la clasificación, especialmente en grupos de edad específicos.

- **Sueño temprano vs. tardío:** Se analizó la importancia de las fases específicas del ciclo de sueño (sueño temprano y tardío), encontrando diferencias significativas en el rendimiento del modelo según la fase analizada.

**Metodología:** Se utilizaron algoritmos de Bosques Aleatorios (Random Forest) entrenados con características extraídas mediante transformadas de ondicula (wavelets) de las señales de PSG. Se implementó un modelo en cascada para mejorar la clasificación de etapas específicas del sueño.

**Resultados:** El enfoque multidimensional y contextualizado médicamente demostró aumentar la exactitud en la clasificación de las etapas del sueño, superando las limitaciones de trabajos previos que ignoraban factores clínicos relevantes.

### Contribución 2: Segmentación de Disco y Copa Óptica para Detección de Glaucoma

El glaucoma es una de las principales causas de ceguera irreversible a nivel mundial. La segmentación precisa del disco óptico y la copa óptica en imágenes de fondo de ojo es fundamental para su detección temprana, ya que la relación copa-disco (Cup-to-Disc Ratio, CDR) es un indicador clave de la enfermedad.

**Aspectos clave investigados:**

- **Modelos en dos etapas vs. end-to-end:** Se cuestionó la necesidad de los modelos en dos etapas (que requieren recortar previamente la región de interés) que son comunes en la literatura. Se evaluó si esta práctica realmente mejora el rendimiento o si, por el contrario, elimina artificialmente variaciones importantes que el modelo debe aprender a manejar.

- **Aprendizaje semi-supervisado:** Se desarrolló un método semi-supervisado que aprovecha datos sin etiquetar para mejorar la capacidad de generalización del modelo a dominios no vistos durante el entrenamiento.

- **Eliminación de intervención manual:** El enfoque propuesto elimina la necesidad de recortar manualmente las imágenes, optimizando el flujo de trabajo clínico y permitiendo que el modelo aprenda a localizar y segmentar las estructuras de forma automática.

**Metodología:** Se implementaron y compararon diferentes arquitecturas de redes neuronales convolucionales (CNNs) para la segmentación, incluyendo modelos end-to-end que procesan la imagen completa sin preprocesamiento manual. Se utilizaron técnicas de aprendizaje semi-supervisado para generar pseudo-etiquetas y mejorar la robustez del modelo.

**Resultados:** El modelo semi-supervisado logró una segmentación robusta incluso en dominios no vistos durante el entrenamiento, mejorando significativamente la generalización. Este enfoque simplificado pero efectivo es especialmente relevante en entornos clínicos con alta variabilidad entre imágenes de diferentes equipos o poblaciones.

---

## Impacto y Conclusiones

Esta tesis doctoral demuestra la importancia de:

1. **Integrar conocimiento médico en el diseño de modelos de aprendizaje automático:** La incorporación de variables demográficas como la edad y el uso de múltiples canales de señales mejora significativamente el rendimiento en la clasificación de etapas de sueño.

2. **Cuestionar prácticas establecidas:** El análisis crítico de los modelos en dos etapas para segmentación de OD/OC revela que la práctica común de recortar imágenes puede no ser necesaria y puede incluso limitar la capacidad de generalización del modelo.

3. **Desarrollar soluciones prácticas para entornos clínicos:** Los métodos propuestos son más robustos, requieren menos intervención manual y generalizan mejor a datos no vistos, haciéndolos más apropiados para su aplicación en la práctica clínica real.

Las contribuciones de esta tesis avanzan el estado del arte en ambos campos, proporcionando herramientas más precisas, eficientes y generalizables para la clasificación de etapas de sueño y la detección temprana de glaucoma, dos problemas de gran relevancia en la salud pública.

---

## Publicaciones Derivadas

Los resultados de esta investigación han sido publicados en revistas y conferencias internacionales de prestigio, contribuyendo al avance del conocimiento en el área de aplicaciones médicas del aprendizaje automático.

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=DBzR_ML4Sd4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
