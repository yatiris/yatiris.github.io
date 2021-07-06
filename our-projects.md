---
title: Our projects
permalink: /our-projects/
---


![](/images/others/whiteboard.jpg)


{% assign reference_types = "projects-english|projects-spanish" | split: "|" %}
{% assign sorted_list_of_posts = site.posts | sort: 'date' %}

{% for type in reference_types %}

{% if type == "projects-english" %}

### **Research projects**
Take a quick look at the projects and initiatives we are working on:

{% endif %}

<div class="content list">
  {% for post in sorted_list_of_posts %}
    {% if post.categories contains type %}
    <div class="list-item">
      <p class="list-post-title">
        <a href="{{ site.baseurl }}{{ post.url }}">- {{ post.title }}</a>
      </p>
    </div>
    {% endif %}
  {% endfor %}
</div>

{% endfor %}

<br>

### Funding

Here you can find the list of grants we got to fund our research.

**(2021-2023)** <br>
_CANOA: CAracterización morfológica de la cabeza del Nervio Óptico en fotografías de fondo de ojo mediante Aprendizaje profundo._<br>
(CANOA: Morphological characterization of the optic nerve head in color fundus photographs using deep learning.)<br>
PICT-2019-00070. FONCyT. Agencia Nacional de Promoción Científica y Tecnológica (ANPCyT). AR$ 475.000. 
Principal Investigator: José Ignacio Orlando.

**(2021)** <br>
_retinar: assisting remote diabetic retinopathy screening with AI tools._<br>
(Weakly-supervised Abdominal Ultrasound Segmentation using Simulated Scans and Cycle-Consistency based Generative Models.)<br>
NVIDIA Applied Research Accelerator Program. NVIDIA Corporation. 500 hours of cloud computing in V100 GPUs using SaturnCloud.<br>
Researcher awarded: José Ignacio Orlando.

_Hacia una plataforma inteligente para el tamizado remoto de la retinopatía diabética: control de calidad de fotografías de fondo de ojo utilizando autocodificadores._<br>
(Towards a smart platform for diabetic retinopathy screening: automated quality control of color fundus photographs using autoencoders) <br>
03-JOVIN-37c. Secretaría de Ciencia, Arte y Tecnología, Universidad Nacional del Centro de la Provincia de Buenos Aires (UNICEN). AR$ 100.000.
Principal Investigator: José Ignacio Orlando.

**(2020)** <br>
_Segmentación de Ultrasonido Abdominal Debilmente Supervisada utilizando Imágenes Simuladas y Modelos Generativos con Consistencia Cíclica._<br>
(Weakly-supervised Abdominal Ultrasound Segmentation using Simulated Scans and Cycle-Consistency based Generative Models.)<br>
[Kaggle Open Data Research Grant.](https://www.kaggle.com/open-data-research-grant-2020-awardees#project-title-12) Google Kaggle. U$S 2.000.
Researchers awarded: José Ignacio Orlando, Santiago Vitale, Emmanuel Iarussi, Alejandro Díaz, Ignacio Larrabide.

**(2020-2022)** <br>
_Modelado computacional de la circulación coronaria._<br>
(Computational modelling of coronary circulation)<br>
PICT-2018-2427. FONCyT. Agencia Nacional de Promoción Científica y Tecnológica (ANPCyT). AR$ 339.600. 
Principal Investigator: Carlos Bulant.

**(2019-2021)** <br>
_Modelado, simulación y optimización para aplicaciones computacionales de análisis y visualización de señales e imágenes._<br>
(Modelization, simulation and optimization for computational application in signal and image analysis and visualization)
Proyecto de Incentivos. Secretaría de Políticas Universitarias (SPU), Ministerio de Educación de la Nación.
Principal Investigator: Mariana del Fresno.

**(2018-2020)** <br>
_HI-MED - Herramientas Informáticas aplicadas a la cuanticación de imagen, simulación y planicación del tratamiento en MEDicina._<br>
(Computational tools applied to medical image quantification, simulation and treatment planning)<br>
PICT 2016-0116. FONCyT. Agencia Nacional de Promoción Científica y Tecnológica (ANPCyT). AR$ 339.600. 
Principal Investigator: Ignacio Larrabide.

**(2015-2017)** <br>
_MISEV: Modelos de Imagen y Simulación para el diagnóstico y tratamiento de enfermedades vasculares._<br>
(Image based and simulation models for computer-assisted diagnosis and treatment of vascular diseases)<br>
PICT 2015-1730. FONCyT. Agencia Nacional de Promoción Científica y Tecnológica (ANPCyT). AR$ 339.600. 
Principal Investigator: Ignacio Larrabide.

**(2015-2017)** <br>
_MAD - Modelos para el planeamiento del tratamiento de Aneurismas Intracraneales con Desviadores de Flujo._<br>
(Models for Intracraneal Aneurysms treatment planning with flow diverters)<br>
PICT Startup 2015-0006. FONCyT. Agencia Nacional de Promoción Científica y Tecnológica (ANPCyT). AR$ 1.164.000. 
Principal Investigator: Ignacio Larrabide.

**(2015-2017)** <br>
_Desarrollo de Modelos y Aplicaciones de Simulación, Optimización, Computación Gráfica y procesamiento de imágenes._<br>
(Development of Models and Applications for automated simulation, optimization, computer graphics and image processing)<br>
Programa de Incentivos. Ministerio de Educación de la Nación.
Principal Investigator: Marcelo Vénere.

**(2014-2015)** <br>
_SIMECO: Desarrollo de un simulador de ecografía para entrenamiento._<br>
(Development of an ultrasound simulator for training)<br>
SPU 0049/2014, Expediente 1-51977/2014. Secretaría de Políticas Universitarias, Ministerio de Educación de la Nación. AR$ 799.000.
Principal Investigator: Ignacio Larrabide.

**(2014-2015)** <br>
_FDF-Movil - Desarrollo de una plataforma móvil para la planificación de intervenciones_<br>
(Development of a mobile platform for intervention planning)<br>
IBEROEKA, S.D.C. S.R.L., Galgo Medical S. L.
Principal Investigator: Ignacio Larrabide.

**NVIDIA Hardware Grants**<br>
We have received six NVIDIA Hardware Grants since the creation of the program by NVIDIA Corporation, granted to Carlos Bulant, Ignacio Larrabide, Gustavo Boroni and Mariana del Fresno.