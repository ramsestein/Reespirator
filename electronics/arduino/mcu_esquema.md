## MCU Esquema. ##

Como se ha comentado en varias ocasiones, esta versión del respirador está basada en un Arduino Mega 2560.
Este microcontrolador será el encargado de llevar a cabo el control y gestión del sistema, sin embargo, dependiendo de la versión de la interfaz escogida, podrá relegar el control de la visualización a otro sistema a parte que permita la representación gráfica.

En cualquier caso, la placa desarrollada dispone de varias opciones de visualización tal y como se ha detallado en la documentación, en el apartado: [Interfaz](https://gitlab.com/reespirator/reespirator2020/-/blob/master/electronics/arduino/interfaz_esquema.md "Interfaz") 

En la siguiente imagen se puede ver el esquema de conexión empleado en el sistema.

![MCU](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/pinout_mcu.png "MCU")

Como se puede apreciar en la imagen, se dispone por un lado del microcontrolador con su pinout, donde se han señalado en **negrita**, aquellos pines fijos que no podían reubicarse en el diseño de la pcb, y por otro lado, existe un bloque denominado J11 consistente en un conector para facilitar la depuración del sistema mediante JTAG.

A partir del microcontrolador, se tiene toda la información proveniente de sensores y por lo tanto permitirá actuar sobre los distintos elementos como alarma, buzzer, válvulas..etc.
