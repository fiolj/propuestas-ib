########################################################################################
Modelado de haces atómicos en procesos de enriquecimiento isotópico asistido por láseres
########################################################################################

:Director: Dr. Juan Fiol
:Lugar: Subgerencia Aplicaciones de la Tecnología Láser de la Gerencia Proyecto LASIE - CAB
:Fecha: |today|

**********
Motivación
**********

Los materiales enriquecidos isotópicamente cumplen un importante papel en cientos de aplicaciones, en áreas tan diversas como tecnología nuclear, medicina, arqueología, ciencias del clima, y en distintas ramas de la industria (ver por ejemplo [wna-uses-isotopes]_).
En general, los distintos isótopos de un átomo tienen propiedades químicas similares, pero características propias de cada isótopo como su estabilidad en el caso de isótopos radiactivos (y correspondiente vida media) o el *spin* nuclear, que dan lugar a comportamientos diferentes que pueden aprovecharse para desarrollar aplicaciones específicas.
Por ejemplo, el litio es uno de los átomos más simples y tiene sólo dos isótopos estables |7Li| y |6Li| con poblaciones naturales de 92,58% y 7,42%, respectivamente. Mientras sus propiedades químicas difieren levemente, las secciones eficaces de captura neutrónica de |6Li| es relativamente alta, alrededor de 20000 veces mayor que la de |7Li|, por lo que es especialmente adecuado para la construcción de detectores de neutrones por centelleo. En este tipo de aplicaciones, el enriquecimiento del material produce un valor agregado en factores que pueden llegar a más de 10000.

Tanto en el caso de litio como en muchos elementos isotópicamente enriquecidos que se utilizan para medicina nuclear, las cantidades requeridas son modestas, en el rango de algunos gramos a unos pocos kilogramos por año, y con un alto grado de enriquecimiento. En estas condiciones se considera que los métodos de separación isotópica mediante ionización selectiva por láseres es altamente apropiada, ya que tienen una alta eficiencia de separación (ver por ejemplo la discusión sobre litio en [wna-sep-litio]_)

El método de separación isotópica de átomos asistida por láseres está basado en la excitación e ionización selectiva mediante láseres con longitudes de onda en la zona del espectro visible e infrarrojo.
Los iones generados, isotópicamente seleccionados, se extraen para su análisis y acumulación mediante campos electromagnéticos. 

Brevemente, el método consta de tres etapas diferenciadas:

Generación del haz atómico:
    Se genera un haz **colimado** de átomos neutros mediante evaporación a temperaturas mayores que las correspondientesa al punto de fusión del material.

Ionización selectiva:
    Los átomos del haz se excitan mediante su irradiación con un láser sintonizable a la longitud de onda de absorción del isótopo de interés.  Esta transición se produce por interacción con un único fotón por lo que se necesita una fluencia moderada, pero es fundamental que el ancho de línea del láser sea muy pequeño para poder excitar sólo el isótopo seleccionado. Posteriormente los átomos excitados se ionizan mediante la aplicación adicional de uno o dos pulsos de láser adicionales.


Diagnóstico y separación:
    La separación de los iones para su acumulación se produce mediante un la aplicación de campos electromagnéticos, en su versión más simple se utiliza un par de placas cargadas. La caracterización del haz atómico y las mediciones de grado de selectividad isotópica y eficiencia de ionización se realizan utilizando un espectrómetro de masas por tiempo de vuelo, diseñado y construido *ad-hoc* para su uso dentro de la cámara de reacción.


*********************
Propuesta y Objetivos
*********************

La presente propuesta se enmarca dentro del proyecto de desarrollo de métodos de separación isotópica asistida por láseres del Proyecto LASIE. Estos experimentos están dirigidos al desarrollo de procesos de enriquecimiento isotópico de litio y otros materiales de interés mediante ionización selectiva.

Se propone investigar en forma teórica, tanto en forma analítica como numérica, y mediante simulaciones computacionales, la generación del haz de átomos neutros. Se estudiará en primer lugar el sistema de generación de haz atómico más simple, correspondiente a un evaporador por temperatura con distintas configuraciones. Además, se propondrán y estudiarán fuentes de átomos alternativas con flujo de gases que permiten aumentar la densidad en varios órdenes de magnitud. El objetivo del trabajo es comprender el proceso y obtener configuraciones optimizadas para su aplicación en sistemas de separación isotópica en desarrollo en el laboratorio. 

**********
Cronograma
**********

1er cuatrimestre:
     - Estudio de los modelos a utilizar, resultados utilizando cálculos analíticos.

     - Análisis y determinación de la geometría y gas de interés a utilizar para el modelado.

2do cuatrimestre:
    - Implementación del sistema elegido en los códigos de cálculo numérico correspondientes para su simulación.

      En esta etapa el estudiante conocerá el funcionamiento básico de los códigos a utilizar y realizará los cálculos para distintas configuraciones.

    - Evaluación cuantitativa de parámetros relevantes del proceso. Documentación del trabajo.

      En esta etapa se espera que el estudiante analice los datos producidos por ambos códigos. Estos resultados permitirán identificar los parámetros de la geometría y condiciones macroscópicas relevantes para optimizar el proceso.



***********
Referencias
***********

.. [wna-uses-isotopes] **The Many Uses of Nuclear Technology** en world-nuclear.org: https://world-nuclear.org/information-library/non-power-nuclear-applications/overview/the-many-uses-of-nuclear-technology.aspx

.. [wna-sep-litio] **Lithium** en world-nuclear.org: https://world-nuclear.org/information-library/current-and-future-generation/lithium.aspx

.. |7Li| replace:: :sup:`7`\ Li
.. |6Li| replace:: :sup:`6`\ Li

		   
