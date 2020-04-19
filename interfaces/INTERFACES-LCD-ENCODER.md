## Interface LCD + Encoder + 4 pulsadores

Los distintos modelos de Reespirator 2020 utilizan diferentes tipos de interfaces de usuario según la disponibilidad en el lugar de fabricación.

El primer prototipo incluía simplemente un Arduino y una simple pantalla LCD y un encoder y con esta configuración se lograron hacer las primeras pruebas preclínicas, también se consideró la posibilidad de usar botones en lugar de encoders porque podían resultar más rápidos para cambiar las configuraciones en ciertos momentos críticos del tratamiento; pero finalmente se optó por una configuración basada en 
- una pantalla LCD de 20x4
- un encoder
- 4 pulsadores
- un zumbador

Los médicos consideraron que si bien podría ser suficiente, era más conveniente incluir una pantalla gráfica para representar las señales producidas por el respirador. 

![Configuración LCD+Encoder+Pulsadores](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/hmi/interfaz_arduino_hmi.png "Configuración LCD+Encoder+Pulsadores")

>La versión con pantalla LCD, encoder y pulsadores se documenta aquí para aquellos lugares donde no se puedan implementar las soluciones gráficas, y además utilizando un ordenador es posible visualizar las gráficas y se puede utilizar igualmente esta configuración básica.
