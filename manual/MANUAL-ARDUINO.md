## Manual de usuario de Reespirator 2020 - Modelo Arduino ## 

**Interfaz de usuario**

Como se ha indicado en el apartado introductorio del presente documento, el interfaz de usuario de Reespirator 2020 cuenta con una botonera de gran tamaño para permitir realizar las acciones que se requieran por el equipo médico. Adicionalmente, existen dos grandes apartados dentro de la ventana de trabajo:

* Visualización gráfica de estado, permite visualizar la progresión de los parámetros de flujo y presión del respirador.
* Ventana de información, muestra, dependiendo de la opción pulsada:
    - La información actual de trabajo del respirador
    - Los parámetros de configuración del respirador

Las siguientes capturas de pantalla muestran estos bloques claramente diferenciados:

    Interfaz de Usuario de Reespirator 2020 con información de trabajo

    Interfaz de Usuario de Reespirator 2020 con parámetros de configuración

## Menú de navegación
El menú de opciones de Reespirator cuenta únicamente con dos botones de acción:
* **INICIO**: muestra los valores numéricos de presión, flujo y volumen en tiempo real.
* **CONF**: muestra los parámetros de configuración de Reespirator 

# Parámetros de configuración
Pulsando sobre el botón **CONF** se visualizan los parámetros de configuración de
Reespirator, los cuales se indican a continuación:
* **PIP** (cmH2O), permite establecer el valor de trabajo. El rango comprendido está entre 1 y 79
* **PEEP** (cmH2O), al igual que el caso de PIP, establece el valor de trabajo con un rango comprendido entre 0 y 78, teniendo que ser siempre menor que el valor de PIP.
* **FR** (rpm), con un rango comprendido entre 1 y 30 permite establecer la frecuencia de trabajo.

# Información en tiempo real
Al iniciar Reespirator se muestran los valores de funcionamiento en tiempo real. Estos parámetros de funcionamiento, que se detallan a continuación, se refrescan cada 100 milisegundos:
* PIP (cmH2O). Peak Inspiratory Pressure
* PEEP (cmH2O). Positive End-Expiratory Pressure
* FR (rpm). Frecuencia de Trabajo
* VOL (ml). Cantidad de Aire con el que está trabajando Reespirator

Asimismo, en esta ventana de parámetros, se permite activar el Modo Recruit en el respirador, el cual permite realizar el aumento transitorio de la presión transpulmonar aplicada para reclutar alvéolos en el pulmón colapsado. Seguidamente se detalla el modo de trabajo en reespirator.

**Modo de reclutamiento**
Como ya se ha indicado, el modo Recruit permite realizar un aumento transitorio de la presión transpulmonar aplicada para re-airear el pulmón colapsado. Para activar esta funcionalidad, simplemente basta con tocar en la pantalla sobre el botón **RECRUIT**.
Tras activarse, el botón anteriormente presionado cambia a color rojo y el texto de este cambia a STOP RECRUIT,
para permitir detener la operación.
Debido al concepto de transitoriedad, en Reespirator el tiempo máximo de la operación de Recruit está configurado
a un máximo de 40 segundos. Es decir que si, transcurrido este tiempo no se desactiva manualmente, Reespirator lo hará automáticamente.

**Visualización gráfica**
Reespirator muestra de forma gráfica y en tiempo real los niveles de Presión y Flujo respectivamente. El tiempo total de ciclo que se muestra en ambas gráficas es de un minuto, tiempo suficiente para poder visualizar la evolución más reciente del paciente.
Los rangos de visualización de gráficas son:
+ Presión: entre 0 y 50 cmH2O
+ Flujo: entre -20 y 30 litros por minuto

Visualización de Gráficas de Presión y Flujo en Tiempo Real
