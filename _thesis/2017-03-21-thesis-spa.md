---
title: Ingeniería de descriptores y aprendizaje automático en la segmentación de ultrasonido intravascular
description: Tesis doctoral de Lucas Lo Vercio, dirigida por el Dr. Ignacio Larrabide y la Dra. Mariana del Fresno
header-img: images/tesis-grado/2017-lovercio.png
categories: tesis-doctorado
---
*Podés acceder al documento de la tesis [desde este link](https://www.ridaa.unicen.edu.ar/items/18bb4da3-4eaf-4daf-afed-6ce6c8d319bb).*


<div class="image-post-container">
    <img src="/images/tesis-grado/2017-lovercio.png"/>
</div>

### Resumen

El ultrasonido intravascular permite la visualización de arterias desde su interior para la evaluación de la enfermedad aterosclerótica y la eficiencia de tratamientos vasculares. El análisis automático es una valiosa herramienta para el diagnóstico clínico debido al gran número de imágenes generadas por estudio. Sin embargo, la presencia de ruido y artefactos convierte a la segmentación en un desafío computacional. El objetivo de esta tesis es la aplicación de técnicas de aprendizaje automático supervisado en la segmentación de la pared arterial, al tiempo que se evalúa la importancia de los descriptores de imagen propuestos en la literatura. Para la caracterización de las túnicas arteriales se utilizaron Maquinas de Vectores de Soporte. La mejor combinación de descriptores, obtenida utilizando Selección Secuencial, fue la compuesta por filtros de reducción de ruido e indicadores de textura basados en matrices de coocurrencia. El Bosque Aleatorio demostró ser eficaz para detectar estructuras morfológicas, mejorando su desempeño cuando fue combinado con submuestreo aleatorio. Para la segmentación de las interfaces lumen-íntima y media-adventicia, los clasificadores propuestos fueron incorporados exitosamente a un método basado en contornos activos. Los resultados obtenidos son altamente satisfactorios, lo que alienta su incorporación en técnicas de segmentación mas robustas.

### Abstract

Intravascular Ultrasound (IVUS) allows the visualization of arteries to assess atherosclerosis and vascular treatments effectiveness. The automatic analysis is valuable for clinical diagnosis due to the large number of images in the studies. Nevertheless, the presence of noise and artifacts in the images turns the segmentation into a computational challenge. The aim of the present thesis is the application of supervised machine learning methods to the automatic segmentation of the artery. Furthermore, the importance of state-of-the-art image features is assessed during the training process. For arterial layers characterization, Support Vector Machines were used. The best set of features, obtained through Sequential Forward Selection, was composed of noise reduction filters and textural descriptors based on gray level co-ocurrence matrixes. Random Forest demonstrated good performance to classify morphological structures when it was combined with Random Undersampling. For segmenting lumen-intima and media-adventitia interfaces, the classifiers were incorporated into a method based on deformable models. The obtained results were successful, suggesting their inclusion on more robust segmentation techniques.