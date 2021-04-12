##########################################################################################
Automatización y caracterización de un dispositivo para enriquecimiento isotópico de litio
##########################################################################################

*******
Resumen
*******

   El presente plan de trabajo se enmarca dentro del proyecto de separación isotópica de litio asistida por láseres, que resulta de una colaboración entre la Subgerencia Aplicaciones de la Tecnología Láser de la Gerencia Proyecto LASIE y el Laboratorio de Fotónica y Optoelectrónica de la Gerencia de Física del Centro Atómico Bariloche. El plan de trabajo integra todas las etapas necesarias para el desarrollo de un método de separación isotópica de litio, con una fuerte interacción entre los aspectos teóricos y experimentales.


********
Objetivo
********

El proyecto propuesto se divide en dos objetivos. El primero de ellos es la caracterización mediante simulaciones numéricas de un evaporador de litio. El segundo objetivo consiste en la implementación del sistema de control, monitoreo y adquisición del dispositivo para enriquecimiento isotópico de litio.

************
Introducción
************

El litio se ha vuelto un recurso muy valioso a nivel mundial, principalmente debido a su uso casi universal en baterías de dispositivos electrónicos. En la actualidad, los mayores esfuerzos se enfocan en fabricar automotores eléctricos que utilicen una tecnología similar.

Argentina posee casi un tercio de las reservas de litio de Sudamérica que, junto a las de Chile y Bolivia, representan más de la mitad de la disponibilidad mundial de litio. En los salares de la Puna se produce carbonato de litio (|Li2CO3|) de grado batería que se exporta a un precio aproximado de 13 US$/kg, de lo cual solo una pequeña fracción queda en Argentina en concepto de regalías (3%) y de las ganancias declaradas de las empresas. 

Este proyecto tiene como objetivo principal agregar valor al sistema de procesamiento  de litio en Argentina a través de la producción de litio enriquecido isotópicamente (el litio natural contiene 92,58% de |7Li| y 7,42% de |6Li|), que es usado en diversas aplicaciones relacionadas a la tecnología nuclear. En este campo, el litio o las sales de litio se emplean en cantidades insignificantes cuando se las compara con su uso en baterías, como componentes de grasas lubricantes o en refrigeración. Sin embargo, el valor estratégico de los materiales en base a litio usados en el sector nuclear hace que tengan un enorme valor agregado.  


El litio en el área nuclear
===========================

El litio es un elemento estratégico en la tecnología nuclear ya que enriquecido en |7Li| se utiliza para controlar la química del circuito primario en centrales nucleares del tipo de agua presurizada, como Atucha I y II y Embalse, que generan el 5,6% de la energía total consumida en el país (136.505 GWh en 2016). Asimismo, este isótopo se lo empleará en las centrales de sal fundida de cuarta generación. Por otra parte, el |6Li| se utilizará como blindaje y detector de neutrones en facilidades como el Laboratorio Argentino de Haces de Neutrones (LAHN), cuya operación en el reactor RA10 se prevé en un futuro próximo. Las próximas generaciones posiblemente verán el uso del litio en reactores de fusión. Estas aplicaciones constituyen una posible futura demanda de sales de litio con un altísimo valor agregado [Corti17]_

Adicionalmente, el litio ha tomado un rol muy importante en la detección de neutrones mediante sensores de centelleo. Trabajos recientes muestran que el |6Li|, debido a su alta sección eficaz, presenta ventajas respecto a otros materiales. Recientemente se ha demostrado el uso de polímeros cargados con |6Li|\ F como detectores de neutrones térmicos con alta eficiencia y discriminación de rayos gamma [Sen12]_\ [Miller14]_, o el uso de polímeros litiados de poliestireno copolimerizado y centelladores orgánicos basados en salicilato de |6Li| [Mabe14]_\ [Mabe16]_.

.. |7Li| replace:: :sup:`7`\ Li
.. |6Li| replace:: :sup:`6`\ Li
.. |Li2CO3| replace:: Li\ :sub:`2`\ CO\ :sub:`3`
.. |LiPF6| replace:: LiPF\ :sub:`6`


Enriquecimiento de Litio
========================

El uso de litio isotópicamente enriquecido en cualquiera de sus dos componentes es un recurso estratégico de gran valor agregado tanto para áreas industriales como en el área nuclear.

A mediados del siglo pasado se desarrolló el método de separación isotópica basada en el fraccionamiento de |7Li|\ /\ |6Li| en mercurio usando columnas de intercambio (COLEX) o intercambio electroquímico (ELEX). Sin embargo, estas técnicas producen una gran cantidad de residuos de mercurio. El gran impacto sobre el medio ambiente hace que estas técnicas estén prohibidas en países como EEUU y sólo se empleen en Rusia y China, que son los principales proveedores a nivel mundial. En este proyecto se propone desarrollar la tecnología de separación isotópica de litio mediante métodos ambientalmente más benignos.


***************
Plan de trabajo
***************

Este plan de trabajo se enmarca dentro del proyecto de desarrollo de un método de separación isotópica de litio asistida por láseres que se está desarrollando actualmente en el CAB. Estos experimentos están dirigidos a demostrar la factibilidad  del proceso de enriquecimiento isotópico de litio mediante la técnica AVLIS (Atomic Vapor Laser Isotope Separation).
 

Descripción del método
======================

El método AVLIS de separación está basado en la excitación e ionización isotópicamente selectiva de átomos de litio mediante láseres con longitudes de onda en la zona del espectro visible e infrarrojo. Los iones generados, isotópicamente seleccionados, se extraen para su análisis y acumulación mediante campos electromagnéticos. 

Brevemente, el método consta de tres etapas diferenciadas:

Generación del haz atómico:
    Se genera un haz **colimado** de átomos neutros mediante la evaporación de litio en un horno a temperaturas entre 300 y 800 grados centígrados. 

Ionización selectiva:
    Los átomos del haz se excitan mediante su irradiación con un láser continuo sintonizable  que opera en el rango 670.77 nm a 670.81 nm, lo que permite excitar selectivamente a cada isótopo desde el estado fundamental al estado 1s\ :sup:`2`\ 2p.  Esta transición se produce por interacción con un único fotón por lo que se necesita una fluencia moderada, pero es fundamental que el ancho de línea del láser sea inferior a 1 pm para poder excitar selectivamente uno de los isótopos. Posteriormente los átomos excitados se ionizan mediante la aplicación adicional de uno o dos pulsos de láser.


Diagnóstico y separación:
    La separación de los iones para su acumulación se produce mediante un sistema simple de placas cargadas. La caracterización del haz atómico y las mediciones de grado de selectividad isotópica y eficiencia de ionización se realizan utilizando un espectrómetro de masas por tiempo de vuelo, diseñado y construido *ad-hoc* para su uso dentro de la cámara de reacción.


Propuesta de trabajo
====================

Se propone que el estudiante se involucre en la caracterización teórico-numérica del evaporador de litio y en el diseño e implementación de un sistema de control y automatización del dispositivo para enriquecimiento isotópico.

Proyecto Integrador
-------------------

En una primera etapa el estudiante realizará simulaciones y cálculos sencillos del horno de evaporación y el haz atómico generado. El objetivo de esta etapa es el desarrollo de un método teórico-numérico para caracterizar el haz y de predicción de su eficiencia. Con esta herramienta se realizarán estudios de diseño óptimo para los experimentos preliminares de separación isotópica y para su extensión a planta piloto en una posterior etapa de escalado.

Adicionalmente, el estudiante realizará un estudio teórico del sistema de diagnóstico basado en espectroscopía por tiempos de vuelo, investigando la dependencia de la resolución y eficiencia de detección del sistema en función de la configuración de campos eléctricos.

En una segunda etapa, se encarará el diseño y la implementación de un sistema de control y monitoreo del equipo. Para ello, se estudiará cómo controlar y configurar las fuentes de tensión, y la medición de temperatura y presión. Adicionalmente, se incorporará el registro y procesamiento de las señales obtenidas con el mini-TOF utilizando un osciloscopio.
  
Seguidamente, y en concordancia con los tiempos de construcción y puesta en marcha del dispositivo experimental, el estudiante participará de los experimentos de generación del haz atómico y del diagnóstico mediante espectroscopía por tiempo de vuelo.

Los resultados de estas mediciones se contrastarán con los cálculos y simulaciones realizadas previamente.


Cronograma
----------

1er cuatrimestre:

        Estudio del problema de flujo de átomos en el horno de evaporación y de los modelos a utilizar.

        Análisis y determinación de la geometría del horno. Inicio de la implementación para el modelado teórico.

	Implementación de los códigos de cálculo y análisis de los resultados para los diseños existentes.

        Evaluación cuantitativa de parámetros relevantes del proceso. Estudio de diseños alternativos.

2do cuatrimestre:

	Diseño conceptual del sistema de control. Determinación de los parámetros a controlar de los instrumentos.

	Poner en funcionamiento y caracterizar el sistema de control y monitoreo.

	Implementación del registro y procesamiento de señales registradas con el osciloscopio.

        Participación de la implementación experimental en el dispositivo para separación isotópica. 

        Documentación del trabajo.


***********
Referencias
***********
                     
.. [Corti17] **Litio y tecnología nuclear.** H. R. Corti. *Litio: un recurso natural estratégico desde los depósitos minerales a las aplicaciones tecnológicas.* Ed. E. Baran. Academia Nacional de Ciencias Exactas, Físicas y Naturales y Academia Nacional de Ingeniería, Publicaciones Científicas No 12, pag. 185-198 (2017).

.. [Sen12] I. Sen, M. Urffer, D. Penumadu, S. A. Young, L. F. Miller, A. N. Mabe. IEEE Trans. Nuclear Sci. 59, 1781 (2012).

.. [Miller14] L. F. Miller, M. J. Urffer, A. N. Mabe, R. Uppal, D. Penumadu, G. Schweitzer. IEEE Trans. Nuclear Sci. 61, 1381 (2014).

.. [Mabe14] A. N. Mabe, M. J. Urffer, D. Penumadu, G. F. Schweitzer. Radiation Measurement 66, 5 (2014).

.. [Mabe16] A. N. Mabe, A. M. Glenn, M. L. Carman, N. P. Zaitseva. Nucl. Instr. Method Phys. Res. A 806, 80 ( 2016).

