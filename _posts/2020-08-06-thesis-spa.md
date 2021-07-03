---
title: Modificación de sistema de física en la simulación de imágenes de ultrasonido en tiempo real
description: Tesis de grado de Tomás Pérez Cambet, dirigida por el Dr. Ignacio Larrabide y el Ing. Santiago Vitale
header-img: images/tesis-grado/2020-cambet.png
categories: tesis-grado
---
*Podés acceder al documento de la tesis [desde este link](https://www.ridaa.unicen.edu.ar/xmlui/bitstream/handle/123456789/2369/Trabajo%20Final%20-%20Tomas%20Perez%20Cambet.pdf?sequence=1&isAllowed=y).*


<div class="image-post-container">
    <img src="/images/tesis-grado/2020-cambet.png"/>
</div>

El objetivo principal de este trabajo es mejorar la performance de trazado de rayos del simulador de ecografías SIMECO. Se logró la incorporación de mejoras importantes al sistema. Los tiempos de ejecución del trazado de rayos se vieron beneficiados por una implementación que aprovecha los recursos provistos por la placa de video instalada en la computadora. Esto trajo consigo una mejora de dichos tiempos de un 600 % e incrementos en la cantidad de rayos trazados por segundo del orden del 200 %. Esto representa, en el pipeline de simulación en su totalidad, la reducción de los tiempos de generación de una imagen a la mitad. Asimismo, se incorporó el uso de simulación Monte-Carlo, proceso que permite incorporar varias mejoras en el modelado de características como la rugosidad de un material, o la penetración de un rayo. Esto también da lugar para la implementación de otros fenómenos, tales como la simulación del grosor de rayo mediante perturbaciones al punto de origen del rayo. Por último, esto fue realizado no solo evitando la perdida de calidad de la imagen generada, sino que también son mejorados ciertos aspectos como la detección de vasos internos de distintos órganos, así como el brillo generado por las distintas interfaces entre órganos.

*Podés ver el video de la defensa de la tesis acá:*

<iframe width="560" height="315" src="https://www.youtube.com/embed/HOsU6TzFVo8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>