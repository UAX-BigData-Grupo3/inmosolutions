# Modelo actual de la organización

InmoSolutions recibe solicitudes de sus clientes para la implementación de mejoras y nuevas funcionalidades para las aplicaciones. Se alcanza un acuerdo entre los Account Managers y los ingenieros de los equipos de desarrollo para la realización de dichos mejoras y nuevas funcionalidades. Todas las solicitudes se gestionan de forma centralizada y se distribuyen a los equipos responsables de cada funcionalidad.

Los trabajos se llevan a cabo y se ponen en la cola de espera para su correspondiente release. Además, los Product Owners de la compañía suelen solicitar mejoras en las aplicaciones asociados a cambios en la estrategia del negocio o para solucionar problemas potendiales no detectados por los clientes.
Como se mencionó anteriormente, el equipo de Operaciones es una unidad cross que forma parte del área de TI. Se apoyan en la documentación elaborada por los equipos de Desarrollo para poder solucionar los posibles problemas que surjan en las aplicaciones.

El equipo de Operaciones suele además realizar diferentes tareas, como son:

- Gestionar solicitudes de variación de cuotas para los servicios.
- Aplicar cambios en esquemas de las bases de datos.
- Revisión de alertas de monitorización no críticas.
- Realización manual de liberación de Releases.
- Conectarse físicamente a la infraestructura para operativas rutinarias.
- Restablecimiento periódico de contraseñas.
- Creación/eliminación de usuarios.
- Reinicios manuales.
- Extracción manual de datos para la generación de reportes.
- Escalado manual de la infraestructura, etc.

Las aplicaciones de software están desarrolladas con tecnología Java para el backend y para el Front se utiliza Angular. Dispone de cuatro entornos: DEV, TEST, UAT y PRO Utiliza Bases de datos estructuradas, sistemas de caché, balanceo de carga y todo está montado en entornos Cloud públicas. Tiene implementado un sistema de Disaster Recovery en caso de que se presenten problemas con las aplicaciones.

Actualmente, las aplicaciones están en proceso de transformación, pasando de ser aplicaciones monolíticas que se despliegan en máquinas virtuales a ser aplicaciones Cloud Native, basadas en microservicios y en un modelo “software as a service” multi-tenant. La funcionalidad del backend estará expuesta mediante APIs que serán consumidas por las aplicaciones front. Implementará la especificación oAuth2 para la autenticación/autorización de consumo de APIs.
