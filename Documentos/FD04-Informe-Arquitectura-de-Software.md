![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.001.png)		Logo de mi Cliente

![C:\Users\EPIS\Documents\upt.png](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.002.png)

**UNIVERSIDAD PRIVADA DE TACNA**

**FACULTAD DE INGENIERIA**

**Escuela Profesional de Ingeniería de Sistemas**


<a name="_hlk213012879"></a> **Proyecto *LastShot - Plataforma de Juegos Sociales Interactivos***

Curso: *Patrones de Software*


Docente: Mag. Patrick Cuadros Quiroga


Integrantes:


***SEBASTIAN NICOLAS FUENTES AVALOS		(2022073902)***

***MAYRA FERNANDA CHIRE RAMOS			(2021072620)***

***GABRIELA LUZKALID GUTIERREZ MAMANI 	(2022074263)***




**Tacna – Perú**

***2025***

**

|<a name="_hlk213012894"></a>CONTROL DE VERSIONES||||||
| :-: | :- | :- | :- | :- | :- |
|Versión|Hecha por|Revisada por|Aprobada por|Fecha|Motivo|
|1\.0|SFA|GGM|MCR|27/09/2025|Versión Original|
|2\.0|SFA|GGM|MCR|30/10/2025|Versión Original|









<a name="_hlk52661524"></a>**Sistema *LastShot - Plataforma de Juegos Sociales Interactivos***

**Documento de Arquitectura de Software**

**Versión *2.0***
**\


|CONTROL DE VERSIONES||||||
| :-: | :- | :- | :- | :- | :- |
|Versión|Hecha por|Revisada por|Aprobada por|Fecha|Motivo|
|1\.0|SFA|GGM|MCR|27/09/2025|Versión Original|
|2\.0|SFA|GGM|MCR|30/10/2025|Versión Original|

INDICE GENERAL

# **Contenido**
[***1.***	***INTRODUCCIÓN	***5******](#_toc69808834)

[**1.1.**	**Propósito (Diagrama 4+1)	**5****](#_toc69808835)

[**1.2.**	**Alcance	**5****](#_toc69808836)

[**1.3.**	**Definición, siglas y abreviaturas	**5****](#_toc69808837)

[**1.4.**	**Organización del documento	**6****](#_toc69808838)

[***2.***	***OBJETIVOS Y RESTRICCIONES ARQUITECTONICAS	***6******](#_toc69808839)

[2.1.1.	Requerimientos Funcionales	6](#_toc69808840)

[2.1.2.	Requerimientos No Funcionales – Atributos de Calidad	6](#_toc69808841)

[***3.***	***REPRESENTACIÓN DE LA ARQUITECTURA DEL SISTEMA	***6******](#_toc69808842)

[**3.1.**	**Vista de Caso de uso	**7****](#_toc69808843)

[3.1.1.	Diagramas de Casos de uso	7](#_toc69808844)

[**3.2.**	**Vista Lógica	**7****](#_toc69808845)

[3.2.1.	Diagrama de Subsistemas (paquetes)	7](#_toc69808846)

[3.2.2.	Diagrama de Secuencia (vista de diseño)	7](#_toc69808847)

[3.2.3.	Diagrama de Colaboración (vista de diseño)	7](#_toc69808848)

[3.2.4.	Diagrama de Objetos	7](#_toc69808849)

[3.2.5.	Diagrama de Clases	7](#_toc69808850)

[3.2.6.	Diagrama de Base de datos (relacional o no relacional)	8](#_toc69808851)

[**3.3.**	**Vista de Implementación (vista de desarrollo)	**8****](#_toc69808852)

[3.3.1.	Diagrama de arquitectura software (paquetes)	8](#_toc69808853)

[3.3.2.	Diagrama de arquitectura del sistema (Diagrama de componentes)	8](#_toc69808854)

[**3.4.**	**Vista de procesos	**8****](#_toc69808855)

[3.4.1.	Diagrama de Procesos del sistema (diagrama de actividad)	8](#_toc69808856)

[**3.5.**	**Vista de Despliegue (vista física)	**8****](#_toc69808857)

[3.5.1.	Diagrama de despliegue	8](#_toc69808858)

[***4.***	***ATRIBUTOS DE CALIDAD DEL SOFTWARE	***8******](#_toc69808859)

[**Escenario de Funcionalidad	**9****](#_toc69808860)

[**Escenario de Usabilidad	**9****](#_toc69808861)

[**Escenario de confiabilidad	**9****](#_toc69808862)

[**Escenario de rendimiento	**9****](#_toc69808863)

[**Escenario de mantenibilidad	**9****](#_toc69808864)

[**Otros Escenarios	**9****](#_toc69808865)















































1. <a name="_toc68679729"></a><a name="_toc69808834"></a>INTRODUCCIÓN

El presente proyecto tiene como propósito desarrollar una aplicación móvil interactiva denominada LastShot, orientada a ofrecer experiencias de juegos multijugador en tiempo real. El sistema está basado en una arquitectura cliente-servidor, donde la comunicación entre los usuarios y el backend se realiza mediante el protocolo WebSocket, permitiendo la transmisión continua de información sin interrupciones y garantizando una interacción fluida durante las partidas.

La aplicación integra una interfaz móvil intuitiva desarrollada con tecnologías modernas y un servidor backend desplegado en la nube a través de Azure App Service, utilizando una pila Node.js para la lógica del servidor y la gestión de eventos. Además, se incorporan servicios de Firebase, como Authentication y Firestore, para asegurar un manejo confiable de las cuentas de usuario, almacenamiento de datos y sincronización de perfiles en línea.

El desarrollo de este sistema busca poner en práctica conceptos fundamentales de la ingeniería de software, tales como el diseño modular, la comunicación en tiempo real, la integración de servicios externos y la seguridad en aplicaciones distribuidas. Asimismo, se enfatiza el uso de herramientas de modelado como PlantUML para representar visualmente los procesos del sistema mediante diagramas de clases, actividades y secuencia, lo que facilita la comprensión de la lógica interna y las interacciones entre los componentes.

En conjunto, este proyecto constituye un ejemplo de cómo la combinación de tecnologías actuales —como Firebase, WebSocket, Azure y Node.js— puede emplearse para construir soluciones escalables, seguras y orientadas a la colaboración entre múltiples usuarios. El resultado final es una aplicación capaz de gestionar perfiles, crear y unir salas de juego, sincronizar eventos en tiempo real y ofrecer una experiencia digital moderna y dinámica.

1. <a name="_toc68679730"></a><a name="_toc69808835"></a>Propósito

El propósito del proyecto es desarrollar una plataforma móvil interactiva de juegos sociales que facilite la integración y el entretenimiento en eventos y reuniones presenciales mediante tecnología moderna y accesible.

La finalidad principal es crear una solución digital que combine la comodidad de los dispositivos móviles con la experiencia social de los juegos presenciales, fortaleciendo vínculos interpersonales y eliminando barreras de acceso al entretenimiento grupal.

Este documento tiene como propósito específico:

- Definir la visión general de la plataforma LastShot, sus funcionalidades y su relevancia social.
- Comunicar a los interesados los objetivos y beneficios del proyecto, asegurando un entendimiento común.
- Orientar las fases de diseño, desarrollo y validación, alineando las expectativas de los usuarios con las capacidades técnicas del equipo de trabajo.

En términos prácticos, LastShot servirá como una aplicación móvil multiplataforma que permitirá a grupos de hasta 8 personas disfrutar de juegos interactivos en tiempo real durante reuniones sociales, eventos corporativos y actividades de integración.

Esto contribuirá a mejorar la experiencia social mediante dinámicas estructuradas, participación activa de todos los asistentes y eliminación de la necesidad de materiales físicos.

1. <a name="_toc68679731"></a><a name="_toc69808836"></a>Alcance

<a name="_hlk212821598"></a>El alcance del proyecto abarca el desarrollo y despliegue de una aplicación móvil multiplataforma construida en Flutter, diseñada para ofrecer juegos sociales interactivos con comunicación en tiempo real.

**Incluye lo siguiente:**

- Desarrollo de aplicación móvil para Android e iOS utilizando Flutter 3.0+.
- Implementación de sistema de autenticación de usuarios mediante Firebase Authentication.
- Desarrollo de backend en tiempo real con Node.js y Socket.IO para sincronización de juegos multijugador.
- Creación de interfaz de usuario intuitiva y atractiva con soporte para hasta 8 jugadores simultáneos.
- Sistema de salas de juego con códigos de acceso y gestión de sesiones.
- Integración de múltiples juegos sociales interactivos con mecánicas variadas.
- Despliegue en Google Play Store para dispositivos Android.

Con este alcance, el proyecto se enfoca en proporcionar una herramienta de entretenimiento social que facilite la integración grupal en eventos presenciales mediante tecnología móvil moderna.
\*\


1. <a name="_toc68679732"></a><a name="_toc69808837"></a>Definición, siglas y abreviaturas
- Flutter: Framework de desarrollo multiplataforma de Google para crear aplicaciones móviles nativas.
- Socket.IO: Biblioteca de JavaScript para comunicación en tiempo real bidireccional basada en eventos.
- WebSockets: Protocolo de comunicación que permite conexiones persistentes y bidireccionales.
- Firebase: Plataforma de desarrollo de aplicaciones móviles de Google que proporciona servicios backend.
- Node.js: Entorno de ejecución para JavaScript del lado del servidor.
- Backend: Parte del sistema que gestiona la lógica, base de datos y comunicación del servidor.
- Frontend: Interfaz de usuario con la que interactúan los jugadores en la aplicación móvil.
- UI/UX: User Interface / User Experience (Interfaz de Usuario / Experiencia de Usuario).
- API: Application Programming Interface (Interfaz de Programación de Aplicaciones).
- RAM: Random Access Memory (Memoria de Acceso Aleatorio).
- vCPU: Virtual Central Processing Unit (Unidad Central de Procesamiento Virtual).
  1. <a name="_toc69808838"></a>Organización del documento

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.003.png)

1. # <a name="_toc69808839"></a>**OBJETIVOS Y RESTRICCIONES ARQUITECTONICAS**
   1. Priorización de requerimientos

|**ID**|**Nombre**|**Descripción**|**Prioridad**|
| - | - | - | - |
|**RF01**|**Administrar Perfil de Usuario**|El sistema debe permitir a los usuarios administrar su perfil (registro, login, edición de datos personales, logout)|**ALTA**|
|**RF02**|**Explorar Juegos Multijugador**|El sistema debe permitir explorar y acceder a juegos multijugador (VASTA, El Infiltrado del Bar) con funcionalidades de sala compartida|**ALTA**|
|**RF03**|**Juegos de Dispositivo Único**|El sistema debe proporcionar juegos de dispositivo único (TODITO, YO NUNCA) que funcionen offline con animaciones|**MEDIA**|
|**RF04**|**Administrar Salas de Juego**|El sistema debe permitir administrar salas de juego (crear, configurar, invitar, gestionar participantes)|**ALTA**|
|**RF05**|**Comunicación en Tiempo Real**|El sistema debe implementar comunicación en tiempo real mediante WebSockets para sincronización de estados|**ALTA**|
|**RF06**|**Generación de Códigos QR**|El sistema debe generar códigos QR para facilitar el acceso y compartir la aplicación|**MEDIA**|
|**RF07**|**Manejo de Desconexiones**|El sistema debe manejar desconexiones automáticamente y permitir reconexión sin pérdida de progreso|**ALTA**|

1. ### <a name="_toc68679736"></a><a name="_toc69808840"></a>Requerimientos Funcionales

|<a name="_toc68679737"></a>**ID**|**Nombre**|**Descripción**|**Prioridad**|
| - | - | - | - |
|**RF01**|**Administrar Perfil de Usuario**|El sistema debe permitir a los usuarios administrar su perfil (registro, login, edición de datos personales, logout)|**ALTA**|
|**RF02**|**Explorar Juegos Multijugador**|El sistema debe permitir explorar y acceder a juegos multijugador (VASTA, El Infiltrado del Bar) con funcionalidades de sala compartida|**ALTA**|
|**RF03**|**Juegos de Dispositivo Único**|El sistema debe proporcionar juegos de dispositivo único (TODITO, YO NUNCA) que funcionen offline con animaciones|**MEDIA**|
|**RF04**|**Administrar Salas de Juego**|El sistema debe permitir administrar salas de juego (crear, configurar, invitar, gestionar participantes)|**ALTA**|
|**RF05**|**Comunicación en Tiempo Real**|El sistema debe implementar comunicación en tiempo real mediante WebSockets para sincronización de estados|**ALTA**|
|**RF06**|**Generación de Códigos QR**|El sistema debe generar códigos QR para facilitar el acceso y compartir la aplicación|**MEDIA**|
|**RF07**|**Manejo de Desconexiones**|El sistema debe manejar desconexiones automáticamente y permitir reconexión sin pérdida de progreso|**ALTA**|
###
1. ### <a name="_toc69808841"></a>Requerimientos No Funcionales – Atributos de Calidad

|**ID**|**Nombre**|**Descripción**|**Prioridad**|
| - | - | - | - |
|**RNF01**|**Rendimiento**|Tiempo de respuesta < 200ms para acciones locales y < 500ms para sincronización de red|**ALTA**|
|**RNF02**|**Usabilidad**|Interfaz intuitiva con jerga peruana familiar y iconos universalmente reconocibles|**ALTA**|
|**RNF03**|**Compatibilidad**|Compatible con Android 6.0+ (API 23+) e iOS 10.0+, soporte para WiFi y datos móviles|**ALTA**|
|**RNF04**|**Confiabilidad**|Disponibilidad del 99.5%, recuperación automática ante fallos, manejo robusto de errores|**ALTA**|
|**RNF05**|**Seguridad**|Encriptación HTTPS/WSS, validación de entrada, autenticación JWT, cumplimiento GDPR|**ALTA**|
|**RNF06**|**Mantenibilidad**|Código modular, documentación completa, logging detallado, arquitectura escalable|**MEDIA**|
|**RNF07**|**Portabilidad**|Flutter multiplataforma, backend Node.js independiente, Firebase cloud, despliegue multi-cloud|**MEDIA**|


1. Restricciones
   1. **Restricciones técnicas**
- La aplicación requiere conexión a internet activa durante toda la sesión de juego.
- La sincronización en tiempo real depende de la estabilidad de la conexión de red de los usuarios.
- El rendimiento puede variar en dispositivos de gama muy baja con menos de 2 GB de RAM.
- La versión inicial se publicará únicamente en Google Play Store (Android).
- El backend debe estar alojado en infraestructura cloud con disponibilidad 24/7.
- Las sesiones de juego están limitadas a un máximo de 8 jugadores simultáneos por cuestiones de experiencia de usuario y viabilidad técnica.
  1. **Restricciones de desarrollo**
- Duración del proyecto limitada a 3 meses según el cronograma establecido.
- Equipo reducido de 3 personas (DevOps, Analista de datos, Director de proyecto).
- Presupuesto total de S/. 12,078.41 que condiciona alcance y funcionalidades.
- Uso obligatorio de tecnologías específicas: Flutter, Node.js, Socket.IO, Firebase.
- Cumplimiento con normativas de protección de datos personales (Ley N° 29733).
  1. **Restricciones operativas**
- Los usuarios deben disponer de smartphones compatibles (Android 6.0+ o iOS 10+).
- Las sesiones de juego requieren que todos los participantes estén físicamente presentes.
- El sistema no ofrece modo offline ni juego individual.
- La aplicación no incluye matchmaking automático con desconocidos.

1. # <a name="_toc69808842"></a>**REPRESENTACIÓN DE LA ARQUITECTURA DEL SISTEMA**
   1. <a name="_toc68679738"></a><a name="_toc69808843"></a>Vista de Caso de uso
      1. ### <a name="_toc69808844"></a>Diagramas de Casos de uso
![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.004.png)

1. <a name="_toc68679739"></a><a name="_toc69808845"></a>Vista Lógica

1. ### <a name="_toc68679740"></a><a name="_toc69124248"></a><a name="_toc69808846"></a>Diagrama de Subsistemas (paquetes)

![ref1]
1. ### <a name="_toc69808847"></a>Diagrama de Secuencia (vista de diseño)
#### `     `*D[*iagrama de Secuencia*](#_heading=h.7lj19pswwxxu) del CUS - Administrar Perfil de Usuario*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.006.png)





#### *D[*iagrama de Secuencia*](#_heading=h.7lj19pswwxxu) del CUS - Explorar Juegos Multijugador*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.007.png)






#### *D[*iagrama de Secuencia*](#_heading=h.7lj19pswwxxu) del CUS - Explorar Juegos de Dispositivo Único*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.008.png)







#### *D[*iagrama de Secuencia*](#_heading=h.7lj19pswwxxu) del CUS - Administrar Sala de Juego*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.009.png)

1. ### <a name="_toc69808848"></a>Diagrama de Colaboración (vista de diseño)
![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.010.png)
1. ### <a name="_toc69808849"></a>Diagrama de Objetos
#### *Diagrama de objetos del CUS - Administrar Perfil de Usuario*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.011.png)

#### *Diagrama de objetos del CUS -  Explorar Juegos Multijugador*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.012.png)

#### *Diagrama de objetos del CUS -  Explorar Juegos de Dispositivo Único*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.013.png)

#### *Diagrama de objetos del CUS - Administrar Sala de Juego*

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.014.png)
1. ### <a name="_toc69808850"></a>Diagrama de Clases
![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.015.png)
1. ### <a name="_toc69808851"></a>Diagrama de Base de datos (relacional o no relacional)
![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.016.png)

1. <a name="_toc68679746"></a><a name="_toc69808852"></a>Vista de Implementación (vista de desarrollo)
   1. ### <a name="_toc69808853"></a>Diagrama de arquitectura software (paquetes)

![ref2]
1. ### <a name="_toc68679747"></a><a name="_toc69808854"></a>Diagrama de arquitectura del sistema (Diagrama de componentes)

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.018.png)

1. <a name="_toc68679741"></a><a name="_toc69124251"></a><a name="_toc69808855"></a>Vista de procesos
   1. ### <a name="_toc68679742"></a><a name="_toc69124252"></a><a name="_toc69808856"></a>Diagrama de Procesos del sistema (diagrama de actividad)
![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.019.png)


1. <a name="_toc68679744"></a><a name="_toc69808857"></a>Vista de Despliegue (vista física)
   1. ### <a name="_toc68679745"></a><a name="_toc69808858"></a>Diagrama de despliegue

![](Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.020.png)

1. # <a name="_toc69808859"></a>**ATRIBUTOS DE CALIDAD DEL SOFTWARE**
<a name="_toc69808860"></a>**Escenario de Funcionalidad**

Un grupo de cuatro amigos quiere jugar VASTA en una reunión; el organizador crea una sala y comparte el código QR, todos se conectan, configuran el juego y participan sin problemas, logrando que el 100% de las funciones principales operen correctamente sin errores críticos en el flujo de juego.

<a name="_toc69808861"></a>**Escenario de Usabilidad**

Cuando un usuario nuevo descarga la aplicación por primera vez, intenta crear una cuenta y unirse a una partida. Completa el registro y se une al juego en menos de dos minutos sin ayuda, logrando que el 90% de los usuarios nuevos finalicen su primer juego exitosamente.

<a name="_toc69808862"></a>**Escenario de confiabilidad**

Si un jugador pierde la conexión WiFi durante una partida multijugador, la aplicación se reconecta automáticamente y sincroniza el estado del juego en menos de diez segundos, garantizando una disponibilidad del 99.5%.

<a name="_toc69808863"></a>**Escenario de rendimiento**

Con 50 salas simultáneas y ocho jugadores por sala (400 usuarios en total), cuando todos los jugadores envían respuestas al mismo tiempo, el sistema procesa todas las acciones sin lag perceptible, manteniendo una latencia menor a 200 ms y un throughput superior a 1000 transacciones por minuto.

<a name="_toc69808864"></a>**Escenario de mantenibilidad**

Cuando surge la necesidad de agregar un nuevo juego, como "Adivina la Película", el desarrollador implementa la funcionalidad y el módulo se integra sin afectar los juegos existentes, permitiendo la implementación en menos de dos días sin regresiones en funcionalidades previas.

2

[ref1]: Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.005.png
[ref2]: Aspose.Words.c4f94265-1f8f-4d6c-8234-bab4237e6a31.017.png
