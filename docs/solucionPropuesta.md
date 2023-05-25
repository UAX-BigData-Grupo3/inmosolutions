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

### Resolución de incidencias

### Gestión de incidencias

### Documentación del Postmortem

### Formación del personal

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

