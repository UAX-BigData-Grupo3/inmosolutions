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
