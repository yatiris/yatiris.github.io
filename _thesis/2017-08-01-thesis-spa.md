---
title: Desarrollo de herramientas de procesamiento de imágenes para simulación de ultrasonido
description: Tesis de grado de Hernán Claudio Külsgaard, dirigida por el Dr. Ignacio Larrabide y el Ing. Pablo Andrés Rubí
header-img: images/tesis-grado/2017-kulsgaard.png
categories: tesis-grado
---

*Podés acceder al documento de la tesis [desde este link](https://www.ridaa.unicen.edu.ar/items/32194aa7-d2ae-4348-aab5-9ed4d6d40c4e).*

<div class="image-post-container">
    <img src="/images/tesis-grado/2017-kulsgaard.png"/>
</div>

### Resumen

El trabajo se divide en dos partes. En la primera el objetivo es construir una herramienta para la creación de filtros de pre-procesamiento que se pueda complementar con el software de visualización 3D ParaView. Actualmente esta tarea se puede realizar dentro de ParaView pero no cuenta con la capacidad de modificar parámetros de los filtros desde la interfaz gráfica, por lo que se deben recurrir directamente al código fuente de éste. Por lo tanto la característica principal que debe tener la herramienta es poder asignarle a los filtros distintos tipos de parámetros modificables. Luego se estudiarán filtros necesarios para el pre-procesamiento en simulador de ultrasonido SIMECO y se crearán utilizando la herramienta. Se describirán los pasos
realizados y los parámetros configurables seleccionados para cada uno. Por otro lado, existe un filtro correspondiente a la recreación de ruido speckle que posee problemas de rendimiento. Como objetivo secundario se propone buscar una implementación alternativa que pueda obtener el mismo resultado pero en una franja de tiempo menor. Se analizarán los resultados comparando el tiempo de procesamiento de cada uno. El segundo objetivo es estudiar e implementar un algoritmo de recreación de ruido speckle dentro de SIMECO que se ejecute en tiempo real. Simular este ruido es computacionalmente muy costoso. Por esta razón simuladores actuales como SIMECO, optan por realizar la recreación en forma de pre-procesamiento a costa de perder realismo en la simulación. Ya que el proceso deberá ser ejecutado en tiempo real, se hará hincapié en el rendimiento del algoritmo. Finalmente se comparará y se analizarán la performance y los resultado con la versión original.