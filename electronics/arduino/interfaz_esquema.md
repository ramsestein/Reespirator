## Interfaz del Sistema. ##

La interacción del usuario con el sistema se realizará a través de una serie de pulsadores y un encoder, además de un display, la ubicación de estos elementos estará debajo de un LCD 4x20 y a la derecha del mismo respectivamente.

Como se indicó en la introducción a la electrónica del respirador, este dispositivo **se ha pensado para tener distintas opciones de montaje y funcionamiento**, siendo la que se detalla a continuación la básica de ellas, pero no la única, puesto que **el sistema está preparado para la conexión a través de los terminales de TxRx y/o del USB**, para la comunicación con otros periféricos de visualización como puede ser una pantalla oled o HMI. 

**La selección de una forma de representación u otra se realizará vía firmware** por lo que no es necesario realizar ningún acople o adaptación a la placa desarrollada, simplemente se seleccionará el dispositivo de visualización deseado o instalado en el equipo en el firmware que se programa en el Arduino Mega.

**Esta versión de LCD 4x20, fue la primera versión que se pensó debido a su bajo coste y a la facilidad para disponer de estas en cualquier parte del mundo**, sin embargo, su limitación a la hora de representar señales y/o gráficas ha hecho necesario adaptar el sistema a otro tipo de dispositivos.

![LCD 4x20](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/lcd4x20.png "LCD 4X20")

En la siguiente imagen se puede ver el esquema de esta parte del sistema.

![Esquema de la Interfaz](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/interfaz_esquema.png "Esquema de la Interfaz")

Como se puede comprobar, se dispone de un LCD con backlight el cual se encuentra conectado en paralelo con el Arduino Mega, disponiendo de un potenciómetro para regular el contraste.

En cuanto a los pulsadores, se dispone de 4 pulsadores que irán cableados a la borna de la placa, estos pulsadores conectados a 24V. Para evitar rebotes y sobretensiones en el Arduino, se ha protegido esta parte del sistema mediante condensadores y **diodos BAS40**, que impedirán que el Arduino encuentre sobretensión en las patillas destinadas al control de los pulsadores. También se han acoplado **diodos unidireccionales TVS** (Transient Voltage Suppressors) para la protección en la tensión de 24V.
 
Por último, esta parte dispone de un **enconder rotatorio con switch**, el cual permitirá hacer selección de configuraciones por parte del usuario de una forma sencilla. 

![Encoder](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/encoder.png "Encoder")

El diagrama de bloques de la placa de circuito impreso diseñada para la versión del arduino, está disponible en el siguiente enlace:

**[Diagrama de Bloques](https://gitlab.com/reespirator/reespirator2020/-/blob/master/electronics/arduino/diagrama_bloques_esquema.md "Diagrama de Bloques")**