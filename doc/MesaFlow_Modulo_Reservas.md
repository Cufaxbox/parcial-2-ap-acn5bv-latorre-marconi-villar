# 1. Introducción

MesaFlow es una plataforma SaaS orientada a establecimientos gastronómicos que busca digitalizar distintos procesos operativos mediante herramientas web y móviles. Entre sus principales funcionalidades se encuentran la gestión de usuarios, administración de mesas, pedidos mediante códigos QR, pagos digitales y reservas.

Dentro de las funcionalidades previstas para el producto, el módulo de reservas fue identificado como una de las características de mayor valor para los establecimientos gastronómicos, ya que permite organizar la ocupación de mesas, anticipar la demanda y mejorar la experiencia de los clientes.

El presente documento se centra específicamente en la planificación y gestión del desarrollo del módulo de reservas de MesaFlow, aplicando conceptos de Administración de Proyectos y metodologías ágiles para organizar el trabajo del equipo y gestionar la evolución de los requerimientos.

---

# 2. Descripción del Proyecto

El módulo de reservas de MesaFlow tiene como objetivo permitir que los clientes puedan consultar disponibilidad y realizar reservas de mesas desde una aplicación móvil o web, mientras que los administradores de los establecimientos disponen de herramientas para gestionar reservas, configurar reglas operativas y administrar la disponibilidad del local.

El sistema contempla funcionalidades como:

* Consulta de disponibilidad de mesas.
* Registro de reservas.
* Cancelación de reservas.
* Gestión de reservas por parte del establecimiento.
* Configuración de reglas de reserva.
* Administración de mesas y capacidad disponible.

Para validar el desarrollo del módulo se utilizará una implementación funcional desarrollada sobre una arquitectura compuesta por backend, base de datos y servicios de integración, permitiendo comprobar el correcto funcionamiento de los requerimientos definidos durante el proyecto.

---

# 3. Alcance del Proyecto

El alcance del presente proyecto comprende el análisis, diseño y desarrollo del módulo de reservas de MesaFlow.

Las funcionalidades incluidas dentro del alcance inicial son:

* Consultar disponibilidad de mesas.
* Registrar reservas por parte de los clientes.
* Cancelar reservas según las políticas definidas por el establecimiento.
* Administrar reservas desde el panel de gestión.
* Configurar horarios y reglas de reserva.
* Gestionar la disponibilidad de mesas.

Quedan fuera del alcance de este proyecto las funcionalidades relacionadas con pedidos mediante QR, gestión de pagos, control de stock y reportes avanzados, ya que forman parte de otros módulos de MesaFlow.

---

# 4. Objetivo General (SMART)

Durante el relevamiento realizado en establecimientos gastronómicos se identificó que la gestión de reservas suele realizarse mediante llamadas telefónicas, mensajes instantáneos o registros manuales, generando dificultades para administrar la disponibilidad de mesas, confirmar reservas y mantener información actualizada sobre la ocupación del local.

A partir de esta necesidad se definió el desarrollo del módulo de reservas de MesaFlow, con el objetivo de digitalizar este proceso y brindar una herramienta que permita mejorar la organización operativa de los establecimientos, optimizar la experiencia de los clientes y reducir errores asociados a la gestión manual de reservas.

Desarrollar una versión funcional del módulo de reservas de MesaFlow antes de la finalización del segundo cuatrimestre de 2026, permitiendo a los clientes consultar disponibilidad y realizar reservas de manera digital, mientras que los administradores pueden gestionar mesas, horarios y reservas desde una plataforma centralizada, contribuyendo a mejorar la organización operativa de los establecimientos gastronómicos y facilitando la administración de la disponibilidad del local.

---

# 5. Resultados Esperados

Al finalizar el proyecto se espera contar con una versión funcional del módulo de reservas de MesaFlow que permita validar los principales procesos relacionados con la gestión de reservas en establecimientos gastronómicos.

Los resultados esperados son:

* Permitir a los clientes consultar disponibilidad y realizar reservas de manera digital.
* Centralizar la administración de reservas desde una única plataforma.
* Mejorar la organización de la ocupación de mesas dentro del establecimiento.
* Reducir errores asociados a la gestión manual de reservas.
* Disponer de una configuración flexible que permita adaptar las reglas de reserva a distintos establecimientos.
* Validar técnicamente la viabilidad de integrar el módulo de reservas dentro del ecosistema general de MesaFlow.
* Obtener una base funcional que pueda evolucionar en futuras versiones incorporando nuevas funcionalidades y mejoras operativas.

# 6. Análisis de Stakeholders

## 6.1 Identificación de Stakeholders

Los stakeholders son las personas o grupos que pueden influir o verse afectados por el desarrollo del módulo de reservas de MesaFlow.

La identificación de los interesados se realizó a partir del relevamiento efectuado en Cervecería DobleSentido, establecimiento utilizado como caso de estudio para la validación inicial del proyecto. Durante esta etapa se analizaron los distintos actores que intervienen en el proceso de reservas y su relación con las necesidades operativas detectadas.

Si bien MesaFlow está concebido como una plataforma SaaS orientada a múltiples establecimientos gastronómicos, los stakeholders identificados en esta sección surgen del análisis realizado sobre dicho establecimiento y constituyen la base para el diseño inicial del módulo de reservas.

Para este proyecto se identificaron los siguientes interesados principales:

### Cliente

Cantidad estimada: Múltiples usuarios.

Utilizan el módulo para consultar disponibilidad y realizar reservas de manera digital.

### Administrador del establecimiento

Cantidad estimada: 1 usuario por establecimiento.

Responsable de gestionar mesas, reservas, horarios y configuraciones operativas del sistema. Además, participa activamente en la validación de los requerimientos funcionales y necesidades del negocio.

### Empleados del establecimiento

Cantidad estimada: Variable según el establecimiento.

Personal que desarrolla sus tareas diarias dentro del establecimiento, como mozos, cocineros y personal de atención. Aportan información sobre la operatoria del negocio y los procesos relacionados con las reservas.

### Equipo de desarrollo

Cantidad estimada: 3 integrantes.

Responsable del análisis, diseño, implementación y validación técnica del módulo de reservas.

---

## 6.2 Análisis de Interesados

Cada stakeholder posee distintos niveles de interés e influencia sobre el proyecto.

| Stakeholder                       | Nivel de interés | Nivel de influencia |
| --------------------------------- | ---------------- | ------------------- |
| Cliente                           | Alta             | Media               |
| Administrador del establecimiento | Muy alta         | Alta                |
| Empleados del establecimiento     | Media            | Baja                |
| Equipo de desarrollo              | Alta             | Alta                |

El administrador del establecimiento presenta el mayor nivel de interés e influencia debido a que participa en la definición de reglas operativas, políticas de reserva y validación de funcionalidades. Por su parte, el equipo de desarrollo posee una alta influencia sobre el proyecto al ser responsable de transformar los requerimientos en una solución tecnológica funcional.

---

## 6.3 Influencia e Impacto

Se realizó una evaluación cualitativa de la influencia e impacto de cada stakeholder sobre el proyecto.

### Cliente

Influencia: Media.

Impacto: Permite validar la experiencia de uso y el proceso de reserva desde la perspectiva del usuario final.

### Administrador del establecimiento

Influencia: Alta.

Impacto: Define requerimientos funcionales, reglas operativas y valida el correcto funcionamiento del módulo de reservas.

### Empleados del establecimiento

Influencia: Baja.

Impacto: Aportan información sobre los procesos operativos y la dinámica diaria del establecimiento.

### Equipo de desarrollo

Influencia: Alta.

Impacto: Responsable de implementar la solución tecnológica y garantizar el cumplimiento de los requerimientos definidos.

### Conclusión

A partir de este análisis se determinó que el Administrador del establecimiento y el Equipo de Desarrollo representan los stakeholders con mayor influencia sobre el proyecto. El primero participa en la definición y validación de los requerimientos funcionales, mientras que el segundo es responsable de implementar la solución tecnológica.

Por su parte, los Clientes y Empleados del establecimiento aportan información relevante para validar la experiencia de uso y la operatoria diaria del negocio.

# 7. Metodología de Trabajo

## 7.1 Metodología Seleccionada

Para el desarrollo del módulo de reservas de MesaFlow se adoptó la metodología ágil Scrum. Esta metodología permite organizar el trabajo de manera iterativa e incremental, facilitando la adaptación a cambios en los requerimientos y promoviendo la entrega continua de valor durante el proyecto.

La elección de Scrum se fundamenta en la necesidad de validar funcionalidades de forma temprana, incorporar retroalimentación obtenida durante el relevamiento y gestionar posibles cambios surgidos durante el desarrollo.

Asimismo, la metodología resulta especialmente adecuada para el proyecto debido a que permite incorporar de manera ordenada las observaciones surgidas durante las validaciones funcionales realizadas con el establecimiento de referencia, favoreciendo una evolución continua del producto y una mejor adaptación a los cambios de requerimientos.

---

## 7.2 Roles y Responsabilidades

Debido al tamaño reducido del equipo, los integrantes desempeñan distintos roles dentro de la metodología Scrum sin dejar de participar activamente en las tareas de análisis, desarrollo y validación del proyecto.

### Scrum Master – Facundo Villar

Responsable de coordinar las actividades del proyecto, realizar el seguimiento de tareas, facilitar la comunicación entre los integrantes y asegurar la correcta aplicación de la metodología de trabajo.

Además, participa en el análisis funcional, diseño técnico y desarrollo de las funcionalidades del módulo de reservas.

### Product Owner – Javier Latorre

Responsable de representar las necesidades del negocio, validar requerimientos funcionales y colaborar en la definición de las reglas operativas del módulo de reservas.

Asimismo, participa en el relevamiento, análisis, desarrollo y validación de funcionalidades asociadas al proyecto.

### Equipo de Desarrollo

El equipo de desarrollo está conformado por Facundo Villar, Facundo Marconi y Javier Latorre.

Los integrantes participan en distintas actividades relacionadas con el análisis, diseño, implementación, pruebas y validación de las funcionalidades del módulo de reservas, aportando conocimientos técnicos y funcionales según su área de experiencia.

Si bien cada integrante posee responsabilidades específicas dentro del proyecto, el desarrollo de las funcionalidades se realiza de manera colaborativa, favoreciendo el intercambio de conocimientos y la participación activa en las distintas etapas del ciclo de desarrollo.

---

## 7.3 Ceremonias Scrum

Para el seguimiento del proyecto se definieron las siguientes ceremonias:

### Sprint Planning

Reunión destinada a planificar las tareas a desarrollar durante cada iteración de trabajo, definiendo objetivos, prioridades y alcance de las actividades a realizar.

### Daily Meeting

Encuentro breve destinado a revisar avances, identificar impedimentos y coordinar actividades entre los integrantes.

Debido a las características del proyecto y al tamaño reducido del equipo, estas reuniones se realizan de forma semanal o cuando la complejidad de las tareas requiere una coordinación adicional entre los integrantes.

### Sprint Review

Instancia de revisión de las funcionalidades desarrolladas y validación de los resultados obtenidos respecto de los objetivos definidos para cada iteración.

### Sprint Retrospective

Reunión orientada a identificar oportunidades de mejora en el proceso de trabajo, analizar dificultades encontradas y definir acciones correctivas para futuras iteraciones.

---

## 7.4 Herramientas Utilizadas

Para la gestión, desarrollo y seguimiento del proyecto se utilizarán las siguientes herramientas:

* GitHub para control de versiones y trazabilidad de cambios.
* Jira para la gestión del backlog, planificación y seguimiento de tareas.
* Spring Boot para el desarrollo del backend.
* MySQL para pruebas locales de base de datos.
* Azure SQL Database como entorno objetivo para persistencia de datos.
* Draw.io para la elaboración de diagramas y documentación técnica.
* Visual Studio Code e IntelliJ IDEA como entornos de desarrollo.

# 8. Análisis de Requerimientos

## 8.1 Relevamiento de Requerimientos

Los requerimientos del módulo de reservas fueron obtenidos a partir del relevamiento realizado en Cervecería DobleSentido y posteriormente refinados mediante reuniones de análisis realizadas por el equipo de trabajo.

Para documentar y mantener la trazabilidad de los requerimientos se utilizaron distintos artefactos de análisis, incluyendo Historias de Usuario (HU), Requerimientos Funcionales (RF) y Casos de Uso (CU).

Estos elementos permiten vincular las necesidades identificadas durante el relevamiento con las funcionalidades que serán implementadas durante el desarrollo del proyecto.

---

## 8.2 Historias de Usuario Principales

A partir del análisis realizado se identificaron las siguientes historias de usuario como parte del alcance inicial del módulo de reservas.

| ID     | Actor         | Descripción                                      | Prioridad |
| ------ | ------------- | ------------------------------------------------ | --------- |
| HU-012 | Cliente       | Consultar disponibilidad y realizar una reserva. | Highest   |
| HU-013 | Cliente       | Modificar o cancelar una reserva existente.      | High      |
| HU-014 | Administrador | Gestionar las reservas del establecimiento.      | Highest   |

Las historias de usuario representan las funcionalidades principales necesarias para permitir la consulta, creación, modificación y administración de reservas dentro del establecimiento.

---

## 8.3 Trazabilidad de Requerimientos

Con el objetivo de asegurar la trazabilidad entre las necesidades identificadas y las funcionalidades implementadas, se estableció la siguiente relación entre Historias de Usuario, Requerimientos Funcionales y Casos de Uso.

| Historia de Usuario | Requerimientos Funcionales | Casos de Uso   |
| ------------------- | -------------------------- | -------------- |
| HU-012              | RF-012, RF-013             | CU-010, CU-011 |
| HU-013              | RF-014, RF-015             | CU-011         |
| HU-014              | RF-016                     | CU-012         |

La utilización de esta matriz de trazabilidad permite verificar que cada requerimiento funcional se encuentra asociado a una necesidad de negocio y a uno o más casos de uso que describen su comportamiento dentro del sistema.

---

## 8.4 Documentación Complementaria

El detalle completo de las historias de usuario, requerimientos funcionales, criterios de aceptación y casos de uso se encuentra documentado en el archivo:

**Analisis_Requerimientos_Reservas_MesaFlow.xlsx**

Asimismo, como complemento al análisis realizado, se desarrollaron diagramas de casos de uso específicos para el módulo de reservas:

* Reservas – Cliente: incluye los casos de uso CU-010 y CU-011.
* Reservas – Administrador: incluye el caso de uso CU-012.

Estos permiten complementar la especificación funcional y visualizar la interacción de los distintos actores con el sistema.

La información obtenida durante esta etapa servirá como base para la construcción del backlog y la posterior planificación de tareas dentro del tablero de seguimiento del proyecto.

# 9. Tablero de Seguimiento

Para realizar el seguimiento del desarrollo del módulo de reservas se utilizó **Jira**, dentro del proyecto general **MesaFlow**.

El tablero fue configurado para organizar las tareas del proyecto mediante épicas, sprints, responsables, prioridades, estimaciones y estados de avance. De esta forma, Jira permite visualizar la planificación del trabajo, el avance de cada actividad y la distribución de responsabilidades entre los integrantes del equipo.

## 9.1 Integrantes del tablero

Se incorporaron al tablero los integrantes del equipo de trabajo:

* Facundo Villar
* Facundo Marconi
* Javier Latorre

Asimismo, se invitó al docente:

sergiod.medina@davinci.edu.ar

El tablero fue compartido con todos los integrantes del proyecto y con el docente para permitir su revisión durante la evaluación. El enlace correspondiente se incluye a continuación.

## 9.2 Organización del tablero

El tablero se organizó utilizando las épicas previamente definidas para el proyecto MesaFlow. Para esta simulación se refinaron principalmente las tareas relacionadas con el módulo de reservas.

Las épicas utilizadas fueron:

* EP-01 Gestión del Proyecto
* EP-03 Análisis y Diseño
* EP-05 Backend
* EP-06 Frontend Web
* EP-07 Mobile
* EP-08 Testing
* EP-09 Documentación

Las tareas fueron asignadas a los integrantes correspondientes, incorporando prioridades, fechas planificadas y estimaciones mediante Story Points.

## 9.3 Flujo de trabajo

El tablero utiliza un flujo simple de seguimiento:

* Pendiente
* In Review
* Done

Este flujo permite representar el estado de avance de cada item durante la simulación del desarrollo.

## 9.4 Sprints y Milestones

Para organizar el seguimiento se definieron tres Sprints. Cada Sprint fue asociado a un hito principal del proyecto, funcionando como referencia para los Milestones solicitados en la consigna.

### Sprint 1 - Planificación y Análisis

**Milestone asociado:** Milestone 1 - Planificación del módulo de reservas.

**Objetivo:** Definir las bases del módulo, sus interesados, la metodología de trabajo y los requerimientos principales.

Este Sprint incluye items relacionados con la definición del objetivo SMART, análisis de stakeholders, metodología Scrum, análisis de requerimientos y gestión inicial de riesgos.

### Sprint 2 - Desarrollo

**Milestone asociado:** Milestone 2 - Desarrollo del módulo de reservas.

**Objetivo:** Implementar las funcionalidades principales del módulo de reservas.

Este Sprint incluye items relacionados con la consulta de disponibilidad, registro de reservas, modificación y cancelación de reservas, gestión administrativa, desarrollo del panel web e implementación de funcionalidades mobile.

### Sprint 3 - Validación y Cierre

**Milestone asociado:** Milestone 3 - Validación del módulo de reservas.

**Objetivo:** Validar el funcionamiento del módulo, corregir incidencias y consolidar la documentación.

Este Sprint incluye items relacionados con la validación funcional, pruebas de integración, corrección de incidencias, actualización de documentación técnica y consolidación de evidencias del desarrollo.

Cada Sprint contiene al menos cuatro items o tarjetas asociadas, cumpliendo con la organización solicitada para los Milestones. En el tablero Jira, los items pueden visualizarse filtrando por Sprint.

## 9.5 Enlace al tablero

El tablero de seguimiento se encuentra disponible en el siguiente enlace:

https://mesaflow.atlassian.net/jira/software/projects/SCRUM/boards/1?atlOrigin=eyJpIjoiODNkMjI2YWEzMTY5NDc2Nzk4NTQxNzg0ZjdiZDUzZDMiLCJwIjoiaiJ9

## 9.6 Relación con la documentación y el versionado

La creación y configuración del tablero permite vincular la planificación realizada en la documentación con el seguimiento de las actividades en Jira.

A partir de esta versión, las tareas del tablero sirven como base para continuar con la simulación del desarrollo, la gestión de riesgos, la actualización de documentación y los futuros cambios de versión del proyecto.
