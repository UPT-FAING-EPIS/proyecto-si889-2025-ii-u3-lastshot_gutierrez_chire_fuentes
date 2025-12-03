![](Aspose.Words.0e16f46b-6fa6-4f30-b571-198b9c055436.001.png)

![C:\Users\EPIS\Documents\upt.png](Aspose.Words.0e16f46b-6fa6-4f30-b571-198b9c055436.002.png)

**UNIVERSIDAD PRIVADA DE TACNA**

**FACULTAD DE INGENIERIA**

**Escuela Profesional de Ingeniería de Sistemas**


` `**Proyecto *LastShot - Plataforma de Juegos Sociales Interactivos***

Curso: *Patrones de Software*


Docente: Mag. Patrick Cuadros Quiroga


Integrantes:


***SEBASTIAN NICOLAS FUENTES AVALOS		(2022073902)***

***MAYRA FERNANDA CHIRE RAMOS			(2021072620)***

***GABRIELA LUZKALID GUTIERREZ MAMANI 	(2022074263)***




**Tacna – Perú**

***2025***
**\


|CONTROL DE VERSIONES||||||
| :-: | :- | :- | :- | :- | :- |
|Versión|Hecha por|Revisada por|Aprobada por|Fecha|Motivo|
|1\.0|SFA|GGM|MCR|27/09/2025|Versión Original|
|2\.0|SFA|GGM|MCR|30/10/2025|Versión Original|











**Sistema <a name="_hlk212816586"></a>*LastShot - Plataforma de Juegos Sociales Interactivos***

**Documento de Especificación de Requerimientos de Software**

**Versión *2.0***
**\


|CONTROL DE VERSIONES||||||
| :-: | :- | :- | :- | :- | :- |
|Versión|Hecha por|Revisada por|Aprobada por|Fecha|Motivo|
|1\.0|SFA|GGM|MCR|27/09/2025|Versión Original|
|2\.0|SFA|GGM|MCR|30/10/2025|Versión Original|

**INDICE GENERAL**
#
[INTRODUCCIÓN	4](#_toc212821236)

[I. Generalidades de la Empresa	4](#_toc212821237)

[1. Nombre de la Empresa	4](#_toc212821238)

[2. Vision	4](#_toc212821239)

[3. Mision	4](#_toc212821240)

[4. Organigrama	5](#_toc212821241)

[II. Visionamiento de la Empresa	5](#_toc212821242)

[1. Descripción del Problema	5](#_toc212821243)

[2. Objetivos de Negocios	5](#_toc212821244)

[3. Objetivos de Diseño	5](#_toc212821245)

[4. Alcance del proyecto	6](#_toc212821246)

[5. Viabilidad del Sistema	6](#_toc212821247)

[6. Información obtenida del Levantamiento de Informacion	6](#_toc212821248)

[III.  Análisis de Procesos	7](#_toc212821249)

[a) Diagrama del Proceso Actual – Diagrama de actividades	7](#_toc212821250)

[b) Diagrama del Proceso Propuesto – Diagrama de actividades Inicial	7](#_toc212821251)

[IV Especificacion de Requerimientos de Software	8](#_toc212821252)

[a) Cuadro de Requerimientos funcionales Inicial	8](#_toc212821253)

[b) Cuadro de Requerimientos No funcionales	8](#_toc212821254)

[c) Cuadro de Requerimientos funcionales Final	9](#_toc212821255)

[d) Reglas de Negocio	10](#_toc212821256)

[V Fase de Desarrollo	10](#_toc212821257)

[1. Perfiles de Usuario	10](#_toc212821258)

[2. Modelo Conceptual	11](#_toc212821259)

[a) Diagrama de Paquetes	11](#_toc212821260)

[b) Diagrama de Casos de Uso	11](#_toc212821261)

[c) Escenarios de Caso de Uso (narrativa)	11](#_toc212821262)

[3. Modelo Logico	16](#_toc212821263)

[a)	Diagrama de objetos	16](#_toc212821264)

[b) Diagrama de Actividades con objetos	18](#_toc212821265)

[c) Diagrama de Secuencia	20](#_toc212821266)

[d) Diagrama de Clases	22](#_toc212821267)

[CONCLUSIONES	22](#_toc212821268)

[RECOMENDACIONES	22](#_toc212821269)

[BIBLIOGRAFÍA	23](#_toc212821270)

[WEBGRAFÍA	23](#_toc212821271)















# <a name="_toc212821236"></a>[**INTRODUCCIÓN**](#_heading=h.y5jf20tiz1ev)
El presente proyecto tiene como propósito desarrollar una aplicación móvil interactiva denominada LastShot, orientada a ofrecer experiencias de juegos multijugador en tiempo real. El sistema está basado en una arquitectura cliente-servidor, donde la comunicación entre los usuarios y el backend se realiza mediante el protocolo WebSocket, permitiendo la transmisión continua de información sin interrupciones y garantizando una interacción fluida durante las partidas.

La aplicación integra una interfaz móvil intuitiva desarrollada con tecnologías modernas y un servidor backend desplegado en la nube a través de Azure App Service, utilizando una pila Node.js para la lógica del servidor y la gestión de eventos. Además, se incorporan servicios de Firebase, como Authentication y Firestore, para asegurar un manejo confiable de las cuentas de usuario, almacenamiento de datos y sincronización de perfiles en línea.

El desarrollo de este sistema busca poner en práctica conceptos fundamentales de la ingeniería de software, tales como el diseño modular, la comunicación en tiempo real, la integración de servicios externos y la seguridad en aplicaciones distribuidas. Asimismo, se enfatiza el uso de herramientas de modelado como PlantUML para representar visualmente los procesos del sistema mediante diagramas de clases, actividades y secuencia, lo que facilita la comprensión de la lógica interna y las interacciones entre los componentes.

En conjunto, este proyecto constituye un ejemplo de cómo la combinación de tecnologías actuales —como Firebase, WebSocket, Azure y Node.js— puede emplearse para construir soluciones escalables, seguras y orientadas a la colaboración entre múltiples usuarios. El resultado final es una aplicación capaz de gestionar perfiles, crear y unir salas de juego, sincronizar eventos en tiempo real y ofrecer una experiencia digital moderna y dinámicas.[	](#_heading=h.y5jf20tiz1ev)
# <a name="_toc212821237"></a>[**I. Generalidades de la Empresa**	](#_heading=h.l35cjpfq0moy)
## `	`**<a name="_toc212821238"></a>[**1. Nombre de la Empresa**](#_heading=h.7lj19pswwxxu)**
`	     `CAPICODEX[	](#_heading=h.7lj19pswwxxu)
## `	`**<a name="_toc212821239"></a>[**2. Vision**](#_heading=h.7lj19pswwxxu)**
En CAPICODEX, aspiramos a ser líderes en el desarrollo de soluciones tecnológicas que impulsen el crecimiento regional a través de la innovación digital. Con proyectos como GameOn Network y el Dashboard de Accidentes Tacna, buscamos transformar la gestión de información en distintos sectores, promoviendo la eficiencia, la transparencia y el acceso equitativo a los datos. Nuestra visión es fortalecer el ecosistema tecnológico de la región, conectando a ciudadanos, instituciones y autoridades en un entorno digital moderno y colaborativo.

[	](#_heading=h.7lj19pswwxxu)
## `	`**<a name="_toc212821240"></a>[**3. Mision**](#_heading=h.7lj19pswwxxu)**
Nuestra misión en CAPICODEX es desarrollar plataformas digitales que optimicen la gestión y el acceso a la información pública, facilitando la toma de decisiones basada en datos. Nos comprometemos a ofrecer herramientas tecnológicas innovadoras, seguras y accesibles que promuevan la participación ciudadana, la prevención de riesgos y el desarrollo sostenible de la ciudad de Tacna.

[	](#_heading=h.7lj19pswwxxu)
## `	`**<a name="_toc212821241"></a>[**4. Organigrama**](#_heading=h.7lj19pswwxxu)**
[	](#_heading=h.7lj19pswwxxu)![Organigrama](Images/organigrama.png)
# <a name="_toc212821242"></a>[**II. Visionamiento de la Empresa**	](#_heading=h.l35cjpfq0moy)
## `	`**<a name="_toc212821243"></a>[**1. Descripción del Problema**](#_heading=h.7lj19pswwxxu)**
Actualmente, el entretenimiento social en reuniones y eventos presenta las siguientes limitaciones:

- **Dependencia de materiales físicos**: los juegos tradicionales requieren cartas, dados, tableros y otros elementos que deben comprarse, transportarse y prepararse.
- **Tiempo de preparación**: las actividades recreativas exigen planificación previa y setup, restando espontaneidad a las reuniones.
- **Limitaciones de participantes**: muchos juegos físicos están diseñados para cantidades específicas de jugadores, excluyendo a algunos asistentes.
- **Falta de variedad**: adquirir múltiples juegos físicos implica costos elevados y espacio de almacenamiento.
- **Desigualdad en la participación**: en reuniones sin estructura lúdica, algunos asistentes tienden a quedar al margen de las conversaciones.
- **Aplicaciones existentes inadecuadas**: la mayoría de apps de juegos se enfocan en entretenimiento individual o competencias online con desconocidos, perdiendo el aspecto social presencial.

Esto impide contar con una solución digital accesible, versátil y orientada específicamente al fortalecimiento de vínculos interpersonales en contextos presenciales, limitando la calidad de la experiencia social en eventos y reuniones.[	](#_heading=h.7lj19pswwxxu)
## `	`**<a name="_toc212821244"></a>[**2. Objetivos de Negocios**](#_heading=h.7lj19pswwxxu)**
El proyecto busca sentar una base sólida para la monetización futura mediante compras in-app y funciones premium, alcanzar 10,000 descargas en los primeros seis meses, mantener un promedio de tres partidas por sesión de usuario, lograr que el 60% de los usuarios inviten amigos mediante códigos QR y posicionarse como la aplicación número uno de juegos de mesa digitales en Perú.
## `	`**<a name="_toc212821245"></a>[**3. Objetivos de Diseño**](#_heading=h.7lj19pswwxxu)**
La aplicación presenta una interfaz intuitiva que no requiere tutorial, proporcionando una experiencia de juego fluida y entretenida. Está optimizada para pantallas táctiles y uso con una mano, cuenta con una arquitectura escalable que soporta crecimiento exponencial y funciona tanto en modo online (multijugador) como offline (solo device).[	](#_heading=h.7lj19pswwxxu)
## `	`**<a name="_toc212821246"></a>[**4. Alcance del proyecto**](#_heading=h.7lj19pswwxxu)**
El alcance del proyecto abarca el desarrollo y despliegue de una aplicación móvil multiplataforma construida en Flutter, diseñada para ofrecer juegos sociales interactivos con comunicación en tiempo real.

**Incluye lo siguiente:**

- Desarrollo de aplicación móvil para Android e iOS utilizando Flutter 3.0+.
- Implementación de sistema de autenticación de usuarios mediante Firebase Authentication.
- Desarrollo de backend en tiempo real con Node.js y Socket.IO para sincronización de juegos multijugador.
- Creación de interfaz de usuario intuitiva y atractiva con soporte para hasta 8 jugadores simultáneos.
- Sistema de salas de juego con códigos de acceso y gestión de sesiones.
- Integración de múltiples juegos sociales interactivos con mecánicas variadas.
- Despliegue en Google Play Store para dispositivos Android.

Con este alcance, el proyecto se enfoca en proporcionar una herramienta de entretenimiento social que facilite la integración grupal en eventos presenciales mediante tecnología móvil moderna.
## `	`**<a name="_toc212821247"></a>[**5. Viabilidad del Sistema**](#_heading=h.7lj19pswwxxu)**
El sistema es técnicamente sólido, utilizando un stack probado basado en Flutter, Node.js y Firebase. Económicamente, presenta costos iniciales bajos y escalado según demanda. Temporalmente, el desarrollo se completó en cuatro meses con un equipo de tres personas. Operacionalmente, requiere un mantenimiento mínimo gracias a los servicios cloud, y legalmente cumple con GDPR y posee términos de servicio claros. 
## `	`**<a name="_toc212821248"></a>[**6. Información obtenida del Levantamiento de Informacion**](#_heading=h.7lj19pswwxxu)**
El público objetivo son jóvenes de 18 a 35 años, estudiantes universitarios y grupos de amigos. La información se obtuvo mediante encuestas a 200 personas, entrevistas a 15 usuarios y análisis de la competencia. El 85% conoce VASTA y el 70% juega juegos de mesa digitales. El 95% utiliza Android y el 60% se coordina mediante WhatsApp. Se identificaron oportunidades como la falta de aplicaciones locales, la demanda de juegos peruanos y la popularidad de los códigos QR post-pandemia. Entre los riesgos se encuentran la competencia internacional, la dependencia de conectividad y la curva de adopción inicial.
# <a name="_toc212821249"></a>[**III.  Análisis de Procesos**	](#_heading=h.l35cjpfq0moy)
## `	`**<a name="_toc212821250"></a>[**a) Diagrama del Proceso Actual – Diagrama de actividades**](#_heading=h.7lj19pswwxxu)**
```plantuml
@startuml
|#lightblue|Organizador|
start
:Planifica evento social;
:Revisa materiales disponibles;
if (¿Tiene todos los materiales?) then (No)
  :Sale a comprar/conseguir materiales;
  :Regresa con materiales;
else (Sí)
endif
:Prepara espacio físico;
:Organiza mesas y sillas;

|#lightgreen|Participantes|
:Llegan al evento;
:Se sientan en círculo/mesa;

|#lightblue|Organizador|
:Explica reglas del juego;
:Distribuye materiales físicos;
:Configura tablero/cartas/dados;
:Da inicio al juego;

|#lightgreen|Participantes|
repeat
  :Esperan su turno;
  :Realizan jugada manual;
  if (¿Surgió disputa?) then (Sí)
    |#lightblue|Organizador|
    :Consulta manual de reglas;
    :Aclara situación;
    |#lightgreen|Participantes|
  else (No)
  endif
  :Continúan jugando;
repeat while (¿Juego terminado?) is (No)

|#lightblue|Organizador|
:Cuenta puntos manualmente;
:Verifica resultados;
:Declara ganador oficial;
:Anota resultados en papel;

if (¿Jugar otro juego?) then (Sí)
  :Recoge materiales anteriores;
  :Prepara nuevo juego;
else (No)
  :Guarda todos los materiales;
  :Limpia espacio;
endif

|#lightgreen|Participantes|
:Se despiden del evento;
stop
@enduml
```
## `	`**<a name="_toc212821251"></a>[**b) Diagrama del Proceso Propuesto – Diagrama de actividades Inicial**](#_heading=h.7lj19pswwxxu)**
```plantuml
@startuml
|#lightblue|Usuario Organizador|
start
:Planifica evento social;
:Abre aplicación LastShot;
:Inicia sesión en la app;

|#orange|Sistema LastShot|
:Autentica credenciales;
:Carga perfil de usuario;
:Muestra pantalla principal;

|#lightblue|Usuario Organizador|
:Selecciona "Crear Juego";
if (¿Juego multijugador?) then (Sí)
  :Elige juego multijugador;
  :Configura parámetros;
else (No)
  :Elige juego solo device;
endif

|#orange|Sistema LastShot|
if (¿Es multijugador?) then (Sí)
  :Genera código único de sala;
  :Crea sala de espera;
else (No)
  :Prepara juego local;
endif

|#lightblue|Usuario Organizador|
if (¿Es multijugador?) then (Sí)
  :Comparte código de sala;
  
  |#lightgreen|Usuarios Participantes|
  :Abren aplicación LastShot;
  :Ingresan código de sala;
  
  |#orange|Sistema LastShot|
  :Valida código de sala;
  :Añade jugadores a la sala;
  :Sincroniza lista de participantes;
  
  |#lightblue|Usuario Organizador|
  :Ve lista completa de jugadores;
  :Presiona "Iniciar Juego";
else (No)
endif

|#orange|Sistema LastShot|
:Asigna turnos/roles aleatoriamente;
:Configura estado inicial del juego;
:Sincroniza con todos los dispositivos;

repeat
  |#lightgreen|Usuarios Participantes|
  :Esperan su turno;
  :Ven interfaz actualizada;
  if (¿Es su turno?) then (Sí)
    :Realizan acción en pantalla;
  else (No)
  endif
  
  |#orange|Sistema LastShot|
  :Recibe acción del jugador;
  :Valida reglas automáticamente;
  if (¿Acción válida?) then (No)
    :Envía notificación de error;
  else (Sí)
    :Actualiza estado del juego;
    :Sincroniza con todos los dispositivos;
  endif
  
  if (¿Juego terminado?) then (No)
    :Avanza al siguiente turno;
  endif
repeat while (¿Juego terminado?) is (No)

|#orange|Sistema LastShot|
:Calcula ganador automáticamente;
:Genera estadísticas del juego;
:Actualiza rankings de usuarios;

|#lightblue|Usuario Organizador|
|#lightgreen|Usuarios Participantes|
:Ven resultados en pantalla;
:Revisan estadísticas del juego;

|#lightblue|Usuario Organizador|
if (¿Jugar otro juego?) then (Sí)
  :Selecciona nuevo juego;
else (No)
  :Cierra sala de juego;
  
  |#orange|Sistema LastShot|
  :Libera recursos de la sala;
  :Guarda estadísticas;
  
@enduml
```
# <a name="_toc212821252"></a>[**IV Especificacion de Requerimientos de Software**	](#_heading=h.l35cjpfq0moy)
1) ## <a name="_toc212821253"></a>[**Cuadro de Requerimientos funcionales Inicial**](#_heading=h.7lj19pswwxxu)

|**ID**|**Nombre**|**Descripción**|**Prioridad**|
| - | - | - | - |
|**RF01**|**Administrar Perfil de Usuario**|El sistema debe permitir a los usuarios administrar su perfil (registro, login, edición de datos personales, logout)|**ALTA**|
|**RF02**|**Explorar Juegos Multijugador**|El sistema debe permitir explorar y acceder a juegos multijugador (VASTA, El Infiltrado del Bar) con funcionalidades de sala compartida|**ALTA**|
|**RF03**|**Juegos de Dispositivo Único**|El sistema debe proporcionar juegos de dispositivo único (TODITO, YO NUNCA) que funcionen offline con animaciones|**MEDIA**|
|**RF04**|**Administrar Salas de Juego**|El sistema debe permitir administrar salas de juego (crear, configurar, invitar, gestionar participantes)|**ALTA**|
|**RF05**|**Comunicación en Tiempo Real**|El sistema debe implementar comunicación en tiempo real mediante WebSockets para sincronización de estados|**ALTA**|
|**RF06**|**Generación de Códigos QR**|El sistema debe generar códigos QR para facilitar el acceso y compartir la aplicación|**MEDIA**|
|**RF07**|**Manejo de Desconexiones**|El sistema debe manejar desconexiones automáticamente y permitir reconexión sin pérdida de progreso|**ALTA**|

1) ## <a name="_toc212821254"></a>[**Cuadro de Requerimientos No funcionales**](#_heading=h.7lj19pswwxxu)

|<a name="_hlk213007886"></a>**ID**|**Nombre**|**Descripción**|**Prioridad**|
| - | - | - | - |
|**RNF01**|**Rendimiento**|Tiempo de respuesta < 200ms para acciones locales y < 500ms para sincronización de red|**ALTA**|
|**RNF02**|**Usabilidad**|Interfaz intuitiva con jerga peruana familiar y iconos universalmente reconocibles|**ALTA**|
|**RNF03**|**Compatibilidad**|Compatible con Android 6.0+ (API 23+) e iOS 10.0+, soporte para WiFi y datos móviles|**ALTA**|
|**RNF04**|**Confiabilidad**|Disponibilidad del 99.5%, recuperación automática ante fallos, manejo robusto de errores|**ALTA**|
|**RNF05**|**Seguridad**|Encriptación HTTPS/WSS, validación de entrada, autenticación JWT, cumplimiento GDPR|**ALTA**|
|**RNF06**|**Mantenibilidad**|Código modular, documentación completa, logging detallado, arquitectura escalable|**MEDIA**|
|**RNF07**|**Portabilidad**|Flutter multiplataforma, backend Node.js independiente, Firebase cloud, despliegue multi-cloud|**MEDIA**|

## <a name="_toc212821255"></a>[**c) Cuadro de Requerimientos funcionales Final**](#_heading=h.7lj19pswwxxu)

|<a name="_hlk213007853"></a>**ID**|**Nombre**|**Descripción**|**Prioridad**|
| - | - | - | - |
|**RF01**|**Administrar Perfil de Usuario**|El sistema debe permitir a los usuarios administrar su perfil (registro, login, edición de datos personales, logout)|**ALTA**|
|**RF02**|**Explorar Juegos Multijugador**|El sistema debe permitir explorar y acceder a juegos multijugador (VASTA, El Infiltrado del Bar) con funcionalidades de sala compartida|**ALTA**|
|**RF03**|**Juegos de Dispositivo Único**|El sistema debe proporcionar juegos de dispositivo único (TODITO, YO NUNCA) que funcionen offline con animaciones|**MEDIA**|
|**RF04**|**Administrar Salas de Juego**|El sistema debe permitir administrar salas de juego (crear, configurar, invitar, gestionar participantes)|**ALTA**|
|**RF05**|**Comunicación en Tiempo Real**|El sistema debe implementar comunicación en tiempo real mediante WebSockets para sincronización de estados|**ALTA**|
|**RF06**|**Generación de Códigos QR**|El sistema debe generar códigos QR para facilitar el acceso y compartir la aplicación|**MEDIA**|
|**RF07**|**Manejo de Desconexiones**|El sistema debe manejar desconexiones automáticamente y permitir reconexión sin pérdida de progreso|**ALTA**|

## `	`**<a name="_toc212821256"></a>[**d) Reglas de Negocio**](#_heading=h.7lj19pswwxxu)**
`	`Las principales reglas de negocio establecidas fueron las siguientes:

- RN-01: Todo usuario debe autenticarse con usuario y contraseña válidos para acceder al sistema.
- RN-02: Los registros de requerimientos o métricas no pueden eliminarse de forma definitiva, únicamente se podrán marcar como inactivos.
- RN-03: Todos los requerimientos funcionales deben clasificarse en prioridad Alta, Media o Baja.
- RN-04: Solo los administradores tienen permiso para gestionar usuarios y modificar configuraciones generales del sistema.
# <a name="_toc212821257"></a>[**V Fase de Desarrollo**	](#_heading=h.l35cjpfq0moy)
## `	`**<a name="_toc212821258"></a>[**1. Perfiles de Usuario**](#_heading=h.7lj19pswwxxu)**
[	](#_heading=h.7lj19pswwxxu)Se definieron los siguientes perfiles de usuario para la fase de desarrollo del sistema:

- Usuario anfitrión (creador de sala): crea sesiones de juego, genera códigos de acceso, selecciona juegos, gestiona participantes y controla el flujo de las dinámicas.
- Usuario jugador: se une a salas mediante códigos, participa en los juegos, interactúa con otros jugadores y disfruta de la experiencia social.
- Usuario casual: busca entretenimiento rápido sin configuraciones complejas, priorizando simplicidad e inmediatez.
## `	`**<a name="_toc212821259"></a>[**2. Modelo Conceptual**	](#_heading=h.7lj19pswwxxu)**

### `	`***<a name="_toc212821260"></a>[***a) Diagrama de Paquetes***](#_heading=h.7lj19pswwxxu)***

```plantuml
@startuml
!theme aws-orange
!define RECTANGLE class
allowmixing

package "CAPA DE PRESENTACIÓN" as presentation #lightblue {
  package "Mobile Application (Flutter)" as mobile_app {
    package "Core Screens" as core_screens {
      class "main.dart" as main
      class "games_screen.dart" as games_screen
      class "login_screen.dart" as login_screen
    }
    
    package "Game Categories" as game_categories {
      package "Multiplayer Games" as multiplayer_games {
        note "VASTA, Impostor, etc.\n(Futuras expansiones)" as multiplayer_note
        class "MultiplayerGameController" as multiplayer_controller
      }
      
      package "Solo Device Games" as solo_games {
        note "TODITO, YO NUNCA, etc.\n(Futuras expansiones)" as solo_note
        class "SoloGameController" as solo_controller
      }
    }
  }
}

package "CAPA DE LÓGICA DE NEGOCIO" as business #lightgreen {
  package "Services Layer" as services {
    class "socket_service.dart" as socket_service
    class "auth_service.dart" as auth_service
    class "api_service.dart" as api_service
    class "new_auth_service.dart" as new_auth_service
  }
  
  package "Data Models" as models {
    class "user_model.dart" as user_model
    class "game_model.dart" as game_model
    class "vasta_model.dart" as vasta_model
  }
}

package "CAPA DE SERVICIOS BACKEND" as backend #orange {
  package "API Layer" as api_layer {
    class "server.js" as server
    
    package "Routes" as routes {
      class "auth.js" as auth_routes
      class "games.js" as games_routes 
      class "users.js" as users_routes
    }
    
    package "Middleware" as middleware {
      class "auth.js" as auth_middleware
      class "validation.js" as validation_middleware
      class "error.js" as error_middleware
    }
  }
  
  package "Real-Time Layer" as realtime {
    class "gameHandlers.js" as game_handlers
    class "vastaHandlers.js" as vasta_handlers
  }
  
  package "Business Models" as business_models {
    class "VastaGame.js" as vasta_game_model
  }
}

package "CAPA DE INFRAESTRUCTURA" as infrastructure #lightcoral {
  package "Configuration" as config {
    class "firebase.js" as firebase_config
  }
  
  package "Cloud Services" as cloud_services {
    database "Firebase Firestore" as firestore
    component "Firebase Auth" as firebase_auth
  }
  
  package "Deployment Platform" as deployment {
    cloud "Azure App Service" as azure {
      note "Backend Node.js\nReal-time WebSockets\nRESTful APIs" as azure_note
    }
  }
}

' === RELACIONES DE DEPENDENCIA ===

' Frontend Dependencies
main --> games_screen
games_screen --> multiplayer_controller
games_screen --> solo_controller

' Game Controllers Dependencies
multiplayer_controller --> socket_service
solo_controller --> api_service

@enduml
```
### `	`***<a name="_toc212821261"></a>[***b) Diagrama de Casos de Uso***](#_heading=h.7lj19pswwxxu)***
```plantuml
@startuml
!theme aws-orange

title "Casos de Uso - Sistema LastShot\nInteracción General del Usuario"

left to right direction

actor "Usuario Jugador" as U #lightblue

package "🎯 FUNCIONALIDADES PRINCIPALES" as main_package #lightblue {
  usecase (UC01: Administrar\nPerfil de Usuario) as UC1
  usecase (UC02: Explorar\nJuegos Multijugador) as UC2
  usecase (UC03: Explorar\nJuegos de\nDispositivo Único) as UC3
  usecase (UC04: Administrar\nSala de Juego) as UC4
}

U --> UC1
U --> UC2
U --> UC3
U --> UC4

note bottom of UC2 : "Permite visualizar y unirse\na partidas multijugador"
note bottom of UC3 : "Permite acceder a juegos\npara un solo dispositivo"
note bottom of UC4 : "Crea o gestiona salas\nde juego disponibles"

@enduml
```
### `	`***<a name="_toc212821262"></a>[***c) Escenarios de Caso de Uso (narrativa)***](#_heading=h.7lj19pswwxxu)***
#### `	     `***RF-001 Administrar Perfil de Usuario***

|**Administrar Perfil de Usuario**||
| - | :- |
|**Tipo**|**Obligatorio**|
|**Autor(es)**|**Gabriela Luzkalid Gutierrez Mamani**|
|**Actores**|**Usuario jugador**|
|**Descripción**|**La aplicación móvil permite al Usuario iniciar sesión, cerrar sesión, registrarse en la aplicación y modificar su nombre de Usuario y contraseña.**|
|**Precondiciones**|**El usuario jugador debe tener descargada la aplicación y conexión a internet.**|
|`                                                      `**Narrativa de cada de uso**||
|`                   `**Acción del actor**|`                   `**Respuesta del sistema**|
|1. El usuario abre la aplicación LastShot|2. El sistema muestra la pantalla principal con opciones de login/registro|
|3. El usuario selecciona "Registrarse" e ingresa email y contraseña|4. El sistema valida los datos ingresados|
||5. El backend envía la información a Firebase Authentication|
||6. Firebase confirma la creación de la cuenta|
||7. El sistema almacena el perfil básico en Firestore|
||8. El sistema genera un token JWT para la sesión|
||9. El sistema muestra mensaje de "Registro exitoso" y redirige al lobby principal|
|10. El usuario puede editar su perfil (nombre, avatar, configuraciones)|11. El sistema actualiza los cambios en Firestore y confirma la actualización|


#### ***RF02 – Explorar juegos Multijugador***

|**Explorar juegos Multijugador**||
| - | :- |
|**Tipo**|**Obligatorio**|
|**Autor(es)**|**Mayra Fernanda Chire Ramos**|
|**Actores**|**Usuario Jugador**|
|**Descripción**|**La aplicación móvil muestra un listado de juegos de la aplicación que funcionan de manera multijugador, por lo general el jugador crea una sala en la aplicación móvil y la aplicación genera un código de ingreso que el jugador anfitrión tendrá que compartir con sus amigos para que puedan ingresar a la sala de juego.**|
|**Precondiciones**|**Iniciado sesión en la aplicación.**|
|`                                                      `**Narrativa de cada de uso**||
|`                   `**Acción del actor**|`                   `**Respuesta del sistema**|
|1. El usuario autenticado accede a la sección "Juegos Multijugador"|2. El sistema muestra la lista de juegos disponibles (VASTA, El Infiltrado del Bar)|
|3. El usuario selecciona un juego específico (ej: VASTA)|4. El sistema muestra opciones: "Crear Sala" o "Unirse a Sala"|
|5. El usuario elige "Unirse a Sala" e ingresa un código de sala|6. El sistema valida el código con el backend vía WebSocket|
||7. El backend verifica que la sala existe y tiene espacio disponible|
||8. El sistema añade al usuario a la sala y sincroniza con otros jugadores|
||9. El sistema muestra la pantalla de lobby con jugadores conectados|
||10. El sistema actualiza en tiempo real cuando otros jugadores se unen/salen|
|11. El usuario espera a que el organizador inicie la partida|12. El sistema recibe señal de inicio y carga la pantalla del juego|



#### ***RF03 – Explorar Juegos de Dispositivo Único***

|**Explorar Juegos de Dispositivo Único**||
| - | :- |
|**Tipo**|**Obligatorio**|
|**Autor(es)**|**Sebastián Nicolas Fuentes Avalos**|
|**Actores**|**Usuario Jugador**|
|**Descripción**|**La aplicación móvil muestra el listado de juegos de SOLO DEVICE, es decir, juegos diseñados para que un grupo de personas jueguen desde un solo dispositivo móvil.**|
|**Precondiciones**|**Iniciado sesión en la aplicación.**|
|`                                                      `**Narrativa de cada de uso**||
|`                   `**Acción del actor**|`                   `**Respuesta del sistema**|
|1. El usuario accede a la sección "Juegos Solo Device"|2. El sistema muestra la lista de juegos offline (TODITO, YO NUNCA)|
|3. El usuario selecciona un juego (Ejm: YO NUNCA)|4. El sistema carga el juego desde memoria local (sin conexión de red)|
||5. El sistema inicializa el mazo de 100 cartas predefinidas|
||6. El sistema muestra la primera carta con animación|
|7. El usuario toca la pantalla para ver la siguiente carta|8. El sistema reproduce animación de transición|
||9. El sistema muestra la nueva carta aleatoria del mazo|
||10. El sistema actualiza el contador de cartas mostradas|
|11. El usuario puede reiniciar el juego o cambiar de juego|12. El sistema reinicia el mazo y vuelve al estado inicial|
####


#### ***RF04 – Administrar Sala de Juego***

|**Administrar Sala de Juego**||
| - | :- |
|**Tipo**|**Obligatorio**|
|**Autor(es)**|**Sebastián Nicolas Fuentes Avalos**|
|**Actores**|**Usuario Jugador**|
|**Descripción**|**La aplicación móvil, cuando el usuario jugador selecciona un juego Multijugador, tiene la opción de compartir el código de acceso de la sala de juego y eliminar jugadores de la sala.**|
|**Precondiciones**|**Explorar Juegos Multijugador**|
|`                                                      `**Narrativa de cada de uso**||
|`                   `**Acción del actor**|`                   `**Respuesta del sistema**|
|1. El usuario selecciona "Crear Sala" desde un juego multijugado|2. El sistema solicita al backend crear una nueva sala|
||3. El backend genera un código único de 6 dígitos para la sala|
||4. El backend crea la instancia de sala en memoria con el usuario como organizador|
||5. El sistema muestra el código de sala y genera QR code automáticamente|
||6. El sistema establece conexión WebSocket para tiempo real|
|7. El usuario configura parámetros del juego (tiempo por turno, número de rondas)|8. El sistema sincroniza la configuración con todos los dispositivos conectados|
|9. El usuario comparte el código QR o código numérico con otros jugadores|10. El sistema actualiza la lista de jugadores conforme se van uniendo|
|11. El usuario inicia la partida cuando tiene suficientes jugadores|12. El backend valida que hay mínimo de jugadores requeridos|
||13. El sistema envía señal de inicio a todos los dispositivos conectados|
||14. El sistema carga la pantalla de juego para todos los participantes simultáneamente|


## [**   	](#_heading=h.l35cjpfq0moy)
1) ### <a name="_toc212821264"></a>***Diagrama de objetos***

#### <a name="_hlk213008430"></a>***Diagrama de objetos del CUS - Administrar Perfil de Usuario***

```plantuml
@startuml
!theme plain
' === ACTOR ===
actor "👤 Usuario Jugador" as Usuario

' === BOUNDARY ===
participant "🖥️ ProfileScreen\n<<Boundary>>" as Boundary #LightSkyBlue

' === CONTROL ===
participant "⚙️ AuthService\n<<Control>>" as Control1 #LightGreen
participant "🌐 ApiService\n<<Control>>" as Control2 #LightGreen
participant "🖥️ Backend Server\n<<Control>>" as Control3 #LightGreen

' === ENTITY / DATABASE ===
database "🗄️ Firebase Auth\n<<Entity>>" as Entity1 #LightCoral
database "💾 Firebase Firestore\n<<Database>>" as Entity2 #LightCoral

@enduml
```

#### ***Diagrama de objetos del CUS -  Explorar Juegos Multijugador***

```plantuml
@startuml
!theme plain
title "Objetos del Diagrama - UC02: Explorar Juegos Multijugador"

' === ACTOR ===
actor "👤 Usuario Jugador" as Usuario

' === BOUNDARY ===
participant "🖥️ MultiplayerScreen\n<<Boundary>>" as Boundary1 #LightSkyBlue
participant "🎮 GameLobby\n<<Boundary>>" as Boundary2 #LightSkyBlue

' === CONTROL ===
participant "🔌 SocketService\n<<Control>>" as Control1 #LightGreen
participant "🖥️ Backend Server\n<<Control>>" as Control2 #LightGreen
participant "⚙️ VastaGame Handler\n<<Control>>" as Control3 #LightGreen

' === ENTITY / DATABASE ===
database "💾 Game Rooms\n<<Database>>" as Entity1 #LightCoral

@enduml
```

#### ***Diagrama de objetos del CUS -  Explorar Juegos de Dispositivo Único***

```plantuml
@startuml
!theme plain
title "Objetos del Diagrama - UC03: Explorar Juegos de Dispositivo Único"

' === ACTOR ===
actor "👤 Usuario Jugador" as Usuario

' === BOUNDARY ===
participant "🖥️ SoloGameScreen\n<<Boundary>>" as Boundary #LightSkyBlue

' === CONTROL ===
participant "🎮 YoNuncaGame\n<<Control>>" as Control1 #LightGreen
participant "🃏 MazoCartas\n<<Control>>" as Control2 #LightGreen
participant "🎬 AnimationController\n<<Control>>" as Control3 #LightGreen
participant "🔊 AudioManager\n<<Control>>" as Control4 #LightGreen

' === ENTITY / DATABASE ===
database "💾 LocalStorage\n<<Database>>" as Entity1 #LightCoral

@enduml
```

#### ***Diagrama de objetos del CUS - Administrar Sala de Juego***

```plantuml
@startuml
!theme plain
title "Objetos del Diagrama - UC04: Administrar Sala de Juego"

' === ACTOR ===
actor "👑 Usuario Organizador" as Organizador

' === BOUNDARY ===
participant "🖥️ AdminScreen\n<<Boundary>>" as Boundary #LightSkyBlue

' === CONTROL ===
participant "🔌 SocketService\n<<Control>>" as Control1 #LightGreen
participant "📱 QRGenerator\n<<Control>>" as Control2 #LightGreen
participant "🖥️ Backend Server\n<<Control>>" as Control3 #LightGreen
participant "⚙️ SalaManager\n<<Control>>" as Control4 #LightGreen
participant "🎮 VastaGame\n<<Control>>" as Control5 #LightGreen

' === ENTITY / DATABASE ===
database "💾 Game Rooms\n<<Database>>" as Entity1 #LightCoral

@enduml
```
### `	`***<a name="_toc212821265"></a>b[***) Diagrama de Actividades con objetos***](#_heading=h.7lj19pswwxxu)***


#### `	     `***Diagrama de Actividades con objetos del CUS - Administrar Perfil de Usuario***

```plantuml
@startuml
' === CONFIGURACIÓN VISUAL ===
!theme plain

skinparam backgroundColor #ffffff
skinparam activity {
  BackgroundColor white
  BorderColor #666666
  FontColor #111111
  FontSize 17
}
skinparam titleFontColor #222222
skinparam titleFontSize 22
skinparam swimlaneFontColor #222222
skinparam swimlaneBorderColor #aaaaaa
skinparam swimlaneFontSize 18
skinparam arrowColor #444444
skinparam arrowThickness 2
skinparam defaultFontName Arial

' === DEFINICIÓN DE SWIMLANES ===
|#ddeeff|Usuario|
|#e6ffe6|Aplicación Mobile|
|#fffbe6|Backend Server|
|#ffe6e6|Firebase Services|

title "Diagrama de Actividades - UC01: Administrar Perfil de Usuario"

|Usuario|
start
:Abre la aplicación LastShot;

|Aplicación Mobile|
:Verifica estado de sesión;
if (¿Usuario autenticado?) then (no)
  :Muestra pantalla de login/registro;
  |Usuario|
  :Selecciona "Registrarse";
  :Ingresa email y contraseña;
  
  |Aplicación Mobile|
  :Valida formato de datos;
  :Envía datos de registro;
  
  |Backend Server|
  :Recibe solicitud de registro;
  :Valida datos del usuario;
  
  |Firebase Services|
  :Crea cuenta en Firebase Auth;
  :Genera UID único;
  :Retorna confirmación;
  
  |Backend Server|
  :Crea perfil en Firestore;
  :Genera token JWT;
  :Envía respuesta exitosa;
  
  |Aplicación Mobile|
  :Almacena token localmente;
  :Muestra mensaje "Registro exitoso";
else (sí)
  :Carga perfil del usuario;
endif

:Muestra pantalla principal del perfil;

|Usuario|
:Selecciona "Editar perfil";

|Aplicación Mobile|
:Muestra formulario de edición;

|Usuario|
:Modifica nombre y avatar;
:Confirma cambios;

|Aplicación Mobile|
:Valida nueva información;
:Envía actualización al backend;

|Backend Server|
:Procesa cambios del perfil;

|Firebase Services|
:Actualiza documento en Firestore;
:Confirma actualización;

|Backend Server|
:Retorna confirmación de cambios;

|Aplicación Mobile|
:Actualiza interfaz con nuevos datos;
:Muestra mensaje "Perfil actualizado";

|Usuario|
:Visualiza perfil actualizado;
@enduml
```



#### ***Diagrama de Actividades con objetos del CUS - Explorar Juegos Multijugador***
```plantuml
@startuml
' === CONFIGURACIÓN VISUAL ===
!theme plain

skinparam backgroundColor #ffffff
skinparam activity {
  BackgroundColor white
  BorderColor #666666
  FontColor #111111
  FontSize 17
}
skinparam titleFontColor #222222
skinparam titleFontSize 22
skinparam swimlaneFontColor #222222
skinparam swimlaneBorderColor #aaaaaa
skinparam swimlaneFontSize 18
skinparam arrowColor #444444
skinparam arrowThickness 2
skinparam defaultFontName Arial

' === DEFINICIÓN DE SWIMLANES ===
|#ddeeff|Usuario|
|#e6ffe6|Aplicación Mobile|
|#fffbe6|Backend Server|
|#ffe6e6|WebSocket Manager|

title "Diagrama de Actividades - UC02: Explorar Juegos Multijugador"

|Usuario|
start
:Accede a sección "Juegos Multijugador";

|Aplicación Mobile|
:Carga lista de juegos disponibles;
:Muestra opciones [VASTA, El Infiltrado];

|Usuario|
:Selecciona juego "VASTA";

|Aplicación Mobile|
:Muestra opciones: "Crear Sala" o "Unirse a Sala";

|Usuario|
:Selecciona "Unirse a Sala";
:Ingresa código de sala "ABC123";

|Aplicación Mobile|
:Valida formato del código;
:Establece conexión WebSocket;

|WebSocket Manager|
:Conecta con servidor backend;
:Escucha eventos de sala;

|Backend Server|
:Verifica existencia de sala "ABC123";
if (¿Sala existe?) then (no)
  :Retorna error "Sala no encontrada";
  |Aplicación Mobile|
  :Muestra mensaje de error;
  |Usuario|
  :Reintenta con nuevo código;
  stop
else (sí)
  if (¿Hay espacio disponible?) then (no)
    :Retorna error "Sala llena";
    |Aplicación Mobile|
    :Muestra mensaje "Sala completa";
    stop
  else (sí)
    :Añade usuario a la sala;
    :Actualiza lista de jugadores;
  endif
endif

|WebSocket Manager|
:Emite evento "jugador-unido";
:Sincroniza estado con todos los clientes;

|Aplicación Mobile|
:Recibe confirmación de unión;
:Navega a pantalla de lobby;
:Muestra jugadores conectados;

|Usuario|
:Visualiza lobby con otros jugadores;

note right: El usuario espera a que\nel organizador inicie la partida

|WebSocket Manager|
:Escucha evento "juego-iniciado";

if (¿Organizador inicia juego?) then (sí)
  |Backend Server|
  :Valida mínimo de jugadores;
  :Inicializa estado del juego;
  :Emite "juego-iniciado" a todos;
@enduml
```
#### ***Diagrama de Actividades con objetos del CUS - Explorar Juegos de Dispositivo Único***
```plantuml
@startuml
' === CONFIGURACIÓN VISUAL ===
!theme plain

skinparam backgroundColor #ffffff
skinparam activity {
  BackgroundColor white
  BorderColor #666666
  FontColor #111111
  FontSize 17
}
skinparam titleFontColor #222222
skinparam titleFontSize 22
skinparam swimlaneFontColor #222222
skinparam swimlaneBorderColor #aaaaaa
skinparam swimlaneFontSize 18
skinparam arrowColor #444444
skinparam arrowThickness 2
skinparam defaultFontName Arial

' === DEFINICIÓN DE SWIMLANES (RAÍLES) ===
|#ddeeff|Usuario|
|#e6ffe6|Aplicación Mobile|
|#fffbe6|Local Storage|
|#ffe6e6|Animation Engine|

title "Diagrama de Actividades - UC03: Explorar Juegos de Dispositivo Único"

|Usuario|
start
:Accede a sección "Juegos Solo Device";

|Aplicación Mobile|
:Carga juegos desde memoria local;
:Muestra lista [TODITO, YO NUNCA];

|Usuario|
:Selecciona "YO NUNCA";

|Aplicación Mobile|
:Verifica que NO requiere conexión de red;

|Local Storage|
:Carga configuración del juego;
:Recupera progreso guardado (si existe);

|Aplicación Mobile|
:Inicializa mazo de 100 cartas;
:Selecciona primera carta aleatoria;

|Animation Engine|
:Prepara animación de entrada;
:Reproduce efecto de sonido;

|Aplicación Mobile|
:Muestra carta con animación;
:Muestra contador de cartas;

|Usuario|
:Lee la carta: "Yo nunca he cantado en karaoke";

if (¿Usuario quiere siguiente carta?) then (sí)
  |Usuario|
  :Toca la pantalla para continuar;
  
  |Aplicación Mobile|
  :Marca carta actual como usada;
  
  |Local Storage|
  :Guarda progreso actualizado;
  
  |Aplicación Mobile|
  :Selecciona nueva carta aleatoria;
  :Verifica que no esté repetida;
  
  |Animation Engine|
  :Ejecuta animación de transición;
  :Reproduce sonido de cambio;
  
  |Aplicación Mobile|
  :Muestra nueva carta;
  :Actualiza contador;
  
  if (¿Quedan cartas disponibles?) then (sí)
    :Continúa con nueva carta;
  else (no)
    :Muestra mensaje "Mazo completado";
    :Ofrece opción de reiniciar;
    
    if (¿Usuario quiere reiniciar?) then (sí)
      |Local Storage|
      :Reinicia progreso del juego;
      
      |Aplicación Mobile|
      :Reinicializa mazo completo;
      :Vuelve a carta inicial;
    else (no)
@enduml
```
####
#### ***Diagrama de Actividades con objetos del CUS - Administrar Sala de Juego***



```plantuml
@startuml
' === CONFIGURACIÓN VISUAL ===
!theme plain

skinparam backgroundColor #ffffff
skinparam activity {
  BackgroundColor white
  BorderColor #666666
  FontColor #111111
  FontSize 17
}
skinparam titleFontColor #222222
skinparam titleFontSize 22
skinparam swimlaneFontColor #222222
skinparam swimlaneBorderColor #aaaaaa
skinparam swimlaneFontSize 18
skinparam arrowColor #444444
skinparam arrowThickness 2
skinparam defaultFontName Arial

' === DEFINICIÓN DE SWIMLANES (RAÍLES) ===
|#ddeeff|Usuario Organizador|
|#e6ffe6|Aplicación Mobile|
|#fffbe6|Backend Server|
|#ffe6e6|WebSocket Manager|

title "Diagrama de Actividades - UC04: Administrar Sala de Juego"

|Usuario Organizador|
start
:Selecciona "Crear Sala" desde juego VASTA;

|Aplicación Mobile|
:Valida que usuario esté autenticado;
:Envía solicitud de creación de sala;

|Backend Server|
:Genera código único de 6 dígitos;
:Crea instancia de sala en memoria;
:Asigna usuario como organizador;

|WebSocket Manager|
:Establece conexión WebSocket dedicada;
:Configura eventos de sala;

|Backend Server|
:Retorna datos de sala creada;
:Incluye código de acceso;

|Aplicación Mobile|
:Genera código QR automáticamente;
:Navega a pantalla de administración;
:Muestra código y QR code;

|Usuario Organizador|
:Configura parámetros del juego;
note right: Tiempo por turno: 5 seg\nNúmero de rondas: 10

|Aplicación Mobile|
:Valida configuración ingresada;
:Envía configuración al backend;

|Backend Server|
:Actualiza configuración de sala;
:Sincroniza cambios con todos los clientes;

|WebSocket Manager|
:Emite evento "configuracion-actualizada";

|Usuario Organizador|
:Comparte código QR con otros jugadores;

note right: Otros jugadores se van uniendo\na la sala usando el código

|WebSocket Manager|
:Recibe eventos "jugador-unido";
:Actualiza lista en tiempo real;

|Aplicación Mobile|
:Muestra jugadores que se van conectando;
:Actualiza contador de participantes;

|Usuario Organizador|
if (¿Hay mínimo 2 jugadores?) then (no)
  :Espera más jugadores;
  note right: Botón "Iniciar" deshabilitado
else (sí)
  :Botón "Iniciar Partida" se habilita;
  :Presiona "Iniciar Partida";
  
  |Aplicación Mobile|
  :Confirma inicio de juego;
  :Envía señal de inicio;
  
  |Backend Server|
  :Valida estado de sala;
  :Inicializa lógica del juego VASTA;
@enduml
```






### <a name="_heading=h.hi66ca2aej59"></a>	***<a name="_toc212821266"></a>c[***) Diagrama de Secuencia***](#_heading=h.7lj19pswwxxu)***

#### `	`***<a name="_hlk213008226"></a>     D[***iagrama de Secuencia***](#_heading=h.7lj19pswwxxu) del CUS - Administrar Perfil de Usuario***

```plantuml
@startuml
!theme plain
title "Diagrama de Secuencia - UC01: Administrar Perfil de Usuario\n(Boundary - Control - Entity - Actor)"

' === ACTORES ===
actor "👤 Usuario Jugador" as Usuario

' === BOUNDARY ===
participant "🖥️ ProfileScreen\n<<Boundary>>" as Boundary #LightSkyBlue

' === CONTROL ===
participant "⚙️ AuthService\n<<Control>>" as Control1 #LightGreen
participant "🌐 ApiService\n<<Control>>" as Control2 #LightGreen
participant "🖥️ Backend Server\n<<Control>>" as Control3 #LightGreen

' === ENTITY / DATABASE ===
database "🗄️ Firebase Auth\n<<Entity>>" as Entity1 #LightCoral
database "💾 Firebase Firestore\n<<Database>>" as Entity2 #LightCoral

' ====================================================
== Registro de Usuario ==

Usuario -> Boundary: abrirApp()
Boundary -> Control1: verificarSesion()
Control1 -> Boundary: sesionNoExiste()
Boundary -> Usuario: mostrarLoginRegistro()

Usuario -> Boundary: seleccionarRegistro()
Usuario -> Boundary: ingresarCredenciales(email, password)
Boundary -> Control1: validarDatos(email, password)
Control1 -> Boundary: datosValidos()

Boundary -> Control2: registrarUsuario(email, password)
Control2 -> Control3: POST /auth/register
Control3 -> Entity1: createUser(email, password)
Entity1 -> Control3: {uid, token}

Control3 -> Entity2: createDocument("users", userData)
Entity2 -> Control3: documentCreated()
Control3 -> Control2: {success, jwt, userData}
Control2 -> Control1: almacenarToken(jwt)
Control1 -> Boundary: registroExitoso()
Boundary -> Usuario: mostrarMensaje("Registro exitoso")

' ====================================================
== Edición de Perfil ==

Usuario -> Boundary: seleccionarEditarPerfil()
Boundary -> Control1: obtenerDatosUsuario()
Control1 -> Boundary: datosUsuario()
Boundary -> Usuario: mostrarFormularioEdicion()

Usuario -> Boundary: modificarDatos(nombre, avatar)
Usuario -> Boundary: confirmarCambios()
Boundary -> Control1: validarCambios(nuevosDatos)
Control1 -> Boundary: cambiosValidos()

Boundary -> Control2: actualizarPerfil(nuevosDatos)
Control2 -> Control3: PUT /users/profile
Control3 -> Entity2: updateDocument(userId, nuevosDatos)
Entity2 -> Control3: documentUpdated()
Control3 -> Control2: {success, updatedData}
Control2 -> Boundary: perfilActualizado()

Boundary -> Control1: actualizarDatosLocales(updatedData)
Control1 -> Boundary: datosActualizados()
Boundary -> Usuario: mostrarMensaje("Perfil actualizado")
Boundary -> Usuario: mostrarPerfilActualizado()

@enduml
```





#### ***D[***iagrama de Secuencia***](#_heading=h.7lj19pswwxxu) del CUS - Explorar Juegos Multijugador***

```plantuml
@startuml
!theme plain
title "Diagrama de Secuencia - UC02: Explorar Juegos Multijugador\n(Boundary - Control - Entity - Actor)"

' === ACTORES ===
actor "👤 Usuario Jugador" as Usuario

' === BOUNDARY ===
participant "🖥️ MultiplayerScreen\n<<Boundary>>" as Boundary1 #LightSkyBlue
participant "🎮 GameLobby\n<<Boundary>>" as Boundary2 #LightSkyBlue

' === CONTROL ===
participant "🔌 SocketService\n<<Control>>" as Control1 #LightGreen
participant "🖥️ Backend Server\n<<Control>>" as Control2 #LightGreen
participant "⚙️ VastaGame Handler\n<<Control>>" as Control3 #LightGreen

' === ENTITY / DATABASE ===
database "💾 Game Rooms\n<<Database>>" as Entity1 #LightCoral

' ====================================================
== Explorar y Seleccionar Juego ==

Usuario -> Boundary1: accederJuegosMultijugador()
Boundary1 -> Boundary1: cargarJuegosDisponibles()
Boundary1 -> Usuario: mostrarOpciones([VASTA, Infiltrado])

Usuario -> Boundary1: seleccionarJuego("VASTA")
Boundary1 -> Usuario: mostrarOpciones("Crear Sala", "Unirse")

' ====================================================
== Unirse a Sala Existente ==

Usuario -> Boundary1: seleccionarUnirse()
Usuario -> Boundary1: ingresarCodigo("ABC123")
Boundary1 -> Boundary1: validarFormatoCodigo("ABC123")

Boundary1 -> Control1: conectarWebSocket()
Control1 -> Control2: establecerConexion()
Control2 -> Control1: conexionEstablecida()
Control1 -> Boundary1: conexionConfirmada()

Boundary1 -> Control1: unirseASala("ABC123", userData)
Control1 -> Control2: emit("join-room", {codigo, usuario})

Control2 -> Entity1: verificarSala("ABC123")
alt Sala existe y tiene espacio
    Entity1 -> Control2: salaEncontrada()
    Control2 -> Entity1: añadirJugadorASala(usuario, "ABC123")
    Entity1 -> Control2: jugadorAñadido()
    Control2 -> Control1: emit("jugador-unido", salaData)
    Control2 -> Control1: emit("sala-actualizada", jugadoresList)
    
    Control1 -> Boundary1: recibirEventoUnion(salaData)
    Boundary1 -> Boundary2: navegarALobby(salaData)
    Boundary2 -> Usuario: mostrarLobby(jugadores)
    
    ' ====================================================
    == Sincronización en Tiempo Real ==
    
    loop Esperando más jugadores
        Control2 -> Control1: emit("jugador-nuevo", nuevoJugador)
        Control1 -> Boundary2: actualizarListaJugadores()
        Boundary2 -> Usuario: mostrarNuevoJugador()
    end
    
    ' ====================================================
    == Inicio del Juego ==
    
    note over Usuario: Organizador inicia el juego
    
    Control2 -> Control3: iniciarJuego("ABC123", "VASTA")
    Control3 -> Entity1: validarMinJugadores()
    Entity1 -> Control3: validacionCompleta()
    Control3 -> Control3: inicializarEstadoJuego()
    
    Control3 -> Control2: juegoInicializado(estadoInicial)
    Control2 -> Control1: emit("juego-iniciado", estadoInicial)
    
    Control1 -> Boundary2: recibirInicioJuego(estadoInicial)
    Boundary2 -> Boundary1: navegarAJuego("VASTA", estadoInicial)
    Boundary1 -> Usuario: mostrarPantallaJuego()

else Sala no existe o está llena
    Entity1 -> Control2: salaNoDisponible()
    Control2 -> Control1: emit("error-union", mensaje)
    Control1 -> Boundary1: mostrarError(mensaje)
    Boundary1 -> Usuario: mostrarMensajeError()
end

@enduml
```






#### ***D[***iagrama de Secuencia***](#_heading=h.7lj19pswwxxu) del CUS - Explorar Juegos de Dispositivo Único***

```plantuml
@startuml
!theme plain
title "Diagrama de Secuencia - UC03: Explorar Juegos de Dispositivo Único\n(Boundary - Control - Entity - Actor)"

' === ACTORES ===
actor "👤 Usuario Jugador" as Usuario

' === BOUNDARY ===
participant "🖥️ SoloGameScreen\n<<Boundary>>" as Boundary #LightSkyBlue

' === CONTROL ===
participant "🎮 YoNuncaGame\n<<Control>>" as Control1 #LightGreen
participant "🃏 MazoCartas\n<<Control>>" as Control2 #LightGreen
participant "🎬 AnimationController\n<<Control>>" as Control3 #LightGreen
participant "🔊 AudioManager\n<<Control>>" as Control4 #LightGreen

' === ENTITY / DATABASE ===
database "💾 LocalStorage\n<<Database>>" as Entity1 #LightCoral

' ====================================================
== Acceso a Juegos Solo Device ==

Usuario -> Boundary: accederJuegosSoloDevice()
Boundary -> Entity1: cargarJuegosDisponibles()
Entity1 -> Boundary: listaJuegos([TODITO, YO NUNCA])
Boundary -> Usuario: mostrarOpcionesJuego()

' ====================================================
== Selección y Inicio de YO NUNCA ==

Usuario -> Boundary: seleccionarJuego("YO NUNCA")
Boundary -> Control1: inicializarJuego()
Control1 -> Entity1: cargarProgreso("YO NUNCA")
Entity1 -> Control1: progresoGuardado(cartaActual, cartasUsadas)

Control1 -> Control2: inicializarMazo(100)
Control2 -> Control1: mazoInicializado()

Control1 -> Control2: obtenerCartaAleatoria(cartasUsadas)
Control2 -> Control1: carta(id: 13, texto: "Yo nunca he cantado en karaoke")

Control1 -> Control3: prepararAnimacionEntrada()
Control3 -> Control4: reproducirSonido("card-appear.mp3")
Control4 -> Control3: sonidoReproducido()

Control3 -> Boundary: mostrarCartaConAnimacion(carta)
Boundary -> Usuario: mostrarCarta("Yo nunca he cantado en karaoke")

' ====================================================
== Navegación entre Cartas ==

Usuario -> Boundary: tocarPantalla()
Boundary -> Control1: siguienteCarta()

Control1 -> Entity1: guardarProgreso(cartaActual: 13)
Entity1 -> Control1: progresoGuardado()

Control1 -> Control2: obtenerNuevaCarta(cartasUsadas)
Control2 -> Control2: verificarNoRepetida(cartasUsadas)
Control2 -> Control1: nuevaCarta(id: 47, texto: "Yo nunca he perdido las llaves")

Control1 -> Control3: ejecutarTransicion("slide-left")
Control3 -> Control4: reproducirSonido("card-flip.mp3")
Control4 -> Control3: sonidoReproducido()

Control3 -> Boundary: mostrarNuevaCarta(carta)
Boundary -> Usuario: mostrarCartaActualizada()

' ====================================================
== Finalización o Reinicio ==

loop Hasta completar mazo o salir
    Usuario -> Boundary: continuarJuego()
    Boundary -> Control1: procesarAccion()
end

alt Mazo completado
    Control1 -> Boundary: mostrarMensaje("¡Mazo completado!")
    Boundary -> Usuario: ofrecerReinicio()
    
    Usuario -> Boundary: seleccionarReinicio()
    Boundary -> Control1: reiniciarJuego()
    Control1 -> Entity1: limpiarProgreso()
    Entity1 -> Control1: progresoLimpiado()
    Control1 -> Control2: reinicializarMazo()
    Control2 -> Control1: mazoReiniciado()
    
else Usuario sale del juego
    Usuario -> Boundary: salirDelJuego()
    Boundary -> Entity1: guardarEstadoFinal()
    Entity1 -> Boundary: estadoGuardado()
end

@enduml
```







#### ***D[***iagrama de Secuencia***](#_heading=h.7lj19pswwxxu) del CUS - Administrar Sala de Juego***

```plantuml
@startuml
!theme plain
title "Diagrama de Secuencia - UC04: Administrar Sala de Juego\n(Boundary - Control - Entity - Actor)"

' === ACTORES ===
actor "👑 Usuario Organizador" as Organizador

' === BOUNDARY ===
participant "🖥️ AdminScreen\n<<Boundary>>" as Boundary #LightSkyBlue

' === CONTROL ===
participant "🔌 SocketService\n<<Control>>" as Control1 #LightGreen
participant "📱 QRGenerator\n<<Control>>" as Control2 #LightGreen
participant "🖥️ Backend Server\n<<Control>>" as Control3 #LightGreen
participant "⚙️ SalaManager\n<<Control>>" as Control4 #LightGreen
participant "🎮 VastaGame\n<<Control>>" as Control5 #LightGreen

' === ENTITY / DATABASE ===
database "💾 Game Rooms\n<<Database>>" as Entity1 #LightCoral

' ====================================================
== Creación de Sala ==

Organizador -> Boundary: seleccionarCrearSala("VASTA")
Boundary -> Control1: conectarWebSocket()
Control1 -> Control3: establecerConexion()
Control3 -> Control1: conexionConfirmada()

Boundary -> Control3: crearSala("VASTA", organizadorData)
Control3 -> Control4: generarCodigoUnico()
Control4 -> Control3: codigo("ABC123")

Control3 -> Control4: crearInstanciaSala(codigo, organizador)
Control4 -> Entity1: inicializarSala(configuracionDefault)
Entity1 -> Control4: salaCreada()
Control4 -> Control3: salaCreada(salaData)

Control3 -> Control1: emit("sala-creada", salaData)
Control1 -> Boundary: recibirSalaCreada(salaData)

Boundary -> Control2: generarQRCode("https://lastshot.app/join/ABC123")
Control2 -> Boundary: imagenQR()
Boundary -> Organizador: mostrarAdminPanel(codigo, qrImage)

' ====================================================
== Configuración del Juego ==

Organizador -> Boundary: modificarConfiguracion(tiempoPorTurno: 5, rondas: 10)
Boundary -> Boundary: validarConfiguracion()
Boundary -> Control1: actualizarConfiguracion(nuevaConfig)
Control1 -> Control3: emit("actualizar-config", nuevaConfig)

Control3 -> Control4: aplicarConfiguracion(salaId, nuevaConfig)
Control4 -> Entity1: actualizarConfiguracion(nuevaConfig)
Entity1 -> Control4: configuracionActualizada()
Control4 -> Control3: configuracionActualizada()
Control3 -> Control1: emit("config-actualizada", nuevaConfig)

Control1 -> Boundary: recibirConfigActualizada()
Boundary -> Organizador: mostrarConfigConfirmada()

' ====================================================
== Gestión de Jugadores ==

loop Jugadores uniéndose
    note over Control3: Otros usuarios se unen usando el código
    
    Control3 -> Control1: emit("jugador-unido", nuevoJugador)
    Control1 -> Boundary: recibirNuevoJugador(jugadorData)
    Boundary -> Boundary: actualizarListaJugadores()
    Boundary -> Organizador: mostrarNuevoJugador()
    
    Boundary -> Boundary: validarMinimosJugadores()
    alt Mínimo 2 jugadores
        Boundary -> Boundary: habilitarBotonIniciar()
    end
end

' ====================================================
== Inicio de la Partida ==

Organizador -> Boundary: presionarIniciarPartida()
Boundary -> Boundary: confirmarInicioJuego()
Boundary -> Control1: iniciarJuego(salaId)
Control1 -> Control3: emit("iniciar-juego", salaId)

Control3 -> Control4: validarEstadoSala(salaId)
Control4 -> Entity1: verificarSala(salaId)
Entity1 -> Control4: salaValidaParaIniciar()
Control4 -> Control3: salaValidaParaIniciar()

Control3 -> Control5: inicializarJuegoVasta(salaData)
Control5 -> Control5: crearEstadoInicial()
Control5 -> Control3: juegoInicializado(estadoInicial)

Control3 -> Control1: emit("juego-iniciado", estadoInicial)
Control1 -> Boundary: recibirInicioJuego(estadoInicial)
@enduml
```


<a name="_heading=h.2gtnnk8tmnnt"></a>[	](#_heading=h.7lj19pswwxxu)
### `	`***<a name="_toc212821267"></a>d[***) Diagrama de Clases***](#_heading=h.7lj19pswwxxu)***

```plantuml
@startuml
!theme aws-orange
allowmixing

title "Diagrama de Clases - Sistema LastShot\nArquitectura Completa del Sistema"

' === CAPA DE PRESENTACIÓN ===
package "Presentation Layer" #lightblue {
  
  class MainActivity {
    - context: BuildContext
    - authService: AuthService
    + initializeApp(): void
    + checkAuthStatus(): bool
    + navigateToHome(): void
  }
  
  class GamesScreen {
    - availableGames: List<GameType>
    - selectedCategory: GameCategory
    + loadMultiplayerGames(): void
    + loadSoloGames(): void
    + navigateToGame(gameType): void
  }
  
  class ProfileScreen {
    - userProfile: UserModel
    - formController: FormController
    + loadUserData(): void
    + updateProfile(userData): Future<bool>
    + validateForm(): bool
  }
  
  abstract class BaseGameScreen {
    # gameState: GameState
    # socketConnection: SocketService
    + {abstract} initializeGame(): void
    + {abstract} handleGameEvent(event): void
    + showGameResult(result): void
  }
  
  class MultiplayerGameScreen {
    - roomCode: string
    - playersList: List<Player>
    - gameConfig: GameConfiguration
    + createRoom(): Future<string>
    + joinRoom(code): Future<bool>
    + startGame(): void
  }
  
  class SoloGameScreen {
    - currentCard: Card
    - cardDeck: CardDeck
    - animationController: AnimationController
    + loadGame(): void
    + nextCard(): void
    + resetGame(): void
  }
}

' === CAPA DE LÓGICA DE NEGOCIO ===
package "Business Logic Layer" #lightgreen {
  
  class AuthService {
    - firebaseAuth: FirebaseAuth
    - currentUser: UserModel
    - jwtToken: string
    + login(email, password): Future<UserModel>
    + register(userData): Future<UserModel>
    + logout(): Future<void>
    + refreshToken(): Future<string>
  }
  
  class SocketService {
    - connection: WebSocketConnection
    - eventHandlers: Map<string, Function>
    - reconnectAttempts: int
    + connect(url): Future<bool>
    + emit(event, data): void
    + on(event, handler): void
    + disconnect(): void
    + reconnect(): Future<bool>
  }
  
  class GameService {
    - activeGames: Map<string, GameInstance>
    - gameRules: GameRules
    + createGame(type, config): GameInstance
    + joinGame(gameId, player): bool
    + processMove(gameId, move): GameState
    + endGame(gameId): GameResult
  }
  
  class ApiService {
    - baseUrl: string
    - httpClient: HttpClient
    - authHeaders: Map<string, string>
@enduml
```
# <a name="_toc212821268"></a>[**CONCLUSIONES**](#_heading=h.zhgktmo5hklg)
- El desarrollo del sistema permitió comprender e implementar de forma efectiva una arquitectura cliente-servidor moderna, donde la aplicación móvil, el backend y el gestor de WebSocket trabajan de manera coordinada para ofrecer una experiencia multijugador fluida en tiempo real.
- La integración de WebSocket resultó esencial para mantener una comunicación bidireccional constante entre los usuarios y el servidor, permitiendo sincronización instantánea de eventos como la creación de salas, uniones de jugadores y el inicio de partidas.
- La correcta división de responsabilidades entre los módulos —Aplicación Móvil, Servidor Backend y WebSocket Manager— facilitó la escalabilidad y mantenimiento del sistema, alineándose con buenas prácticas de diseño de software y principios de ingeniería orientada a componentes.
- El uso de herramientas de desarrollo actuales (como frameworks móviles, servicios en la nube y control de versiones con GitHub) permitió construir un entorno de trabajo colaborativo, seguro y fácilmente desplegable en distintos escenarios de prueba.
- Este proyecto representa una base sólida para futuros desarrollos en el ámbito de juegos en línea y aplicaciones interactivas, evidenciando la importancia de la comunicación en tiempo real y la optimización de la experiencia del usuario.

[	](#_heading=h.zhgktmo5hklg)
# <a name="_toc212821269"></a>[**RECOMENDACIONES**](#_heading=h.uzi8oymm2pix)
- Implementar un sistema de autenticación de usuarios (por ejemplo, mediante tokens JWT) para reforzar la seguridad y personalización de las sesiones de juego.
- Incorporar métricas de rendimiento y monitoreo (logs de conexión, tiempo de respuesta, número de jugadores activos) que permitan optimizar los recursos del servidor en escenarios de alta concurrencia.
- Evaluar la migración hacia una infraestructura con balanceo de carga y escalado automático, especialmente si el número de jugadores concurrentes crece significativamente.
- Documentar todas las API del backend mediante herramientas como Swagger o Postman, facilitando la comprensión y mantenimiento del sistema por parte de futuros desarrolladores.
- Considerar la integración de notificaciones push o alertas en tiempo real para mejorar la interacción entre los jugadores y aumentar la retención de usuarios en la aplicación.
- Realizar pruebas exhaustivas de seguridad y estrés (por ejemplo, simulación de múltiples conexiones WebSocket simultáneas) antes de un despliegue en producción.

# <a name="_toc212821270"></a>[**BIBLIOGRAFÍA**](#_heading=h.1kaoe2cubbyl)
# Sommerville, I. (2016). Ingeniería del Software (10ª edición). Pearson Educación.
# Pressman, R. S., & Maxim, B. R. (2019). Software Engineering: A Practitioner’s Approach. McGraw-Hill Education.
# Fowler, M. (2003). Patterns of Enterprise Application Architecture. Addison-Wesley.
# Bass, L., Clements, P., & Kazman, R. (2021). Software Architecture in Practice (4th Edition). Addison-Wesley Professional.
Tanenbaum, A. S., & Wetherall, D. J. (2011). Redes de Computadoras. Pearson Educación.[	](#_heading=h.1kaoe2cubbyl)
# <a name="_toc212821271"></a>[**WEBGRAFÍA**](#_heading=h.mkmfgmvy7hbw)
MDN Web Docs. (2024). Introducción a WebSocket.

https://developer.mozilla.org/es/docs/Web/API/WebSockets\_API

PlantUML Documentation. (2024). Activity Diagrams Syntax.

https://plantuml.com/activity-diagram

Azure App Service Documentation. (2024). Deploying Node.js and PHP apps.

https://learn.microsoft.com/azure/app-service/

Firebase Documentation. (2024). Realtime Database y Cloud Firestore.

https://firebase.google.com/docs

Socket.IO Official Docs. (2024). Real-time communication for web and mobile apps.

https://socket.io/docs/

GitHub Docs. (2024). Continuous Deployment with GitHub Actions.

https://docs.github.com/
