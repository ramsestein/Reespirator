# Reespirator 2020

Este repositorio pretende documentar y organizar los pasos para fabricar prototipos de  **Reespirator-2020**, un respirador open-source basado en el sistema de ventilación mecánica Jackson-Rees, diseñado y mejorado a partir de los prototipos elaborados por el equipo de Reesistencia Team para todas aquellas personas, organizaciones o empresas que quieran fabricarlo en cualquier parte del mundo.  


> ESTA DOCUMENTACIÓN ESTÁ EN ELABORACIÓN, COMPRUEBE REGULARMENTE LOS CAMBIOS, LAS PRIMERAS VERSIONES PUBLICADAS ESTÁN DESACTUALIZADAS. 



## Disclaimer
*Recuerde que un respirador es un dispositivo médico que sólo puede ser utilizado por personal cualificado y que un mal respirador o un respirador mal utilizado puede matar.*

La presente documentación **NO PERMITE CONSTRUIR UN RESPIRADOR FINAL**, sólo se publica para que se pueda fabricar PROTOTIPOS para investigación. 

## Info
*¿Qué es Reespirator 2020?*

El dispositivo Reespirator 2020 es un prototipo de sistema respirador de emergencia con elementos disponibles por la mayoría de las personas en cualquier parte del mundo, de rápida construcción y con la capacidad para mantener constantes ventilatorias aceptables en un paciente afecto de [Síndrome de Distrés Respiratorio Agudo](https://es.wikipedia.org/wiki/S%C3%ADndrome_de_dificultad_respiratoria_aguda) o SDRA que esperamos puede ser aplicable a los pacientes con COVID-19.

Aunque el origen de Reespirator es España, debido a las regulaciones y validaciones necesarias para los productos médicos, y aunque Reespirator 23 de [Reesistencia Team](https://gitlab.com/reesistencia), en el que se basó inicialmente este nuevo diseño, ha superado varias pruebas preclínicas con animales, y de compatibilidad electromagnética, suponemos que este dispositivo nunca se llegará a fabricar masivamente en España, dónde afortunadamente lo peor de la crisis del COVID-19 parece que ya ha pasado (08/04/20); esperamos que este y otros diseños puedan ser útiles en otros países.

Aún así no nos damos por vencidos y seguiremos desarrollando el proyecto al menos en 2 versiones:

* Versión low cost (basada en Arduino y con caja de metacrilato, madera...)
* Versión pro (con un autómata PLC + un HMI y caja de chapa plegada en acero inoxidable)

En la siguiente figura podemos ver una representación del dispositivo:

![Reespirator](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/Reespirator-2020-redesign.jpg "Reespirator")



## Primeros pasos
**Antes de montar un respirador lea toda la documentación posible e infórmese bien, si necesita alguna aclaración abra un Issue y lo corregiremos en cuanto podamos. Si cree que puede mejorar el diseño, el código o que falta alguna cosa importante envíenos un Pull Request.**

## [Información médica básica del dispositivo Reespirator 2020](https://gitlab.com/reespirator/reespirator2020/-/blob/master/medical/MEDICAL.md)
El dispositivo se está diseñando para intentar cumplir las siguientes [especificaciones clínicas](https://foro.coronavirusmakers.org/index.php?p=/discussion/44/especificaciones-clinicas-de-un-respirador-util-en-esta-crisis#latest). Los dispositivos que estamos prototipando podrán funcionar en diferentes modos ventilatorios. En el siguiente enlace tendrás acceso a [Información médica básica sobre el dispositivo Reespirator 2020](https://gitlab.com/reespirator/reespirator2020/-/blob/master/medical/MEDICAL.md)

## [Estructura básica](https://gitlab.com/reespirator/reespirator2020/-/blob/master/case/CASE.md)
La versión low-cost de Reespirator 2020 consta de una [caja](https://gitlab.com/reespirator/reespirator2020/-/blob/master/case/CASE.md) diseñada para fabricarse mediante corte láser que contiene casi todos elementos del respirador en su interior. En el prototipo actual las piezas del prototipo se han diseñado para su corte por láser en metacrilato, si bien la imagen anterior corresponde a la nueva evolución que podrá fabricarse también con chapa plegada.

## [Sistema neumático](https://gitlab.com/reespirator/reespirator2020/-/blob/master/neumatic/NEUMATIC.md)
El [sistema neumático](https://gitlab.com/reespirator/reespirator2020/-/blob/master/neumatic/NEUMATIC.md) del Reespirator 2020 está basado en un sistema Jackson-Rees. Reespirator 2020 utiliza además una serie de válvulas, sensores de presión y caudal y tubuladuras para hacer llegar al aire a los pulmones del paciente.

## [Mecánica](https://gitlab.com/reespirator/reespirator2020/-/blob/master/mechanic/MECHANIC.md)
El [sistema mecánico](https://gitlab.com/reespirator/reespirator-doc/-/blob/master/mechanic/MECHANIC.md) pretende realizar los movimientos necesarios para realizar las maniobras de inspiración y espiración forzada del paciente mediante elementos mecánicos sustituyendo al personal humano que utilizaría el sistema de ventilación.

## [Electrónica](https://gitlab.com/reespirator/reespirator2020/-/blob/master/electronics/ELECTRONICS.md)
La [electrónica](https://gitlab.com/reespirator/reespirator-doc/-/blob/master/electronics/ELECTRONICS.md) de control gestiona el movimiento del motor y los sensores que permiten realizar un control de lazo cerrado automatizado del sistema.
Además de la electrónica de control se emplea una electrónica adicional como interfaz de usuario que permite monitorizar diferentes señales del respirador y modificar en tiempo real diferentes configuraciones del mismo.

## [Firmware](https://gitlab.com/reespirator/reespirator-doc/-/blob/master/firmware/FIRMWARE.md)
El sistema de control necesita ser programado con un [firmware](https://gitlab.com/reespirator/reespirator-doc/-/blob/master/firmware/FIRMWARE.md) que permita hacer funcionar el dispositivo. Dicho programa se ha realizado conforme a las especificaciones de los especialistas médicos para realizar las funciones para las que el dispositivo fue diseñado.

## [Simulación](https://gitlab.com/reespirator/reespirator2020/-/blob/master/simulation/SIMULATION.md)
En este apartado se consideran los fundamentos del sistema de control en lazo cerrado para los distintos modos de control que permite el Reespirator 2020. Los modelos matemáticos que permiten la [simulación numérica](https://gitlab.com/reespirasistemator/reespirator2020/-/blob/master/simulation/SIMULATION.md) del comportamiento del sistema corresponden a la información de este apartado.

## [Lista de materiales](https://gitlab.com/reespirator/reespirator2020/-/blob/master/bom/BOM.md)
La [lista de materiales, (BOM o Bill of materials)](https://gitlab.com/reespirator/reespirator2020/-/blob/master/bom/BOM.md) para construir un Reespirator 2020 es cuando menos complicada, incluye elementos como metacrilato, madera, MDF o chapa para la caja, sistmeas electrónicos como un Arduino Mega o un autómata PLC, y otros componentes, pero también elementos mecánicos y otros incluso impresos en 3D; pero sobre todo requiere también de la utilización de sistemas médicos tales como tubuladuras y un sistema ventilatorio Jackson-Rees.

## [Manual de usuario](https://gitlab.com/reespirator/reespirator2020/-/blob/master/manual/MANUAL.md)
El dispositivo Reespirator 2020 es un dispositivo médico y su uso sólo debe realizarse por personal especializado. Ofrecemos aquí un breve [manual de uso](https://gitlab.com/reespirator/reespirator-doc/-/blob/master/manual/MANUAL.md) del mismo; pero es el personal sanitario el que sabe los parámetros que deben utilizarse para el tratamiento de un paciente.

## [Vídeos]
En el siguiente enlace podemos ver algunos vídeos con detalles del Reespirator 2020 en funcionamiento:

* https://www.youtube.com/channel/UC9xr1HbWGLBjd4ADTvGcOnw


## Historia y principales cambios de esta versión

El proyecto Reespirator2020 toma como punto de partida el proyecto Reespirator 23 (o 24) v3 de **Reesistencia Team** a partir del cual realizamos un fork, el repositorio original está en [https://gitlab.com/reesistencia](https://gitlab.com/reesistencia).

En esta nueva versión se incluyen principalmente los siguientes cambios:

 - Revisión y reestructuración en profundidad del códido de Arduino para asegurar la robustez de funcionamiento en todos los supuestos.
 - La recuperación del interfaz básico con LCD de 20x04 y elementos sencillos de control (4 pulsadores y un encoder con pulsador).
 - Establecimiento y documentación de una interfaz de comunicación serie que permite la utilización de sistemas (en adelante llamados Display+) de visualización, control y conectividad, que pueden ser utilizados como accesorios para aportar mejor usabilidad al sistema.
 - Se trabaja para estandarizar y popularizar los sensores y electro-válvulas para utilizar partes (comerciales o diseñadas) posibles de conseguir con la situación de emergencia actual y a precios accesibles.
 - Posibilidad de usar diferentes interfaces de usuario.
 - Opción de utilizar un microcontrolador tipo Arduino o similar o bien un autómata PLC.

