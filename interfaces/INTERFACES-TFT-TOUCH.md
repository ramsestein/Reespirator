## Interface TFT-Touch

Para pantalla visualizar las gráficas de funcionamiento del Reespirator 2020 y poder interactuar con el dispositivo podemos utilizar una pantalla TFT táctil conectada a una Raspberry Pi o una Beagle Bone. En el prototipo original Reespirator 23 se utilizó una BeagleBone con una pantalla TFT táctil de 7" que es lo se tenía disponible en ese momento, sin embargo dado que se empleó Python, el código es fácilmente adaptable a otras plataformas como Raspberry Pi o similares.
Mediante comunicación serie, el Arduino Mega del sistema de control envía y recibe los datos necesarios para monitorizar y manejar el dispositivo.
