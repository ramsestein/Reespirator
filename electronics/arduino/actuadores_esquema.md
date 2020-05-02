## ACTUADORES Esquema. ##

En esta parte del esquema electrónico se verán los distintos componentes empleados para actuar sobre el sistema.

En la siguiente imagen se puede observar el diseño de lo mencionado:

[Esquema Actuadores](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/actuadores_esquema.png "Actuadores") 

Como se puede observar, el primero de los integrados que se observa es el **ULN2803A**, este circuito integrado, está compuesto por un conjunto de ocho puertas inversoras implementadas con transistores NPN tipo Darlington, lo que le permite soportar la conexión de dispositivos que requieren una fuerte demanda de corriente como motores paso a paso o relés que se podrán activar con una baja corriente de entrada.

![ULN2803](https://upload.wikimedia.org/wikipedia/commons/a/a2/ULN2003A_Pin_Connection.PNG)

De este modo, están conectados a sus entradas las señales de control del microcontrolador, y las salidas irán a los dispositivos mencionados como son el FAN (Ventilador), los drivers de los motores..etc. Tal y como se ha mencionado en otros apartados, estas salidas están protegidas mediante diodos TVS unidireccionales (SMF30).

![Esquema Actuadores](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/actuadores_esquema1.png "Actuadores")
 
Debido al elevado número de dispositivos a controlar es necesario disponer de dos de estos circuitos integrados, empleando el segundo de ellos para controlar el Buzzer, el backlight de la pantalla LCD, el caldeo (heater) del caudalímetro, así como el control de 2 diodos led que se han añadido para posibles indicaciones.

![Esquema Actuadores](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/actuadores_esquema2.png "Actuadores")

También se ha tenido en cuenta en esta parte una alarma para el **SAI** (Sistema de Alimentación Ininterrumpida), de forma que el sistema tenga control sobre cuál es la alimentación con la que se está funcionando.

![Esquema Actuadores](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/actuadores_esquema3.png "Actuadores")

Por último, estaría el control de las electroválvulas, en este caso se pueden controlar 2 electroválvulas. El control de éstas se realiza a través de la conexión del microcontrolador al circuito integrado **L293**, el integrado L293D incluye dos circuitos puente H, para controlar cargas como motores o en el caso que nos ocupa electroválvulas:

![L293](https://upload.wikimedia.org/wikipedia/commons/7/77/H_bridge2.png)

La salida del L293, que irá conectada a las electroválvulas está protegida una vez más mediante ferritas y diodos TVS unidireccionales, 

![Esquema Actuadores](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/actuadores_esquema4.png "Actuadores")

El diagrama de bloques de la placa de circuito impreso diseñada para la versión del arduino, está disponible en el siguiente enlace:

**[Diagrama de Bloques](https://gitlab.com/reespirator/reespirator2020/-/blob/master/electronics/arduino/diagrama_bloques_esquema.md "Diagrama de Bloques")**