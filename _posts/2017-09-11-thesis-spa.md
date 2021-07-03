---
title: Aprendizaje automático para asistencia al diagnóstico de enfermedades visuales basado en imágenes de fondo de ojo
description: Tesis doctoral de José Ignacio Orlando, dirigida por el Dr. Matthew Blaschko y la Dra. Mariana del Fresno
header-img: images/tesis-grado/2017-orlando.png
categories: tesis-doctorado
---
*Podés acceder al documento de la tesis [desde este link](https://www.ridaa.unicen.edu.ar/xmlui/bitstream/handle/123456789/1476/Orlando%2c%20Jos%c3%a9%20Ignacio.PDF?sequence=1&isAllowed=y).*


<div class="image-post-container">
    <img src="/images/tesis-grado/2017-orlando.png"/>
</div>

# Resumen

Las fotografías de fondo de ojo representan una técnica no-invasiva muy empleada por oftalmólogos para detectar retinopatía diabética (RD) y glaucoma, dos de las principales causas mundiales de ceguera prevenible. En esta tesis se presentan algunas contribuciones al análisis automático de estas imágenes mediante técnicas de aprendizaje automático. Inicialmente se propone un método de segmentación de vasos sanguíneos basado en el aprendizaje de campos condicionales aleatorios totalmente conectados mediante máquinas de vectores de soporte de salida estructurada. Este enfoque permite obtener representaciones precisas del árbol vascular, que son luego utilizadas en el contexto de dos técnicas para la detección de glaucoma y RD. Para detectar glaucoma, se plantea transferir redes neuronales convolucionales (CNNs) preentrenadas con datos no médicos. Las imágenes son adaptadas inicialmente mediante métodos de preprocesamiento tradicionales, y los descriptores extraídos se utilizan para entrenar modelos regularizados de regresión logística, obteniendo resultados competitivos con el estado del arte. Finalmente, se introduce una técnica para detectar lesiones rojas típicas de la RD basada en hibridar descriptores aprendidos utilizando una CNN y otros diseñados manualmente. Posteriormente se utiliza un Bosque Aleatorio entrenado con estos valores para identi ficar lesiones candidatas, con alta e ficacia en diversas bases de datos.

# Abstract

Fundus images are a non-invasive imaging modality that is typically used by ophthalmologists to assess the retina. They are widely applied for detecting diabetic retinopathy (DR) and glaucoma, which are leading causes of preventable blindness in the world. In this thesis we contribute with novel tools for automated fundus image analysis based on machine learning. First, we propose a vessel segmentation method based on learning fully connected conditional random elds using structured output support vector machines. This approach allows to recover accurate segmentations of the retinal vasculature that are afterwards applied in the context of two deep learning based techniques for glaucoma and DR detection. For automated glaucoma assessment, we propose to transfer convolutional neural networks (CNNs) that were pre-trained using non-medical data. Images are adapted using state of the art preprocessing methods before feeding the CNNs, and the extracted features are used to train regularized logistic regression classi ers, achieving results that are competitive with other methods. For DR screening, we introduce a red lesion detection approach based on hybridizing deep learned and hand crafted features. A Random Forest classifier is trained on these features to identify true lesion candidates, reporting state of the art performance in benchmark data sets.