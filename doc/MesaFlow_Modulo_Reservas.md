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

