## Interface TFT-Touch

Para pantalla visualizar las gráficas de funcionamiento del Reespirator 2020 y poder interactuar con el dispositivo podemos utilizar una pantalla TFT táctil conectada a una Raspberry Pi o una Beagle Bone. En el prototipo original Reespirator 23 se utilizó una BeagleBone con una pantalla TFT táctil de 7" que es lo se tenía disponible en ese momento, sin embargo dado que se empleó Python, el código es fácilmente adaptable a otras plataformas como Raspberry Pi o similares.
Mediante comunicación serie, el Arduino Mega del sistema de control envía y recibe los datos necesarios para monitorizar y manejar el dispositivo.

Actualmente (19/04/2020), la única combinación que está completamente funcional corresponde al uso de la BeagleBone con el último firmware de Arduino para Reespirator 23, ambos están disponibles en los repositorios de los anteriores enlaces.

Para utilizar una Raspberry Pi no debería ser muy diferente que con BeagleBone, es necesario configurar el Python que en las distribuciones de Raspbian suelen estar incluidas e instalar algunas librerías como PyQt pero el software de visualización/interacción debería funcionar igualmente.
En el siguiente enlace se describe por ejemplo como instalar Qt5: https://wiki.qt.io/Raspberry_Pi_Beginners_Guide/es 
