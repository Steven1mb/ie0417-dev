*************
Laboratorio 1
*************
+---------------+--------------+
| Estudiante    |  Carnet      |
+---------------+--------------+
|| Steven Mora | B95109        |
+---------------+--------------+


**Planeamiento**
================

De manera breve, explique cómo se pueden planear los releases de funcionalidad del proyecto para habilitar lo más rápido posible el desarrollo en el equipo del App (externo a eieLabs).

Utilice conceptos de planeamiento a largo plazo con metodologías Agile (Quiz 2).


Paso 1:
^^^^^^^

Para iniciar con el proyecto se tiene la idea general de este ultimo: Se tiene un proyecto en el cual se tendrá 
dos secciones importantes el eieManager que se encarga de comunicarse con los dispositivos de la empresa,este eieManager debe
de servir como API es decir,sirve como un intermediario entre los dispositivos a controlar y el cliente,
los dispositivos a controlar como un grupo es el eieDevice el cual debe recibir 
comandos desde el eieManager actuar de acuerdo a estos comandos recibidos y de ser el caso se genera una respuesta al cliente.

Se crearan procesos para construir un eieManager bastante solido,una base comunicacion AP queI en la pueda ser 
fácilmente consumido por otro equipo de desarrollo
para implementar un cliente en un App móvil con GUI.

Paso 2:
^^^^^^^

Al ser un diseño de software los aspectos de mas valor caerán en la estabilidad y modificabilidad de diseño API aplicado.

Paso 3:
^^^^^^^

eieManager
""""""""""

*Comandos*

* Definir los comandos predefinidos que se enviaran a los eieDevices
* Esquematizar el rango de dispositivos aplicado por cada uno de los comandos
  
*API*

* Iniciar el API bajo un protocolo de comunicacion RPC
* Crear un puente de comunicacion tal que el eieManager pueda recopilar todas las respuestas y se las presente al cliente
* Permitir que el funcionamiento del API sea independiente del sistema operativo utilizado y los comandos que transiten por el *cohesion*
* Configurar el API de manera que soporte concurrencia en cantidad de comandos aplicados como la cantidad de dispositivos a los cuales se les envia el comandos
* Restablecimiento a un punto anterior

Paso 4:
^^^^^^^

