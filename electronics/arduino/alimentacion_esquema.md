## Fuente de Alimentación. ##

Para la alimentación el sistema se empleará una fuente de alimentación capaz de suministrar un mínimo de 3A y con salida de 24V.

De entre todas las fuentes del mercado, lo recomendable sería emplear una fuente que haya sido diseñada para emplearse en equipos médicos puesto que dispondrá de circuitos específicos para el aislamiento ante posibles interferencias (EMI).

Preferiblemente se optará por una fuente de alimentación conmutada que permite entre otras cosas disponer de una fuente de alimentación menos voluminosa con un mayor rendimiento.

Un posible diagrama de bloques de la fuente de alimentación seleccionada es la que se presenta en la figura siguiente:

![Diagrama Bloques Fuente Alimentación](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/power_suply_schema.png "Diagrama Bloques Fuente Alimentación")

Existen muchas alternativas en el mercado, por lo que atendiendo a la disponibilidad y coste, se podrá optar por una u otra. Dicha fuente es la que alimentará entre otras partes del sistema a la placa de circuito impreso que se ha desarrollado. 

## Esquema del circuito electrónico de alimentación. ##

Como se podrá observar, esta parte del circuito corresponde a la alimentación de los distintos componentes y al sistema en general. Cabe destacar que se parte de una fuente de alimentación de +24V en corriente continua como se ha indicado anteriormente.

![Esquema Fuente Alimentación](https://gitlab.com/reespirator/reespirator2020/-/raw/master/images/arduino/alimentacion_esquema.png "Esquema Fuente Alimentación")

En el esquema se puede observar cómo de los bornes de entrada de la fuente de alimentación de 24V tenemos 4 salidas, las dos primeras son las que proporcionarán tensión y corriente a toda la placa, mientras que las dos inferiores son las que proporcionarán tensión al DRV.

La alimentación pasa a través de F1 que servirá de fusible para proteger el sistema y tras él se encuentra un Choke para evitar las interferencias y proteger de EMI. Tras el Choke CK1, se pueden distingir dos apartados:

- El primero de ellos es una **salida de +24V**. Esta salida se empleará en la parte de actuadores como drivers, válvulas..etc., como se verá más adelante.
- La segunda es una **salida de 5V** que se obtiene tras pasar un convertidor DC/DC con capacidad para conducir 3A. 

Todo esto permite tener una alimentación estable en la placa de +24V y +5V, protegida por diferentes componentes como ferritas y diodos de protección.

En esta parte también se puede ver una red de condensadores que son de desacoplo y que estarán ubicados lo más próximos posible a la alimentación de los circuitos integrados. 
Y por último también se pueden observar algunos de los conectores  de alimentación, que estarán disponibles para conectar periféricos, todos ellos protegidos por diodos unidireccionales TVS (Transient Voltage Suppressors).
