# Laboratorio N° 1 de robotica
## Descripcion General
>En este repositorio encontrarás las memorias y programas desarrollados durante la primera práctica de laboratorio del curso de Robótica. Esta práctica está diseñada para aprender a manejar el manipulador ABB IRB 140 en el espacio del laboratorio LabSIR utilizando el controlador ABB IRC5. El objetivo principal es escribir un logotipo, en nuestro caso el logotipo de XBOX mas nuestras iniciales(J,J,R), con un marcador en un tablero inclinado. Esto se logra mediante el uso de una herramienta de diseño libre acoplada al manipulador y la definición de las trayectorias en Robot Studio.
## Diagrama de Flujo
![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://github.com/JuanAAlonso/Laboratorio1-Robtica-Industrial/blob/main/2.%20Diagrama%20de%20flujo/Diagrama%20de%20flujo%20acciones%20del%20robot.png)
>Al comenzar el proceso, cargarse el módulo con el código de RAPID e iniciar la rutina, lo primero que esperara el ROBOT será a que la entrada digital 1 (DI_01) se presione, a lo que de manera inmediata se encenderá el Led (DO_01) y comenzará a dibujar la trayectoria del logotipo de X (ver anexo “1. Descripción de la solución”. Una vez terminada la rutina el robot ira a una posición de Home con todas sus articulaciones en 0 grados y esperara a que la segunda entrada digital (DI_02) se active para irse a una posición de mantenimiento donde fácilmente se pueda retirar la herramienta y acto seguido apagara el Led (DO_01).
## Descripcion de Funcionalidades
>La función movj en RAPID se utiliza para controlar el movimiento del robot a través de puntos de articulación específicos en una trayectoria definida. Este tipo de movimiento se conoce como movimiento de articulación. Al emplear movj, el robot se mueve de un punto a otro utilizando las articulaciones del robot, lo que permite una mayor flexibilidad en la trayectoria. Este método es útil cuando se requieren movimientos precisos y rápidos, ya que minimiza el tiempo de desplazamiento entre los puntos y permite ajustes finos en las articulaciones para alcanzar la posición deseada con precisión.

>Por otro lado, la función movl en RAPID se utiliza para controlar el movimiento del robot a lo largo de una trayectoria lineal entre dos puntos en el espacio de trabajo. Este tipo de movimiento se conoce como movimiento lineal. Al utilizar movl, el robot se mueve en una línea recta desde un punto inicial hasta un punto final, lo que permite realizar movimientos de desplazamiento suaves y continuos. Este método es útil cuando se requiere que el robot siga una trayectoria lineal precisa, como en operaciones de ensamblaje o soldadura, donde se necesita un movimiento fluido y preciso para completar la tarea de manera eficiente.
## Plano de la Planta
![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://github.com/JuanAAlonso/Laboratorio1-Robtica-Industrial/blob/main/3.%20Estación%20y%20distribución%20de%20objetos.PNG)
>La planta como se puede ver en la imagen, distribuye los objetos como se solicita en el laboratorio de la siguiente manera: El robot ubicado su centro sobre el 0 del plano cartesiano, mientras que el logo en superficie plana esta en el playo y(-), x(+) con una pequeña inclinación correspondiente a las tablas del laboratorio, por otra parte el logotipo en superficie inclinada (30°) está en el plano y(+),x(+).
## Videos
>https://drive.google.com/drive/folders/1DHHZ0SXXfLdBjRneUswRhG2qwDi7JxS7?usp=drive_link
