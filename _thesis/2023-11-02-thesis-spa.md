---
title: Modelos generativos de aprendizaje antagónico desapareado para la simulación realista de ecografías abdominales
description: Tesis doctoral de Santiago Vitale, dirigida por el Dr. Ignacio Larrabide y José Ignacio Orlando
header-img: images/tesis-grado/2023-vitale.png
categories: tesis-doctorado
---
*Podés acceder al documento de la tesis [desde este link](https://www.ridaa.unicen.edu.ar/bitstreams/5051f0ff-91fe-4b71-80f7-97e023d7f4fa/download).*


<div class="image-post-container">
    <img src="/images/tesis-grado/2023-vitale.png"/>
</div>

### Resumen

Ultrasound is a non-invasive, cost-effective, and radiation-free medical imaging technique commonly used in emergentology, for guiding invasive procedures, and for medical diagnosis. However, the quality of the images heavily depends on the operator's experience. Although simulators have been shown to be as effective as real ultrasound machines for physician training, existing approaches for simulating the interaction of ultrasound waves with the human body require complex and expensive computational models, limiting their ability to accurately reproduce specific tissues. This thesis presents a series of contributions to realistic abdominal ultrasound simulation based on the application of deep learning generative models on images simulated using physical models. Specifically, it builds on top of an existing simulator developed by our research group, which uses ray-casting algorithms to produce synthetic ultrasound studies of the abdomen. To improve its realism, we apply generative adversarial networks with cycle consistency losses, trained from an unpaired set of synthetic and real ultrasound images. Furthermore, to achieve a more robust model and a higher level of realism, a novel cycle consistency term is introduced, conditioned by a pre-trained segmenter that produces labels of the main abdominal organs and penalizes anatomical differences caused by unexpected hallucinations.
The final result of this thesis is a hybrid simulator based on both the physical modeling of ultrasound waves and deep learning generative models. It is capable of synthesizing realistic ultrasound scans of healthy subjects with representations of multiple abdominal organs from any computed tomography as input.

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=0zBJg-_7fCs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
