# Sistema de Gestión de Horarios

### Problemática  
La institución educativa enfrenta problemas para organizar los horarios de clases debido a que dependen de hojas de cálculo. Este método no les permite llevar un buen control sobre las horas de trabajo de los profesores ni sobre la disponibilidad de los salones. Esto provoca desorden al momento de asignar las clases, lo que genera conflictos de horarios, creando confusión y dificultad tanto para los docentes como para los encargados de la organización. En general, la manera en que se gestionan los horarios es ineficiente y causa una gran pérdida de tiempo.

### Solución  
La solución es crear una página web que permita a los responsables de la organización gestionar de manera más sencilla las horas de trabajo de los profesores. Esta herramienta permitirá asignar los salones de forma más ordenada y distribuir las clases sin que haya problemas con los horarios. Además, la página ofrecerá la opción de imprimir los horarios y enviarlos por correo electrónico o WhatsApp, asegurando que los profesores reciban sus horarios de manera rápida y clara.

### Objetivo  
El objetivo del proyecto es desarrollar una página web que haga más fácil y eficiente la organización de los horarios de clases. Con esta herramienta se eliminarán los problemas de conflictos en los horarios, mejorando la planificación y la organización. Así se evitará el uso de hojas de cálculo y se logrará que los horarios se gestionen de manera más clara y precisa, beneficiando tanto a los profesores como a los encargados de la administración.

## Levantamiento de Requerimientos

### Requerimientos Funcionales

#### RF1: Gestión de Docentes y Carga Académica
- **Historia de Usuario**: El director de programa gestiona la carga académica de los docentes según su contrato.
- **Criterios de Aceptación**: Ingreso de información de docentes, cálculo automático de horas según contrato, registro y actualización automática de la carga horaria.
- **Prioridad**: Alta

#### RF2: Gestión de Salones y Bloques
- **Historia de Usuario**: El director de programa organiza la asignación de salones por bloques evitando conflictos.
- **Criterios de Aceptación**: Asignación de salones manual o automática sin solapamientos.
- **Prioridad**: Alta

#### RF3: Asignación de Horarios y Evitación de Cruces
- **Historia de Usuario**: El director de programa asigna horarios a docentes sin cruces y sin sobrecarga horaria.
- **Criterios de Aceptación**: Asignación de horarios respetando la disponibilidad, evitando conflictos.
- **Prioridad**: Alta

#### RF4: Exportación e Impresión de Horarios
- **Historia de Usuario**: El director de programa imprime horarios en un formato estandarizado.
- **Criterios de Aceptación**: Exportación de horarios en PDF en formato imprimible.
- **Prioridad**: Media

#### RF5: Envío de Horarios por Email y WhatsApp
- **Historia de Usuario**: El director de programa envía los horarios a los docentes por correo electrónico o WhatsApp.
- **Criterios de Aceptación**: Envío automático y confirmación de recepción.
- **Prioridad**: Media


### Requerimientos No Funcionales

#### RNF1: Seguridad del Sistema
- **Descripción**: Protección de credenciales y datos sensibles.
- **Criterios de Evaluación**: Autenticación segura, cifrado, validación de permisos.
- **Prioridad**: Alta

#### RNF2: Escalabilidad y Rendimiento
- **Descripción**: Soporte a múltiples usuarios simultáneos sin pérdida de rendimiento.
- **Criterios de Evaluación**: Manejo de concurrencia, optimización de bases de datos, distribución de carga.
- **Prioridad**: Alta

#### RNF3: Interfaz de Usuario (UI/UX)
- **Descripción**: Interfaz fácil de usar, adaptable y accesible desde múltiples dispositivos.
- **Criterios de Evaluación**: Adaptación a diferentes resoluciones y dispositivos.
- **Prioridad**: Media

#### RNF4: Disponibilidad del Sistema
- **Descripción**: El sistema debe estar disponible el 99.9% del tiempo, con mantenimientos planificados fuera de horarios críticos.
- **Criterios de Evaluación**: Monitoreo y planificación de tiempos de inactividad.
- **Prioridad**: Alta

#### RNF5: Mantenimiento y Soporte
- **Descripción**: Plan de soporte y mantenimiento continuo.
- **Criterios de Evaluación**: Diagnóstico, parches, actualizaciones de software.
- **Prioridad**: Media

## Ceremonias Scrum

- **Sprint Planning**: En esta ceremonia, el equipo se enfocaría en identificar las funcionalidades clave, como la gestión de salones o la impresión de horarios, que deben ser desarrolladas. Se descomponen las tareas en subtareas más pequeñas (Ej. Implementación de API para enviar horarios por WhatsApp).

- **Daily Scrum**: Durante las reuniones diarias, los desarrolladores discuten su progreso en tareas específicas, como el diseño de la interfaz de usuario o la validación de no cruces de horarios, y se aseguran de que todo esté alineado con el objetivo del sprint.

- **Sprint Review**: El equipo presentaría el prototipo del sistema con las funcionalidades desarrolladas, como la asignación automática de horarios, a los directores de programa para recibir retroalimentación. Esto permitirá ajustes en las futuras iteraciones.

- **Sprint Retrospective**: El equipo reflexiona sobre lo que podría mejorarse en el proceso de desarrollo (por ejemplo, el uso de herramientas de gestión de tareas o la comunicación interna), y busca formas de mejorar la eficiencia para el próximo sprint.

## Actores Scrum

### Product Owner (Propietario del Producto)
- **Responsabilidades**: Define y prioriza requisitos, gestiona el backlog y toma decisiones para satisfacer necesidades del usuario.
- **Objetivo**: Maximizar el valor del producto para mejorar la gestión de horarios.

### Scrum Master
- **Responsabilidades**: Facilita el proceso Scrum, elimina obstáculos y coordina ceremonias Scrum.
- **Objetivo**: Optimizar el proceso de desarrollo y asegurar eficiencia del equipo.

### Development Team (Equipo de Desarrollo)
- **Responsabilidades**: Implementa funcionalidades, asegura calidad del producto y colabora para resolver problemas.
- **Objetivo**: Entregar incrementos funcionales de alta calidad que cumplan con los criterios del Product Owner.

## Diagramas C4

### Diagrama de Contexto (Nivel 1)
Este nivel muestra el sistema como un todo y cómo interactúa con usuarios y otros sistemas externos. Es el diagrama más abstracto y simple.

- **¿Qué incluye?** El sistema principal, los actores (usuarios o sistemas externos), y las relaciones básicas entre ellos.
- **Propósito:** Ayudar a los interesados a entender quién interactúa con el sistema y cuál es el propósito general de este.
![Contexto](Imagenes/Diagrama%20de%20Contexto.png)

### Diagrama de Contenedores (Nivel 2)
Este nivel descompone el sistema en contenedores, que son aplicaciones o servicios desplegables. Estos pueden ser aplicaciones web, bases de datos, API, etc.

- **¿Qué incluye?** Diferentes contenedores dentro del sistema, sus interacciones y los protocolos de comunicación entre ellos.
- **Propósito:** Mostrar la estructura interna de alto nivel del sistema.
![Contenedores](Imagenes/Diagrama%20de%20Contenedores.jpg)

### Diagrama de Componentes (Nivel 3)
Descompone cada contenedor en sus componentes internos. Un contenedor puede estar compuesto por varios módulos o clases.

- **¿Qué incluye?** Módulos dentro de un contenedor, sus roles y sus interacciones.
- **Propósito:** Proveer una vista más detallada de cómo están organizados los diferentes elementos de cada contenedor.
![Componentes](Imagenes/Diagrama%20de%20Componentes.jpg)

## Ver Planificación
En el siguiente enlace se presenta la planificación del proyecto utilizando Trello:
### [Trello](https://trello.com/b/fYtaCQ2X/backlog)
![Portada](Imagenes/Trello.png)

## Ver Documentación
La documentación mas detallada del proyecto en el marco de trabajo para desarrollo ágil de Software Scrum, se puede ver en el siguiente enlace redireccionado al Drive:
### [Documento](https://docs.google.com/document/d/1HuPlz14qKayrUuJ3_qlQw3R39Xpf_KNS/edit?usp=sharing&ouid=106806333699918306085&rtpof=true&sd=true)
![Portada](Imagenes/Documento.png)


