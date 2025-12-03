![](Aspose.Words.89e9c321-ad4d-49f1-a5fa-53804af75814.001.png)		Logo de mi Cliente

![Logo UPT](Images/upt.png)

**UNIVERSIDAD PRIVADA DE TACNA**

**FACULTAD DE INGENIERIA**

**Escuela Profesional de Ingeniería de Sistemas**


**Informe Final** 
**\


**Proyecto *LastShot - Plataforma de Juegos Sociales Interactivos***

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

**INDICE GENERAL**
# **Contenido**
[Antecedentes	3](#_toc213014404)

[Planteamiento del Problema	3](#_toc213014405)

[1.	Problema	3](#_toc213014406)

[2.	Justificación	3](#_toc213014407)

[3.	Alcance	3](#_toc213014408)

[Objetivos	3](#_toc213014409)

[Marco Teórico	3](#_toc213014410)

[Desarrollo de la Solución	3](#_toc213014411)

[1.	Análisis de Factibilidad (técnico, económica, operativa, social, legal, ambiental)	3](#_toc213014412)

[2.	Tecnología de Desarrollo	3](#_toc213014413)

[3.	Metodología de implementación (Documento de VISION, SRS, SAD)	3](#_toc213014414)

[Cronograma	3](#_toc213014415)

[Presupuesto	3](#_toc213014416)

[Conclusiones	3](#_toc213014417)

[Recomendaciones	3](#_toc213014418)

[Bibliografía	3](#_toc213014419)

[Anexos	3](#_toc213014420)

[Anexo 01 Informe de Factibilidad	3](#_toc213014421)

[Anex0 02   Documento de Visión	3](#_toc213014422)

[Anexo 03 Documento SRS	3](#_toc213014423)

[Anexo 04 Documento SAD	3](#_toc213014424)






# <a name="_toc213014404"></a>Antecedentes
<a name="_toc213014405"></a><a name="_hlk213007488"></a>El presente proyecto tiene como propósito desarrollar una aplicación móvil interactiva denominada LastShot, orientada a ofrecer experiencias de juegos multijugador en tiempo real. El sistema está basado en una arquitectura cliente-servidor, donde la comunicación entre los usuarios y el backend se realiza mediante el protocolo WebSocket, permitiendo la transmisión continua de información sin interrupciones y garantizando una interacción fluida durante las partidas.

La aplicación integra una interfaz móvil intuitiva desarrollada con tecnologías modernas y un servidor backend desplegado en la nube a través de Azure App Service, utilizando una pila Node.js para la lógica del servidor y la gestión de eventos. Además, se incorporan servicios de Firebase, como Authentication y Firestore, para asegurar un manejo confiable de las cuentas de usuario, almacenamiento de datos y sincronización de perfiles en línea.

El desarrollo de este sistema busca poner en práctica conceptos fundamentales de la ingeniería de software, tales como el diseño modular, la comunicación en tiempo real, la integración de servicios externos y la seguridad en aplicaciones distribuidas. Asimismo, se enfatiza el uso de herramientas de modelado como PlantUML para representar visualmente los procesos del sistema mediante diagramas de clases, actividades y secuencia, lo que facilita la comprensión de la lógica interna y las interacciones entre los componentes.

En conjunto, este proyecto constituye un ejemplo de cómo la combinación de tecnologías actuales —como Firebase, WebSocket, Azure y Node.js— puede emplearse para construir soluciones escalables, seguras y orientadas a la colaboración entre múltiples usuarios. El resultado final es una aplicación capaz de gestionar perfiles, crear y unir salas de juego, sincronizar eventos en tiempo real y ofrecer una experiencia digital moderna y dinámica.
# Planteamiento del Problema
1. ## <a name="_toc213014406"></a>Problema
<a name="_hlk212821512"></a>Actualmente, el entretenimiento social en reuniones y eventos presenta las siguientes limitaciones:

- **Dependencia de materiales físicos**: los juegos tradicionales requieren cartas, dados, tableros y otros elementos que deben comprarse, transportarse y prepararse.
- **Tiempo de preparación**: las actividades recreativas exigen planificación previa y setup, restando espontaneidad a las reuniones.
- **Limitaciones de participantes**: muchos juegos físicos están diseñados para cantidades específicas de jugadores, excluyendo a algunos asistentes.
- **Falta de variedad**: adquirir múltiples juegos físicos implica costos elevados y espacio de almacenamiento.
- **Desigualdad en la participación**: en reuniones sin estructura lúdica, algunos asistentes tienden a quedar al margen de las conversaciones.
- **Aplicaciones existentes inadecuadas**: la mayoría de apps de juegos se enfocan en entretenimiento individual o competencias online con desconocidos, perdiendo el aspecto social presencial.

Esto impide contar con una solución digital accesible, versátil y orientada específicamente al fortalecimiento de vínculos interpersonales en contextos presenciales, limitando la calidad de la experiencia social en eventos y reuniones.

1. ## <a name="_toc213014407"></a>Justificación
El proyecto LastShot surge como respuesta a la necesidad de contar con una plataforma de juegos de mesa digitales accesible, interactiva y adaptable a dispositivos móviles. Actualmente, los usuarios enfrentan limitaciones en las aplicaciones existentes, como la falta de compatibilidad con modos multijugador en tiempo real, interfaces poco intuitivas, dependencia total de conexión a Internet y ausencia de experiencias de juego que puedan disfrutarse tanto de manera individual como en grupo.

LastShot busca solventar estas deficiencias ofreciendo un sistema que permita a los jugadores crear salas, invitar amigos mediante códigos QR, jugar de manera sincronizada y mantener el progreso del juego de forma confiable, incluso en situaciones de interrupción de conectividad. La plataforma se fundamenta en tecnologías modernas (Flutter para frontend, Node.js para backend y Firebase para servicios en la nube) que garantizan rendimiento, escalabilidad y mantenimiento eficiente, asegurando que tanto usuarios nuevos como experimentados puedan disfrutar de partidas entretenidas, seguras y sin complicaciones técnicas.

Además, el proyecto apunta a generar un impacto positivo en la comunidad de jugadores peruanos, facilitando la socialización digital mediante juegos tradicionales adaptados a la era móvil y estableciendo las bases para futuras funcionalidades de monetización y expansión del catálogo de juegos.
1. ## <a name="_toc213014408"></a>Alcance
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

# <a name="_toc213014409"></a>Objetivos
# <a name="_toc213014410"></a>**Objetivo general**
Desarrollar una plataforma móvil integral de juegos sociales interactivos que facilite la integración y entretenimiento en eventos sociales, utilizando tecnologías modernas de desarrollo móvil y comunicación en tiempo real.

**Objetivos Específicos**

- Implementar un sistema de juegos multijugador en tiempo real que soporte hasta 8 jugadores simultáneos con sincronización instantánea de estados de juego.
- Desarrollar una interfaz de usuario intuitiva y atractiva utilizando Flutter que garantice una experiencia fluida en dispositivos Android e iOS.
- Establecer una arquitectura backend escalable con Node.js y Socket.IO que maneje múltiples sesiones de juego concurrentes y gestión de usuarios.
# Marco Teórico	
1\. Aplicaciones móviles y desarrollo multiplataforma

Las aplicaciones móviles se han convertido en un canal fundamental para la interacción social y el entretenimiento digital. Según Sommerville (2016), el desarrollo de software para dispositivos móviles requiere considerar aspectos como la interfaz de usuario, la experiencia de usuario y la optimización para distintos sistemas operativos. En este contexto, frameworks multiplataforma como Flutter permiten desarrollar aplicaciones con una base de código única que funciona tanto en Android como iOS, optimizando tiempo y recursos de desarrollo (Google, 2023).

2\. Juegos digitales y gamificación

Los juegos digitales fomentan la interacción, la concentración y la cooperación entre los participantes (Gee, 2003). La gamificación en entornos educativos o de socialización aumenta la motivación intrínseca de los usuarios, ofreciendo recompensas, niveles y retos que mejoran la experiencia de juego (Deterding et al., 2011). En el caso de LastShot, se implementan juegos de mesa tradicionales en formato digital, facilitando su acceso mediante dispositivos móviles y mejorando la interacción social mediante salas multijugador y códigos QR.

3\. Sistemas multijugador en tiempo real

Los juegos multijugador requieren la gestión eficiente de la comunicación en tiempo real entre clientes y servidores. Tecnologías como WebSockets permiten mantener conexiones persistentes, reduciendo la latencia y asegurando la sincronización de los estados del juego entre los usuarios (Fitzgerald, 2020). La arquitectura de LastShot utiliza Node.js para manejar eventos de juego y sincronización de salas, garantizando que todos los jugadores experimenten el mismo estado del juego al mismo tiempo.

4\. Almacenamiento en la nube y persistencia de datos

La persistencia de datos en aplicaciones móviles es crucial para guardar el progreso de los usuarios y las configuraciones del juego. Plataformas como Firebase Firestore ofrecen bases de datos NoSQL en la nube, escalables y en tiempo real, facilitando la integración con aplicaciones móviles y la gestión de usuarios y partidas (Firebase, 2023). Esto permite a LastShot mantener estadísticas de jugadores, progreso de cartas y configuraciones de sala, tanto en juegos individuales como multijugador.

5\. Experiencia de usuario (UX) y diseño de interfaces

La interfaz de usuario y la experiencia de usuario son determinantes para la aceptación de aplicaciones móviles. Nielsen (1994) destaca que la usabilidad, la claridad de la navegación y la consistencia visual son esenciales para que el usuario pueda interactuar sin dificultades. En LastShot, se prioriza un diseño mobile-first, con animaciones y retroalimentación visual que mejoran la comprensión de las acciones y aumentan la diversión durante el juego.
# <a name="_toc213014411"></a>Desarrollo de la Solución	
1. ## <a name="_toc213014412"></a>Análisis de Factibilidad (técnico, económica, operativa, social, legal, ambiental)

1. <a name="_toc52661352"></a>**Factibilidad Operativa**

***Beneficios principales:***

- *Facilitación de actividades de integración social sin requerir materiales físicos*
- *Acceso instantáneo a múltiples juegos desde cualquier smartphone*
- *Reducción de tiempo de preparación para eventos sociales*
- *Escalabilidad automática para diferentes tamaños de grupos*

***Capacidad de operación y mantenimiento:***

- *Sistema autogestionado con mínima intervención manual requerida*
- *Monitoreo automatizado de rendimiento y disponibilidad*
- *Actualizaciones remotas sin interrumpir el servicio*
- *Soporte técnico básico manejable por un desarrollador*

***Impacto en usuarios:***

- *Mejora significativa en la experiencia de eventos sociales*
- *Reducción de la barrera de entrada para participar en juegos grupales*
- *Fomento de la interacción social a través de mecánicas de juego innovadoras*

***Interesados:***

- *Organizadores de eventos sociales y corporativos*
- *Estudiantes universitarios y grupos de amigos*
- *Empresas que buscan actividades de team building*
- *Desarrolladores interesados en contribuir al proyecto open source*


1. <a name="_toc52661353"></a>**Factibilidad Legal**
- ***Ley de Protección de Datos Personales (Ley N° 29733)**: Implementación de políticas de privacidad claras y consentimiento explícito para el tratamiento de datos personales*
- ***Código de Protección y Defensa del Consumidor**: Términos y condiciones transparentes para el uso de la aplicación*
- ***Ley de Delitos Informáticos (Ley N° 30096)**: Medidas de seguridad para prevenir accesos no autorizados y proteger la integridad de los datos*
- ***Regulaciones de INDECOPI**: Cumplimiento con normas de competencia desleal y protección al consumidor digital*
- *No existen restricciones legales específicas para aplicaciones de juegos sociales en Perú*
- *Uso de licencias open source compatibles (MIT/Apache 2.0) para componentes de terceros*

1. <a name="_toc52661354"></a>**Factibilidad Social**

***Aspectos culturales peruanos:***

- *Integración de elementos culturales locales en los juegos (jerga peruana, referencias culturales)*
- *Fomento de la tradición social peruana de reuniones familiares y de amigos*
- *Contribución a la digitalización de entretenimiento social tradicional*
- *Promoción de la inclusión social mediante juegos accesibles para diferentes edades*

***Impacto social positivo:***

- *Reducción de la brecha digital en entretenimiento social*
- *Fortalecimiento de vínculos interpersonales a través de tecnología*
- *Generación de espacios de sana competencia y diversión*

1. <a name="_toc52661355"></a>**Factibilidad Ambiental**

***Impacto ambiental mínimo:***

- *Reducción del uso de materiales físicos para juegos (cartas, dados, tableros)*
- *Menor generación de residuos al digitalizar entretenimiento tradicional*
- *Eficiencia energética mediante arquitectura cloud optimizada*
- *Contribución indirecta a la sostenibilidad al reducir necesidad de producción de juegos físicos*

***Consideraciones de sostenibilidad:***

- *Uso responsable de recursos cloud para minimizar huella de carbono*
- *Optimización de código para reducir consumo de batería en dispositivos móviles*
- *Promoción de reutilización digital versus adquisición de juegos físicos*

1. ## <a name="_toc213014413"></a>Tecnología de Desarrollo

- Framework: Flutter 3.0+ para desarrollo multiplataforma
- Backend: Node.js 18+ con Express y Socket.IO para comunicación en tiempo real
- Base de datos: Firebase Firestore para datos de usuarios y MongoDB para logs de juegos
- Autenticación: Firebase Authentication con soporte para email/contraseña
- Hosting: Azure App Service o AWS EC2 para despliegue del backend
- Sistema Operativo: Linux Ubuntu 20.04 LTS para servidores
- Herramientas de desarrollo: VS Code, Android Studio, Xcode (para iOS)
# <a name="_toc213014415"></a>Cronograma
# <a name="_toc213014416"></a>Presupuesto
**Costos Generales** 

Estos costos incluyen gastos operativos básicos necesarios para la implementación del sistema.

|**Material**|**Cantidad**|**Precio Unitario**|**Total**|
| - | - | - | - |
|Paquete de Hojas Bond|1|S/ 6.00|S/ 6.00|
|Lápices|3|S/ 1.60|S/ 4.80|
|**TOTAL**| | |**S/ 10.80**|





Tabla 01: En Costos Generales se detallan las utilidades con sus cantidades y precios haciendo un total de S/10.80.

**Costos operativos durante el desarrollo** 

|***Concepto***|***Duración***|***Costo Mensual***|***Costo Final***|
| - | - | - | - |
|*Internet* |*3 meses*|*S/ 90*|*S/ 270*|
|*Energía eléctrica*|*3 meses*|*S/ 70*|*S/ 210*|
|***TOTAL***|* |* |***S/ 480***|

**Costos del ambiente**

*Se evalúan costos asociados al entorno tecnológico necesario para la implementación del sistema.*

|<p></p><p>*CONCEPTO*</p>|*DURACIÓN*|*COSTO EN $*|*COSTO EN S/.*|
| - | - | - | - |
|<p>*Azure App Service (Plan Básico B1)*</p><p></p>|*12 meses*|*$104.19*|*S/. 387.61*|
|<p>*Google Play Store (registro desarrollador)*</p><p></p>|<p>*Único*</p><p></p>|<p>*$25.00*</p><p></p>|<p>*S/. 93.00*</p><p></p>|
|***Total***|* |***$104.19***|***S/. 480.61***|

**Costos de personal**

*Estos costos corresponden al recurso humano necesario para desarrollar e implementar el sistema de gestión. Incluirán roles como:*
\*\


*●  	Desarrolladores de software para construir y mantener el sistema.*

*●  	Tester o QA para asegurar la calidad del sistema.*

*●  	Diseñador UI/UX para crear una interfaz fácil de usar para el cliente y los empleados.* 

|*ROL*|*DURACIÓN DEL PROYECTO*|*COSTO POR MES*|*COSTO FINAL*|
| - | - | - | - |
|*DevOps*|*3 meses*|*S/. 1200*|*S/. 3600*|
|*Analista de datos*|*3 meses*|*S/. 1200*|*S/. 3600*|
|*Director de proyecto*|*3 meses*|*S/. 1300*|*S/. 3900*|
|***Total***|* |* |***S/. 11100***|

**Costos totales del desarrollo del sistema** 

|CONCEPTO|COSTO SOLES|
| - | - |
|Costos Generales|S/ 10.80|
|Costos Operativos|S/. 480|
|Costos de Ambiente|S/. 387.61|
|Costos de Personal|S/. 11200|
|Total|S/. 11,100|

# <a name="_toc213014417"></a>Conclusiones

El análisis de factibilidad del proyecto LastShot indica que es altamente viable y factible desde múltiples perspectivas:

- Técnicamente, el proyecto utiliza tecnologías maduras y ampliamente adoptadas (Flutter, Node.js, Firebase), con requerimientos de hardware accesibles y una arquitectura escalable que garantiza el éxito técnico de la implementación.
- Económicamente, los costos de desarrollo e implementación son moderados (S/. 1,615.22 anuales para infraestructura) en comparación con los beneficios potenciales, especialmente considerando la escalabilidad del modelo digital.
- Operativamente, la solución ofrece beneficios claros tanto para usuarios finales como para organizadores de eventos, con una propuesta de valor sólida y un impacto positivo medible en la experiencia social.
- Legalmente, no existen barreras significativas en el contexto peruano, y el cumplimiento con las regulaciones de protección de datos y derechos del consumidor es perfectamente alcanzable.
- Social y ambientalmente, el proyecto contribuye positivamente a la digitalización del entretenimiento social tradicional, promoviendo la inclusión y reduciendo el impacto ambiental.

La convergencia de estos factores positivos, junto con la creciente adopción de soluciones móviles y la demanda de entretenimiento social digital, confirman que LastShot es un proyecto factible con alto potencial de éxito e impacto positivo en su mercado objetivo.
# <a name="_toc213014418"></a>Recomendaciones

- Iniciar con un MVP funcional que incluya 3-5 juegos sociales bien pulidos antes de expandir el catálogo, priorizando calidad sobre cantidad.
- Realizar pruebas beta con usuarios reales en eventos sociales y corporativos para validar usabilidad, identificar puntos de fricción y ajustar mecánicas de juego según feedback.
- Establecer alianzas estratégicas con organizadores de eventos, empresas de team building y universidades para promover adopción temprana y generar casos de éxito.
- Implementar sistema de analytics desde el lanzamiento para medir engagement, retención, juegos más populares y comportamiento de usuarios, informando decisiones de producto.
- Diseñar roadmap de contenido con lanzamiento periódico de nuevos juegos (mensual/bimestral) para mantener interés y retención de usuarios activos.
- Evaluar modelo de monetización ético a mediano plazo (juegos premium, personalización avanzada, versión corporativa) sin comprometer accesibilidad básica gratuita.
- Considerar programa de desarrolladores externos que permita a la comunidad contribuir con juegos personalizados siguiendo guías de diseño establecidas.
- Planificar lanzamiento en iOS una vez validado product-market fit en Android, optimizando inversión en registro de Apple Developer Program.
- Documentar lecciones aprendidas durante el desarrollo para facilitar escalabilidad del equipo y transferencia de conocimiento en futuras iteraciones.
- Preparar estrategia de marketing digital enfocada en redes sociales, influencers y boca a boca, aprovechando naturaleza viral del producto en eventos sociales.[	](#_heading=h.vax4lox2mjni)
# <a name="_toc213014419"></a>Bibliografía

Deterding, S., Dixon, D., Khaled, R., & Nacke, L. (2011). From game design elements to gamefulness: defining “gamification.” *Proceedings of the 15th International Academic MindTrek Conference: Envisioning Future Media Environments*, 9–15. <https://doi.org/10.1145/2181037.2181040>

Firebase. (2023). *Firebase Firestore documentation*. Google. <https://firebase.google.com/docs/firestore>

Fitzgerald, M. (2020). *Real-time multiplayer game architecture*. O’Reilly Media.

Gee, J. P. (2003). *What video games have to teach us about learning and literacy*. Palgrave Macmillan.

Google. (2023). *Flutter: Build apps for any screen*. <https://flutter.dev>

Nielsen, J. (1994). *Usability engineering*. Morgan Kaufmann.

Sommerville, I. (2016). *Software engineering* (10th ed.). Pearson.
# <a name="_toc213014420"></a>Anexos
## <a name="_toc213014421"></a>Anexo 01 Informe de Factibilidad
<https://github.com/UPT-FAING-EPIS/proyecto-si889-2025-ii-u3-lastshot_gutierrez_chire_fuentes/blob/main/Documentos/FD01-Informe-Factibilidad.md>

## <a name="_toc213014422"></a>Anexo 02 Documento de Visión
<https://github.com/UPT-FAING-EPIS/proyecto-si889-2025-ii-u3-lastshot_gutierrez_chire_fuentes/blob/main/Documentos/FD02-Informe-Vision.md>

## <a name="_toc213014423"></a>Anexo 03 Documento SRS (Especificación de Requerimientos)
<https://github.com/UPT-FAING-EPIS/proyecto-si889-2025-ii-u3-lastshot_gutierrez_chire_fuentes/blob/main/Documentos/FD03-Informe%20Especificaci%C3%B3n%20Requerimientos.md>

## <a name="_toc213014424"></a>Anexo 04 Documento SAD (Arquitectura de Software)
<https://github.com/UPT-FAING-EPIS/proyecto-si889-2025-ii-u3-lastshot_gutierrez_chire_fuentes/blob/main/Documentos/FD04-Informe-Arquitectura-de-Software.md>

