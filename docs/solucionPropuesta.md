# Solución propuesta

## SLI

Un SLI basado en la latencia de solicitud podría ser el porcentaje de solicitudes que se completan en un tiempo determinado, en este caso vamos a determinar un **_95% de las solicitudes deberían completarse en menos de 400 milisegundos_**.

La tasa de error se refiere a la proporción de solicitudes que fallan en un sistema. En este caso vamos a determinar que como **_tope el 0,5% de las solicitudes deberían dar como resultado un error_**.

El throughput se refiere a la cantidad de solicitudes que un sistema puede manejar en un período de tiempo determinado. Para determinar un throughput correcto, se ha decidido aplicar que el **_número de solicitudes completadas exitosamente en un segundo debería ser de 1000_**.

La disponibilidad se refiere al tiempo durante el cual un sistema está operativo y accesible para los usuarios. Se ha decidido aplicar un **_99.9% de disponibilidad mensual_**.

La durabilidad se refiere a la capacidad de un sistema para retener y mantener los datos de manera confiable a lo largo del tiempo. Se ha decidido aplicar el **_almacenamiento confiable de un 99.9% de los datos durante 5 años_**.

## SLO

Un SLO basado en la latencia de solicitud podría establecer un objetivo específico para la latencia promedio de las solicitudes. Decidimos aplicar una **_latencia de menos de 200 milisegundos_**.

Un SLO basado en la tasa de error podría establecer un objetivo para mantener la tasa de error por debajo de cierto umbral. Se decide aplicar que **_menos del 0.7% de las solicitudes serán error_**.

Un SLO basado en el throughput podría establecer un objetivo para el rendimiento del sistema en términos de solicitudes por segundo. Se decide que por la magnitud de los servicios, se mantiene un **_minimo de throughtput de 1000 solicitudes por segundo_**.

Un SLO basado en la disponibilidad podría establecer un objetivo específico para la disponibilidad del sistema. Se decide aplicar un **_99.9% de disponibilidad anual_**.

Un SLO basado en la **_durabilidad_** podría establecer un objetivo para la durabilidad de los datos. Se decide aplicar un objetivo estandar en la industria, un **_99,999%_**

## SLA

Un SLA basado en la latencia de solicitud podría incluir un compromiso contractual en el que el proveedor del servicio se compromete a mantener una latencia de solicitud inferior a un umbral específico. Se decide aplicar un **_promedio mensual de latencia inferior a 300 milisegundos_**.

Un SLA basado en la tasa de error podría incluir un compromiso contractual en el que el proveedor del servicio se compromete a mantener una tasa de error por debajo de un valor específico. En nuestro caso, decidimos aplicar un **_promedio mensual de errores inferior al 0.5%_**.

Un SLA basado en el throughput podría incluir un compromiso contractual en el que el proveedor del servicio se compromete a proporcionar un throughput mínimo garantizado. Decidimos aplicar un **_promedio mensual de throughput no inferior a 500 solicitudes por segundo_**.

Un SLA basado en la disponibilidad podría incluir un compromiso contractual en el que el proveedor del servicio se compromete a mantener una disponibilidad mínima garantizada. Para mantener una disponibilidad adecuada proponemos un **_promedio mensual de no inferior al 99.95%_**.

Un SLA basado en la durabilidad podría incluir un compromiso contractual en el que el proveedor del servicio se compromete a mantener una durabilidad mínima garantizada. Se decide mantener un **_promedio anual de durabilidad no inferior al 99.9%_**.

## Procesos y flujos de trabajo

### Servicio de guardias

Para garantizar la disponibilidad de los servicios, es importante contar con un servicio de guardias que pueda responder rápidamente a los incidentes. Esto implica tener un equipo de guardia disponible las 24 horas del día, los 7 días de la semana, para responder a los incidentes y resolverlos de manera oportuna se propone el siguiente flujo de trabajo:

- Propósito y responsabilidades claras: Los miembros del equipo de guardia deben comprender claramente el propósito de las guardias y las responsabilidades asociadas. Esto incluye conocer las metas de disponibilidad del sistema, los acuerdos de nivel de servicio (SLA) y las expectativas de respuesta ante incidentes.

- Rotación equitativa: Las guardias deben distribuirse de manera equitativa entre los miembros del equipo. Esto asegura que todos los miembros tengan oportunidades iguales de aprender y participar en la resolución de incidentes, evitando la fatiga y el agotamiento de los miembros individuales.

- Documentación y procedimientos claros: Es esencial contar con documentación y procedimientos claros para el manejo de incidentes. Esto incluye tener guías detalladas sobre cómo responder a incidentes comunes, protocolos de comunicación y escalada, y una base de conocimientos actualizada que pueda ser referenciada durante las guardias.

- Automatización y monitoreo: Un buen servicio de guardias debe contar con herramientas de monitoreo y automatización efectivas. Esto permite detectar y responder rápidamente a los incidentes, minimizando el tiempo de respuesta y facilitando la resolución de problemas.

- Capacitación y desarrollo: Los miembros del equipo de guardia deben recibir capacitación continua para mantenerse actualizados sobre las últimas tecnologías y mejores prácticas de resolución de problemas. Esto incluye participar en ejercicios de simulación de incidentes y revisar las lecciones aprendidas después de cada guardia.

- Retroalimentación y mejora continua: Es importante establecer un ciclo de retroalimentación después de cada guardia para identificar áreas de mejora. Esto implica analizar los incidentes ocurridos, revisar los tiempos de respuesta y la efectividad de las acciones tomadas, y realizar ajustes en los procesos o procedimientos según sea necesario.

### Resolución de incidencias

Para abordar la resolución de incidencias, se propone el siguiente flujo de trabajo:

- Detección y notificación: El primer paso es detectar la incidencia lo más rápido posible, ya sea a través de sistemas de monitoreo automatizados, alertas o reportes de usuarios. Una vez detectada, es importante notificar al equipo de guardia o al equipo responsable de la resolución de incidentes.

- Respuesta inicial: El equipo debe iniciar una respuesta rápida y efectiva. Esto implica recopilar información relevante sobre la incidencia, como registros del sistema, métricas de rendimiento y cualquier dato disponible para comprender la naturaleza y el alcance del problema.

- Mitigación y estabilización: Una vez recopilada la información inicial, el equipo debe tomar medidas para mitigar los efectos de la incidencia y estabilizar el sistema. Esto puede incluir acciones como reiniciar servicios, aplicar parches, ajustar la configuración o tomar otras medidas correctivas según corresponda.

- Comunicación y coordinación: Durante todo el proceso de resolución de la incidencia, es crucial mantener una comunicación clara y efectiva. Esto implica informar a los interesados relevantes, como usuarios, clientes o partes interesadas internas, sobre el progreso de la resolución y proporcionar estimaciones realistas sobre el tiempo de recuperación.

- Investigación y análisis posterior: Una vez que se haya restablecido la estabilidad del sistema, es importante llevar a cabo una investigación exhaustiva para comprender la causa raíz de la incidencia. Esto implica analizar los registros, revisar los eventos previos y utilizar técnicas como el análisis de causa raíz (RCA) para identificar las causas subyacentes y prevenir futuros incidentes similares.

- Lecciones aprendidas y mejoras: Después de la resolución de la incidencia y la investigación posterior, el equipo debe llevar a cabo una sesión de revisión y análisis para identificar lecciones aprendidas y oportunidades de mejora. Esto puede implicar actualizar la documentación, mejorar los sistemas de monitoreo, implementar cambios en la arquitectura o procesos, o cualquier otra acción que ayude a prevenir futuros incidentes o a manejarlos de manera más efectiva.

### Gestión de incidencias

Es fundamental tener un proceso de gestión de incidencias bien definido, documentado y practicado regularmente en Inmosolutions. Esto permite una respuesta rápida, efectiva y consistente ante las incidencias, minimizando el impacto en el sistema y mejorando la confiabilidad y disponibilidad en general. Para ello, se proponen los siguientes puntos.

La gestión de incidencias, según el libro "Site Reliability Engineering" (SRE) de Google, se basa en un enfoque estructurado y sistemático. Comienza con la detección temprana de la incidencia, utilizando sistemas de monitoreo automatizados, alertas, registros de errores o reportes de usuarios.

Una vez detectada, se notifica al equipo responsable de su gestión y se inicia una investigación para comprender la naturaleza y causa raíz del problema. Esto implica recopilar información relevante, revisar registros, métricas y otros datos que ayuden a identificar qué está causando la incidencia y cómo está afectando al sistema.

Durante todo el proceso de gestión de la incidencia, es esencial mantener una comunicación clara y efectiva. Se informa a los interesados, como usuarios o partes interesadas internas, sobre el estado de la incidencia, los pasos que se están tomando y las estimaciones de tiempo para su resolución. La comunicación continua ayuda a mantener la confianza y la transparencia.

Una vez comprendida la causa raíz de la incidencia, se toman acciones para mitigar sus efectos. Esto puede implicar aplicar parches, reiniciar servicios, realizar ajustes de configuración u otras acciones correctivas necesarias para restablecer el funcionamiento normal del sistema.

Una vez mitigada la incidencia, se realiza un seguimiento para confirmar que el sistema esté nuevamente en funcionamiento normal y que el problema se haya resuelto por completo. También se lleva a cabo un análisis posterior para identificar lecciones aprendidas y oportunidades de mejora, con el objetivo de prevenir futuras incidencias similares.

### Documentación del Postmortem

#### ¿Qué es un postmortem y que partes debe tener?

En la práctica de Site Reliability Engineering (SRE) de Google, un documento postmortem (también conocido como informe de análisis de incidentes) es un documento que se crea después de que ocurre una incidencia o interrupción del servicio. Su propósito principal es analizar y documentar de manera detallada la causa raíz de la incidencia, las acciones tomadas para resolverla y las lecciones aprendidas para prevenir futuros problemas similares.

El documento postmortem es una herramienta importante en la cultura de SRE de Google, ya que fomenta la transparencia, el aprendizaje y la mejora continua. Se espera que se redacte de manera objetiva, describiendo los hechos relevantes, las decisiones tomadas y sus impactos, sin buscar culpables o sanciones. El objetivo es comprender completamente lo que sucedió y trabajar en conjunto para evitar que ocurra nuevamente.

Un documento postmortem típicamente incluirá información sobre la incidencia, como la fecha y hora de inicio, el impacto en el sistema y los usuarios, así como una cronología detallada de los eventos relevantes. También se describirá la causa raíz identificada, que puede ser una combinación de errores humanos, fallos en el diseño del sistema, problemas de configuración, entre otros. Se proporcionarán detalles sobre las acciones correctivas y preventivas tomadas, junto con recomendaciones para mejorar la resiliencia del sistema.

Además, el documento postmortem puede incluir datos cuantitativos, como el tiempo de recuperación, la pérdida de ingresos o el número de usuarios afectados, así como comentarios y retroalimentación recopilados durante la incidencia. Este documento se comparte ampliamente dentro de la organización para que otros equipos puedan aprender de la experiencia y contribuir a la mejora continua de la confiabilidad y disponibilidad del sistema.

Para Inmosolutions se propone que los siguientes apartados sean obligatorios a la hora de hacer un documento postmortem:

- Resumen ejecutivo: Este resumen proporciona una descripción concisa de la incidencia, incluyendo el impacto en el sistema, la duración y las partes afectadas. También puede incluir una evaluación inicial de la gravedad y las lecciones aprendidas más importantes.

- Cronología detallada: El documento debe proporcionar una cronología completa de los eventos que llevaron a la incidencia, desde el inicio hasta la resolución. Esto incluye detalles sobre los signos de advertencia, las acciones tomadas y cualquier cambio relevante en el sistema durante el incidente.

- Causa raíz: Se debe realizar un análisis de causa raíz exhaustivo para identificar las causas fundamentales que contribuyeron a la incidencia. Esto implica investigar y documentar los fallos en el diseño, las configuraciones incorrectas, los errores humanos u otros factores subyacentes que condujeron al incidente.

- Acciones correctivas y preventivas: El documento debe incluir las acciones tomadas para corregir la incidencia y prevenir futuros problemas similares. Esto puede incluir cambios en la arquitectura, en los procesos, en las herramientas de monitoreo o en la capacitación del personal. Es importante proporcionar una descripción clara de estas acciones y su estado de implementación.

- Lecciones aprendidas: Se deben identificar y documentar las lecciones aprendidas durante la gestión de la incidencia. Esto puede incluir recomendaciones para mejorar la resiliencia del sistema, sugerencias para optimizar la respuesta a incidentes o cualquier otro conocimiento valioso adquirido durante el proceso.

- Impacto y retroalimentación: El documento debe abordar el impacto de la incidencia en el sistema, los usuarios y otros aspectos relevantes. También es importante recopilar comentarios y retroalimentación de los equipos involucrados en la gestión de la incidencia para identificar áreas de mejora en los procesos y la colaboración.

#### Ejemplo de Postmortem

```
Resumen ejecutivo:

La incidencia ocurrida el 15 de mayo de 2023 afectó al sistema de facturación y provocó una interrupción del servicio durante aproximadamente 3 horas. El incidente afectó a los usuarios finales y generó una pérdida estimada de ingresos de $50,000. El objetivo de este documento es analizar la causa raíz de la incidencia y proponer acciones correctivas y preventivas.

Cronología detallada:

- 9:00 a.m.: Se reciben las primeras alertas de fallas en el sistema de facturación.
- 9:05 a.m.: El equipo de guardia inicia la investigación y detecta un aumento inesperado en la carga de trabajo del servidor.
- 9:15 a.m.: Se identifica un error en la configuración de escalado automático, lo que lleva a una asignación inadecuada de recursos.
- 9:30 a.m.: Se toma la decisión de desactivar el escalado automático y aumentar manualmente la capacidad del servidor.
- 10:00 a.m.: La capacidad adicional del servidor permite estabilizar el sistema y restablecer el servicio.
- 12:00 p.m.: La causa raíz se identifica como un error de configuración no detectado durante las pruebas previas a la implementación.
  Causa raíz:
  El error de configuración que condujo a la incidencia fue una regla incorrecta en el sistema de escalado automático. Durante la implementación previa, la regla no fue debidamente validada, lo que permitió que se aplicara una configuración errónea. Esto resultó en un aumento excesivo de la capacidad de los servidores, provocando inestabilidad y un rendimiento deficiente.

Acciones correctivas y preventivas:

Se realizará una revisión exhaustiva del proceso de validación de cambios en la configuración, incluyendo pruebas rigurosas y validación por parte de múltiples miembros del equipo antes de su implementación.
Se implementará una alerta adicional para monitorear el rendimiento del escalado automático y detectar anomalías en la capacidad de los servidores.
Se llevará a cabo una sesión de capacitación para todo el equipo de operaciones, destacando la importancia de la validación adecuada de la configuración y las mejores prácticas para el manejo de situaciones similares.

Lecciones aprendidas:

La importancia de una validación rigurosa de los cambios de configuración antes de su implementación.
La necesidad de contar con alertas y monitoreo adecuados para detectar anomalías en el rendimiento del sistema.
La importancia de la comunicación clara y rápida con los interesados durante una incidencia para mantener la confianza del cliente.
Impacto y retroalimentación:
La incidencia causó una interrupción significativa del servicio, generando una pérdida de ingresos y afectando la satisfacción del cliente. Se recopilaron comentarios de los usuarios afectados y se tomarán medidas para mejorar la comunicación durante futuras incidencias y minimizar el impacto en el negocio.

Este documento de postmortem se compartirá ampliamente dentro del equipo de operaciones y se tomarán las acciones necesarias para implementar las correcciones y mejorar la resiliencia del sistema.

```

### Formación del personal

En Inmosolutions consideramos que además de adquirir conocimientos teóricos, la formación en SRE también implica experiencia práctica significativa, como participación en proyectos reales, trabajo en entornos operativos y exposición a situaciones reales de incidencias. Esto contribuye al desarrollo efectivo de profesionales de SRE. Para ello se proponen los siguientes apartados núcleo para la formación del personal:

- Fundamentos de ingeniería de confiabilidad: Los profesionales de SRE deben comprender los principios fundamentales de la ingeniería de confiabilidad, como disponibilidad, escalabilidad, tolerancia a fallos, monitoreo, resiliencia y gestión de incidencias.

- Conocimientos técnicos profundos: Los ingenieros de SRE deben tener un conocimiento profundo de los sistemas que gestionan, incluyendo lenguajes de programación, sistemas operativos, redes, almacenamiento, bases de datos y tecnologías específicas del dominio.

- Automatización y desarrollo de software: Los profesionales de SRE deben tener habilidades en desarrollo de software y automatización de tareas, incluyendo programación, scripting, desarrollo de herramientas, infraestructura como código y prácticas ágiles de desarrollo.

- Gestión de incidencias y respuesta a emergencias: La formación en gestión de incidencias es esencial para los ingenieros de SRE, incluyendo técnicas de identificación, notificación, escalado, investigación, resolución y análisis posterior a la incidencia.

- Habilidades de colaboración y comunicación: Los profesionales de SRE deben ser capaces de colaborar eficazmente con otros equipos y partes interesadas, incluyendo habilidades de comunicación clara, trabajo en equipo, resolución de conflictos y negociación.

- Cultura de aprendizaje continuo: Se valora la actitud de aprendizaje continuo en SRE, donde los ingenieros deben mantenerse actualizados con las últimas tecnologías, prácticas y enfoques, estar abiertos a aprender de los errores y adaptarse rápidamente a los cambios.

## Skills necesarios

## Tareas por roles

## Monitorización

## Automatización

## Stack tecnológico

Se propone el siguiente stack tecnológico para implementar la unidad Devops:

**_Control de versiones_**:
**_GitHub_**: Es una plataforma de control de versiones distribuido basado en Git. Permite almacenar y gestionar el código fuente de manera colaborativa, facilitando la colaboración entre desarrolladores y el seguimiento de cambios en el código. 
GitHub se puede utilizar como repositorio de código para almacenar y gestionar el código fuente de las aplicaciones de InmoSolutions. Los equipos de desarrollo pueden colaborar, revisar y realizar seguimiento de los cambios en el código a través de ramas, pull requests y comentarios.

**_Gestión de la nube:_**
**_Azure:_** Es una plataforma de servicios en la nube de Microsoft. Proporciona una amplia gama de servicios, como infraestructura escalable, almacenamiento, bases de datos, servicios de aplicaciones, redes y más. Azure se utiliza para alojar y desplegar las aplicaciones de InmoSolutions en la nube. 
Se puede utilizar para implementar y hospedar las aplicaciones de InmoSolutions en entornos cloud. Ofrece servicios como máquinas virtuales, bases de datos, servicios de aplicaciones, almacenamiento, entre otros, que son necesarios para desplegar y escalar las aplicaciones de forma segura y confiable.

**_Gestión de dependencias y construcción:_**
**_Maven:_** Es una herramienta de gestión de dependencias y construcción de proyectos en Java. Maven permite definir y gestionar las dependencias del proyecto a través de un archivo de configuración (pom.xml). También automatiza el proceso de compilación, prueba y generación de artefactos, lo que facilita la construcción de proyectos de forma coherente y reproducible.
Maven se puede utilizar para construir, gestionar dependencias y generar los artefactos de las aplicaciones de InmoSolutions. Permite definir y mantener un proyecto de manera estructurada, gestionar las dependencias de bibliotecas y automatizar el proceso de compilación y empaquetado de las aplicaciones.

**_Integración continua y entrega continua:_**
**_Jenkins:_** Es una herramienta de automatización de integración continua y entrega continua (CI/CD). Jenkins permite la configuración de pipelines de construcción y despliegue, donde se pueden definir pasos y tareas automatizadas, como la compilación del código, ejecución de pruebas, análisis estático, creación de artefactos y despliegue en entornos de desarrollo, prueba y producción. Jenkins se puede utilizar para configurar y ejecutar pipelines de integración continua que automatizan las tareas de compilación, prueba y despliegue de las aplicaciones de InmoSolutions. Facilita la detección temprana de errores, garantiza la calidad del código y agiliza la entrega de nuevas funcionalidades al automatizar los procesos de construcción y despliegue.

**_Contenedorización y despliegue:_**
**_Tomcat:_** Es un servidor de aplicaciones web Java que permite ejecutar y desplegar aplicaciones basadas en tecnología Java Servlet y JavaServer Pages (JSP). Tomcat proporciona un entorno de ejecución para aplicaciones Java y permite el despliegue sencillo de aplicaciones web.
Tomcat se puede utilizar como servidor de aplicaciones para implementar y ejecutar las aplicaciones backend de InmoSolutions desarrolladas con tecnología Java. Proporciona un entorno de ejecución estable y escalable para las aplicaciones web y permite gestionar el despliegue y la administración de las aplicaciones en los diferentes entornos.

**_Gestión de artefactos:_**
**_Artifactory:_** Es un repositorio de artefactos empresarial que permite almacenar y gestionar de forma segura los artefactos generados durante el proceso de construcción de software. Artifactory es utilizado para gestionar las dependencias de las aplicaciones, como bibliotecas, JAR, WAR, Docker images, y garantizar su disponibilidad y trazabilidad.
 Artifactory se puede utilizar como repositorio de artefactos para almacenar y gestionar los artefactos generados por Maven durante el proceso de construcción de las aplicaciones de InmoSolutions. Proporciona un lugar centralizado para almacenar y distribuir los artefactos, lo que facilita la gestión de versiones y la reutilización de componentes.

**_Análisis estático de código:_**
**_SonarQube:_** Es una plataforma de análisis estático de código que proporciona métricas y análisis detallados sobre la calidad del código. SonarQube permite identificar problemas de código, vulnerabilidades, duplicaciones y malas prácticas. Ayuda a mantener un alto nivel de calidad en el código fuente y promueve buenas prácticas de desarrollo.
SonarQube se puede utilizar para analizar y evaluar la calidad del código de las aplicaciones de InmoSolutions. Permite identificar y corregir problemas de código, mantener un estándar de calidad en el desarrollo y mejorar la seguridad y el rendimiento de las aplicaciones.

Estas tecnologías se complementan entre sí para permitir la automatización de procesos, el despliegue ágil y confiable de aplicaciones, el control de calidad del código y la gestión eficiente de dependencias y artefactos. La combinación de estas herramientas en el stack tecnológico propuesto proporciona una base sólida para implementar prácticas de DevOps en InmoSolutions y lograr los objetivos establecidos.

