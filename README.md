# Vamos a aprender ROS con GoPiGO3

<blockquote><a rel="cc:attributionURL" property="dct:title" href="https://github.com/Albert-Alvarez/ros-con-gopigo3">Vamos a aprender ROS con GoPiGo3</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://thealbert.dev/">Albert Álvarez Carulla</a> se distribuye bajo una <a rel="license" href="https://creativecommons.org/licenses/by-nd/4.0/deed.es">Licencia Creative Commons Atribución-SinDerivadas 4.0 Internacional (CC BY-ND 4.0)</a>.<br /><img alt="Licencia Creative Commons" style="border-width:0" src="https://licensebuttons.net/l/by-nd/4.0/88x31.png" /></a></blockquote>

Si estás aquí es porque, como te habrá *spoileado* el título, vamos a empezar a ver **cómo funciona *Robot Operating System* (ROS)** utilizando la **plataforma GoPiGo3**. Hasta ahora, de ROS, hemos visto cómo instalarlo, cómo crear *packages*, cómo compilar el *workspace*, cómo correr nuestros nodos, cómo crear lanzadores, cómo lanzar y ver simulaciones, etc. Una larga lista que de momento no hemos explotado sobre robots físicos. 



> Como habrás leído, en estas sesiones damos por hecho que ya tienes ROS instalado y sabes hacer las operaciones básicas. Si no es el caso, te recomiendo que te pongas manos a la obra y primero veas qué es ROS, cómo instalarlo y cómo hacer las operaciones básicas. **Estas no pretenden ser unas sesiones de introducción básica a ROS**. Aún así, no te alarmes, **se detallarán todas las operaciones a realizar por si hay alguna cosa que no logras recordar** 😉

## Requerimientos

Para llevar a cabo estas sesiones necesitaras de los siguientes requerimientos:

- Un ordenador (PC) con [Ubuntu Desktop 18.04](https://releases.ubuntu.com/18.04/). Puede ser una Máquina Virtual (VM).
- [ROS Melodic](http://wiki.ros.org/melodic) instalado en el PC.
- Una plataforma [GoPiGo3](https://www.dexterindustries.com/gopigo3/) con una [Raspberry Pi 3 B+](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/).
- Un [*Laser Imaging Detection and Ranging* (LIDAR)](https://es.wikipedia.org/wiki/LIDAR) modelo [YDLIDAR X4](https://www.ydlidar.com/products/view/5.html).
- Un [módulo de cámara](https://www.raspberrypi.org/products/camera-module-v2) para la Raspberry Pi.
- Una tarjeta microSD para la Raspberry Pi de mínimo 16 GB con [Raspberry Pi OS](https://www.raspberrypi.org/software/), con los **controladores del GoPiGo3** y **ROS Melodic instalados** y la **cámara habilitada**.
- Un transformador para alimentar la Raspberry Pi cuando estemos programando en ella. Ha de cumplir [estas especificaciones](https://www.raspberrypi.org/documentation/hardware/raspberrypi/power/README.md#:~:text=The power supply requirements differ,uses a USB-C connector).
- 8 baterías tipo AAA para alimentar el robot cuando se tenga que mover.
- Un *router* con conectividad WiFi. Obviamente, mejor con acceso a internet, pero no es indispensable. Simplemente, nos servirá para conectar el PC con la Raspberry Pi.

## Planificación

La planificación está pensada para **dos sesiones en el aula** más un **proyecto final**. En la **primera sesión**, veremos cómo configurar nuestro *workspace*, realizar **operaciones básicas** como conectarse remotamente a la Raspberry Pi, y hacer que el robot ejecute las operaciones básicas como moverse, capturar imágenes con la cámara o leer la información provista por el LIDAR. En la **segunda sesión**, se implementará un sistema robótico mediante el cuál, **manualmente**, se hará un **mapeado del habitáculo** en el que se encuentre el robot. Por último, el **proyecto** consistirá en realizar dicho **mapeado de manera autónoma** para así, posteriormente, poder decir al robot que vaya de una localización a otra él solo.

Cada sesión está organizada en su propia carpeta dentro del repositorio. Dirígete a la carpeta correspondiente y sigue el archivo `README`que allí encontrarás (o clica directamente sobre los siguientes enlaces:

- Primera sesión: `session1` ([enlace](session1/README.md)).
- Segunda sesión: session2 ([enlace](sessions2/README.md)).
- Proyecto: `project` ([enlace](project/README.md)).