=========================
 Proyecto Maestría: FROG
=========================
Implementación de la resolución numérica de la traza FROG de un pulso ultracorto.
=================================================================================

Resumen
=======

El presente plan de trabajo propone realizar la implementación de un sistema de resolución de espectrogramas para pulsos láser ultracortos, del orden de cientos de fentosegundos.

Objetivo
========

El objetivo del presente plan de trabajo es investigar métodos, y realizar la implementación y optimización de la resolución numérica del método FROG (Frequency-Resolved Optical Gating) para la medición de pulsos láseres ultracortos en la escala de los femtosegundos.



Introducción
============

La invención de los láseres en la década del 60 del siglo pasado, abrió un amplio espectro de descubrimientos científicos y desarrollos tecnológicos que impactaron en la vida cotidiana. Con el paso de los años, los avances tecnológicos aplicados a los láseres permitieron aumentar su energía o su ancho temporal, entre otros.

Asimismo, el desarrollo de láseres de pulsos ultracortos (menores al picosegundo), abrieron un amplio campo de estudio en diferentes disciplinas. En el área de la biología y la química, fenómenos como fotosíntesis y vibraciones moleculares, entre otros, ocurren en escalas de los femtosegundos. En el ámbito de la física, tiempos de vida media de estados excitados, fotoionización y otros fenómenos, ocurren en escalas ultrarrápidas.[Trebino2000]_

Para estudiar estos sistemas, es necesario conocer el ancho temporal del pulso del láser para asegurarse que es más corto que el fenómeno que se quiere medir. Por otro lado, para ciertos experimentos, como por ejemplo el estudio de las vibraciones moleculares, es conveniente caracterizar la estructura del pulso ya que determina los resultados de las mediciones. Es importante verificar cómo varía el color o la frecuencia durante el pulso, fenómeno conocido con *chirp.*\ [Trebino2000]_

En el proyecto LASIE, los experimentos de separación isotópica involucran la generación de haces pulsados de clústeres o agregados de átomos o moléculas. Para estudiar la estabilidad y/o vida media de estos agregados, se pueden utilizar pulsos ultracortos que excitan y luego ionizan estos compuestos y se detectan con un espectrómetro por tiempo de vuelo. Asimismo, los pulsos ultracortos se pueden utilizar para determinar la estructura y evolución del haz pulsado molecular para el diseño de orificios o toberas.

Cuando se trabaja con pulsos de anchos temporales del orden de los nanosegundos o mayores, se utilizan fotodiodos cuya respuesta temporal es del orden de los picosegundos. Con este tipo de instrumentos es posible obtener resultados inmediatos y con muy buena resolución temporal.

En cambio, cuando se trata de pulsos del orden de los picosegundos o femtosegundos, no es posible aplicar esta metodología. Es por eso que se aplican otras técnicas que permiten caracterizar pulsos ultracortos que además de obtener información sobre el ancho temporal, es posible determinar la fase de las diferentes componentes en longitudes de onda que forman el pulso.

Una de las metodologías que se utiliza para medir pulsos ultracortos se denomina FROG (Frequency-Resolved Optical Gating). La técnica consiste en generar, a partir del pulso a medir, dos pulsos, uno retrasado con respecto al otro, que se solapan espacial y temporalmente en un cristal no lineal. Si, además, los dos pulsos inciden en el cristal con las energías y ángulos adecuados, se generan procesos no lineales que son detectados con un espectrómetro, generando lo que se llama un espectrograma.
El espectrograma es una medición de la intensidad de radiación detectada para cada valor del tiempo de retraso y para cada valor de la longitud de onda.
A partir de la medición del espectrograma, que se obtiene registrando el espectro en función del retraso entre los dos pulsos que inciden en el cristal, se puede obtener el ancho temporal y la fase del pulso.

Entre las diversas técnicas que se utilizan se pueden mencionar GRENOUILLE que consiste en una mejora de la técnica FROG ya que no requiere la alineación de dos haces [Trebino2000]_, SPIDER (Spectral Phase Interferometry for Direct Electric-field Reconstruction), entre otras.

El espectrograma de un pulso contiene información sobre su ancho temporal y sobre su fase. Para extraer esta información, se debe aplicar un algoritmo que va probando y comparando el espectrograma de un pulso de prueba con el que se obtiene experimentalmente. Según la estrategia de resolución del algoritmo que se implemente, la convergencia, estabilidad y otros factores de la solución que se obtenga, permitirán evaluar y caracterizar el pulso que se estudia.

Desde la invención de esta técnica, se han publicado varios programas para obtener el ancho del pulso y su fase. El inventor de la técnica, R.  Trebino, ofrece en su página web un programa en Matlab con diferentes actualizaciones y mejoras. Recientemente, se publicaron diferentes códigos en Python y Matlab que ofrecen diferentes funcionalidades y que aplican diferentes formas de resolver el problema numérico [Jafari2019]_, [Geib2019]_, [Pinilla2019]_.

Plan de trabajo
===============

El plan de trabajo se divide en dos ejes.

Primer eje
----------

El primer eje consiste en introducir al estudiante en los conceptos téoricos relacionados con óptica no lineal, cómo medir pulsos ultracortos y cómo utilizar procesos lineales para obtener la autocorrelación entre dos pulsos. La autocorrelación es la forma más simple de medir un pulso ultracorto, pero con limitaciones que se discutirán con el estudiante.

Una mejora a la utilización de la autocorrelación como metodología de medición de pulsos consiste en registrar el espectrograma. Para ello se discutirán las formas de obtener un espectrograma, se introducirá el concepto de FROG y qué geometrías y procesos se emplean para obtener un espectrograma. Se discutirán los procesos no lineales que se utilizan y cómo se modelan matemáticamente.

El siguiente paso consistirá en el estudio de diferentes métodos para la resolución numérica para obtener el pulso y la fase a partir de un espectrograma.  A continuación se realizará la implementación del código para implementar el método que se considere más adecuado y se comparará con otros métodos.
Este punto se divide en varias etapas que involucran:

- generación de pulsos 'teóricos' o de 'prueba'.

- verificación de funcionamiento del código.

- estudio de la convergencia y estabilidad del sistema de resolución.

- resolución de los espectrogramas con la incorporación de 'ruido'.

- comparación con otros códigos de resolución numérica.

Segundo eje
-----------

El estudiante se involucrará en mediciones experimentales de pulsos del orden de los 150 fs. Realizará mediciones de autocorrelación y de FROG en el láser de femtosegundo disponible en el Laboratorio de Espectroscopía Ultrarrápida del proyecto LASIE.

El trabajo del estudiante comprenderá los siguientes aspectos:

- Mediciones de autocorrelación.
- Mediciones de espectrogramas mediante FROG.
- Análisis y procesamiento de los datos registrados.
- Caracterización de los pulsos láseres ultracortos utilizando el código numérico implementado.


Referencias
===========

.. [Trebino2000] R. Trebino. *Frequency-Resolved Optical Gating: The Measurement of Ultrashort Laser Pulses.* Kluwer Academic Publishers. 2000 ISBN 1-4020-7066-7

.. [Jafari2019] R. Jafari, T. Jones and R. Trebino. *100% reliable algorithm for second-harmonic-generation frequency-resolved optical gating*. Optics Express Vol. 27, Issue 3, pp. 2112-2124 (2019).

.. [Geib2019] N. C. Geib, M. Zilk, T. Pertsch and F. Eilenberger. *Common pulse retrieval algorithm: a fast and universal method to retrieve ultrashort pulses.*\ Optica Vol. 6, Issue 4, pp. 495-505 (2019)

.. [Pinilla2019] S. Pinilla, T. Bendory, Y. C. Eldar and H. Arguello, *Frequency-Resolved Optical Gating Recovery via Smoothing Gradient.* IEEE Transactions on Signal Processing, vol. 67, no. 23, pp. 6121-6132, 2019.
