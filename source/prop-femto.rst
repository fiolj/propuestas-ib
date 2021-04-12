*********************************************************************************
Implementación de la resolución numérica de la traza FROG de un pulso ultracorto.
*********************************************************************************

:Director: Dr. Juan Fiol
:Co-Director: Dr. Pablo Knoblauch
:Lugar: Subgerencia Aplicaciones de la Tecnología Láser de la Gerencia Proyecto LASIE - CAB
:Fecha: |today|

Motivación
==========

En el proyecto LASIE, los experimentos de separación isotópica involucran la generación de haces pulsados de clústeres o agregados de átomos o moléculas. Para estudiar la estabilidad y/o vida media de estos agregados, se pueden utilizar pulsos ultracortos que excitan y luego ionizan estos compuestos y se detectan con un espectrómetro por tiempo de vuelo. Asimismo, los pulsos ultracortos se pueden utilizar para determinar la estructura y evolución del haz pulsado molecular para el diseño de orificios o toberas.

Cuando se trabaja con pulsos de anchos temporales del orden de los nanosegundos o mayores, se utilizan fotodiodos cuya respuesta temporal es del orden de los picosegundos. Con este tipo de instrumentos es posible obtener resultados inmediatos y con muy buena resolución temporal. En cambio, cuando se trata de pulsos del orden de los picosegundos o femtosegundos, no es posible aplicar esta metodología. Es por eso que se aplican otras técnicas que además de proveer información sobre el ancho temporal, permiten determinar la fase de las diferentes componentes en longitudes de onda que forman el pulso.

Una de las metodologías que se utiliza para medir pulsos ultracortos se denomina FROG (Frequency-Resolved Optical Gating). La técnica consiste en generar, a partir del pulso a medir, dos pulsos, uno retrasado con respecto al otro, que se solapan espacial y temporalmente en un cristal no lineal. Si, además, los dos pulsos inciden en el cristal con las energías y ángulos adecuados, se generan procesos no lineales que son detectados con un espectrómetro, generando lo que se denomina un espectrograma.
El espectrograma es una medición de la intensidad de radiación detectada para cada valor del tiempo de retraso y para cada valor de la longitud de onda.
A partir de la medición del espectrograma, que se obtiene registrando el espectro en función del retraso entre los dos pulsos que inciden en el cristal, se puede obtener el ancho temporal y la fase del pulso.


Objetivos Proyecto Integrador
=============================

El objetivo de esta propuesta es el desarrollo de un algoritmo y sistema automático de caracterización temporal y de frecuencias de pulsos ultracortos de radiación láser.

El espectrograma de un pulso contiene información sobre su ancho temporal y sobre su fase. Para extraer esta información, se debe aplicar un algoritmo que va probando y comparando el espectrograma de un pulso de prueba con el que se obtiene experimentalmente. Según la estrategia de resolución del algoritmo que se implemente, la convergencia, estabilidad y otros factores de la solución que se obtenga, permitirán evaluar y caracterizar el pulso que se estudia.

Además de la implementación numérica, se probará y validará el código con resultados experimentales, realizando mediciones y posterior análisis de los datos obtenidos.


Cronograma
==========

1er cuatrimestre:

* Revisión y aprendizaje de métodos y herramientas teóricas, numéricas y computacionalmente relacionadas con el problema.

* Estudio teórico de los espectrogramas y los fundamentos del método de inversión de la señal.

* Implementación de un métodos computacional de análisis:
  
  - generación de pulsos 'teóricos' o de 'prueba'.
  - verificación de funcionamiento del código.

* Mediciones de espectros de autocorrelación de intensidad.


2do cuatrimestre:

* Implementación y validación de códigos de cálculo

  - estudio de la convergencia y estabilidad del sistema de resolución.
  - resolución de los espectrogramas con la incorporación de 'ruido'.
  - comparación con otros códigos de resolución numérica.

* Mediciones y validación del código

  - mediciones de espectrogramas mediante FROG.
  - análisis y procesamiento de los datos registrados.
  - caracterización de los pulsos láseres ultracortos utilizando el código numérico implementado.

* Documentación del trabajo.

Plan de Formación
=================

Se sugiere el cursado de una materia en el área de Métodos numéricos y computacionales, dependiendo de la oferta de materias disponibles

---------
