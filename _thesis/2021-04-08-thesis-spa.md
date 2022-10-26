---
title: Simulación de cámaras estereoscópicas utilizando redes neuronales
description: Tesis de grado de Rodrigo Cobo, dirigida por el Dr. José Ignacio Orlando y el Dr. Ignacio Larrabide.
header-img: images/tesis-grado/2021-cobo.png
categories: tesis-grado
---

<div class="image-post-container">
    <img src="/images/tesis-grado/2021-cobo.png"/>
</div>

Las cámaras estereoscópicas son dispositivos que poseen múltiples lentes y, de esta forma, capturan en el mismo instante un conjunto de fotografías en paralelo. Usualmente, dichos modelos de cámaras se utilizan para la generación de un efecto animado llamado \emph{wigglegram}. Los wigglegrams son imágenes animadas estereoscópicas 3D en las que un objeto de interés se mantiene fijo y todos los objetos en segundo plano se alteran de manera coherente con su ubicación en el entorno 3D. 

En este trabajo se propone facilitar al usuario la creación de wigglegrams, de forma tal de no requerir hardware adicional, y en consecuencia reducir los costos asociados a la producción. En particular, se utilizaron algoritmos de aprendizaje profundo basados en redes generativas adversarias (GANs) que permitieron, a partir de una imágenes de entrada, producir una imagen similar a la que se obtendría desde otro ángulo. Así, repitiendo la utilización de la red para varias vistas sucesivamente, se buscó reproducir un efecto equivalente al obtenido utilizando cámaras estereoscópicas. Los modelos propuestos se entrenaron en base a un \emph{dataset} creado exclusivamente para este trabajo, formado por imágenes multivistas obtenidas por cámaras estereoscópicas en la producción de películas 3D. Durante el trabajo además, se evaluaron diferentes arquitecturas de redes para identificar cuál obtuvo los mejores resultados.

<iframe width="560" height="315" src="https://www.youtube.com/embed/K8w2wHLjH_s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>