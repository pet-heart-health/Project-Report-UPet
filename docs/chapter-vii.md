# Capítulo VII: DevOps Practices
## 7.1. Continuous Integration

### 7.1.1. Tools and Practices

Como parte de nuestras prácticas, aplicamos metodologías como el **Test Driven Development (TDD)** y el **Behavior Driven Development (BDD)**.  
Con **TDD**, adoptamos un enfoque iterativo en el que primero se definen pruebas automatizadas antes de escribir el código correspondiente, lo que nos permite desarrollar funcionalidades más confiables y con una base sólida de validación.  
**BDD**, en cambio, se enfoca en describir el comportamiento esperado del sistema en términos comprensibles para todas las partes involucradas, promoviendo así una mejor colaboración entre perfiles técnicos y no técnicos.

El uso combinado de estas metodologías, junto con herramientas especializadas, fortalece la calidad del software, reduce errores en etapas posteriores y agiliza los ciclos de entrega. Entre las herramientas que empleamos con mayor frecuencia se encuentran:

| Herramienta | Tipo | Descripción | Propósito |
|-------------|------|-------------|-----------|
|![img](https://cucumber.io/img/logo.svg) **Cucumber**   | BDD  | Cucumber es una herramienta de pruebas que permite escribir pruebas en lenguaje natural, facilitando la colaboración entre desarrolladores, testers y stakeholders. Utiliza el formato Gherkin para describir el comportamiento esperado de la aplicación. | Permitir a los equipos de desarrollo y negocio escribir pruebas de comportamiento en un formato fácil de entender y ejecutar. |
|![](https://miro.medium.com/v2/resize:fit:1126/1*2SvCLR90HHlzFPyIEMD2xg.png) **unittest** | TDD  | `unittest` es el framework de pruebas unitarias estándar de Python. Permite realizar pruebas de unidades de código, asegurando que cada componente del sistema funcione correctamente de manera aislada. | Validar el comportamiento de las unidades de código en fases tempranas de desarrollo mediante pruebas unitarias e integrales. |


### 7.1.2. Build & Test Suite Pipeline Components
<!-- TODO: Se debe agregar imágenes de los archivos de test --> 

## 7.2. Continuous Delivery
El objetivo de la **Entrega Continua** es automatizar la integración y pruebas del código, asegurando que siempre esté listo para ser desplegado cuando se necesite, pero sin realizar el despliegue de forma automática.

### 7.2.1. Tools and Practices

#### Herramientas:
- **GitHub Actions y GitLab CI/CD**: Herramientas que permiten automatizar el pipeline de **CI/CD**. En el contexto de **Continuos integration**, podemos configurar una etapa en la que el despliegue final sea realizado manualmente. Esto asegura que el software está listo, pero el despliegue no es automático, ya que esa es la función de la **Continuos deployment**.
- **Trello**: Utilizado para gestionar el proceso de aprobación del despliegue. Se puede configurar un sistema en el que, tras la validación del pipeline, un administrador o gerente del proyecto debe revisar y aprobar el despliegue a producción.
- **Docker**: Docker se usa para contenerizar la aplicación, asegurando que el entorno de desarrollo y producción sean consistentes. Esto facilita la validación del código en entornos intermedios, como **staging**.

#### Prácticas:

- **Desarrollo basado en ramas (Feature Branching) y Merge Requests:** Las nuevas características se implementan en ramas separadas. Al finalizar, se integran a la rama principal mediante merge requests. A diferencia del Despliegue Continuo, aquí se requiere una aprobación manual después de que el código ha sido probado y fusionado.

- **Pruebas en entorno staging:** Se utilizan entornos de staging que simulan las condiciones reales de producción. Esto permite detectar errores antes del despliegue final y facilita realizar pruebas funcionales, exploratorias o con participación de usuarios clave.

- **Despliegue controlado:** Aunque el pipeline automatiza la preparación del entorno para el despliegue, la acción final de publicar los cambios se hace de forma manual. Esto es esencial en Continuous Delivery para mantener el control y mitigar riesgos.

- **Validación manual:** El proceso requiere la aprobación de un responsable antes de que el código pase a producción. Este paso puede involucrar revisión de logs, verificación de comportamiento esperado o cumplimiento de requisitos específicos del negocio.

- **Rollback manual:** Aunque algunos pipelines incluyen scripts para revertir cambios automáticamente, en entornos de Continuous Delivery el rollback suele ser una operación deliberada y manual, ejecutada por el equipo de desarrollo u operaciones si algo falla tras el despliegue.

- **Automatización de procesos repetitivos:** Se busca automatizar todo lo posible dentro del flujo de trabajo —desde la integración de código, pruebas unitarias, hasta la creación de entornos— con el objetivo de tener una pipeline robusta y confiable.

- **Cambios siempre listos para release:** Cada modificación en el código debe estar acompañada de documentación técnica, registros para auditoría y material para usuarios finales, de forma que cualquier versión aprobada esté lista para producción.

- **Evitar ramas largas:** Siguiendo el enfoque de trunk-based development, se promueve la integración frecuente en la rama principal, lo cual reduce conflictos y acelera la retroalimentación sobre errores.

- **Sin tiempo de inactividad (No Downtime):** Las actualizaciones se prueban primero en staging o mediante técnicas como canary releases para garantizar que no interrumpan la disponibilidad del sistema.

- **Release por bloque funcional:** Si dos módulos deben probarse juntos, deben también desplegarse juntos para asegurar su compatibilidad. En caso contrario, deben desacoplarse completamente.


### 7.2.2. Stages Deployment Pipeline Components

- **Integración Continua (CI)**: Cada commit en el repositorio de desarrollo activa automáticamente una serie de pruebas y validaciones. El objetivo es detectar errores de forma temprana y asegurar que el código está en condiciones de ser liberado.

- **Validación en Staging**: Esta etapa replica las condiciones de producción en un entorno aislado. Permite ejecutar pruebas manuales, de carga o de seguridad antes del despliegue final, detectando problemas que no se manifiestan en ambientes de desarrollo.

- **Despliegue con aprobación**: Aunque el código ya ha sido validado técnicamente, el paso a producción se realiza únicamente con la aprobación explícita de un responsable, lo que añade una capa de supervisión crítica.

- **Monitoreo continuo y retroalimentación**: Una vez que se despliega el código, herramientas de monitoreo evalúan el impacto en el rendimiento y en la experiencia de usuario. Esta retroalimentación se usa para mejorar versiones futuras y actuar rápidamente ante cualquier anomalía.

- **Etapa de aprobación final (Manual Gate)**: El pipeline se detiene antes del paso de producción, esperando que un miembro del equipo lo autorice. Esta práctica es fundamental en **Continuous Delivery**, pues combina automatización con control humano.


## 7.3. Continuous Deployment

El objetivo del Despliegue Continuo es automatizar por completo todo el flujo desde la integración del código hasta su despliegue en producción, de modo que cualquier cambio que pase todas las pruebas sea liberado automáticamente sin necesidad de aprobación manual.

### 7.3.1. Tools and Practices

#### Tools

 - **GitHub Actions**: Se utiliza para automatizar el pipeline de integración y entrega continua (CI/CD), ejecutando pruebas automatizadas, validaciones y despliegues a entornos como desarrollo, staging y producción.

- **Docker**: La aplicación FastAPI es completamente containerizada. Esto asegura que el comportamiento del sistema sea el mismo en cualquier entorno (local, testing o producción), reduciendo errores por diferencias de configuración o dependencias.

- **Aiven**: Gestiona el entorno de base de datos MySQL con soporte para despliegues automatizados, migraciones estructuradas y copias de seguridad.

- **Render**: Plataforma utilizada para desplegar automáticamente el backend en FastAPI, ofreciendo escalabilidad, monitoreo y reinicios automáticos ante fallos.

- **Firebase Hosting**: Se emplea para el despliegue automático y seguro del frontend desarrollado en Angular.

#### Prácticas
- **Desarrollo guiado por pruebas (TDD)**: Antes de desarrollar nuevas funcionalidades, se definen especificaciones y se escriben pruebas automatizadas para validar el comportamiento esperado. El código solo se implementa una vez que estas pruebas están listas, asegurando calidad desde el inicio.

- **Feature Branching con despliegue basado en commits**: Cada nueva funcionalidad se desarrolla en una rama separada. Al fusionarse a la rama `develop`, se activa automáticamente el pipeline que ejecuta pruebas y despliega los cambios al entorno correspondiente. Esto permite mantener un flujo ágil, automatizado y trazable.

- **Validación en entorno staging**: Antes de llegar a producción, los cambios pasan por un entorno intermedio que replica la configuración de producción. Allí se realizan pruebas manuales, de carga y de seguridad para detectar errores que no se presentan en desarrollo.

- **Despliegue con aprobación manual (Manual Gate)**: A pesar de que las pruebas hayan sido exitosas, la promoción a producción requiere la aprobación explícita de un miembro del equipo. Esto añade una capa de supervisión responsable.

- **Despliegue exclusivamente a través del pipeline**: El pipeline CI/CD es el único medio autorizado para desplegar código. Se prohíbe cualquier modificación manual directa en el entorno de producción, lo que evita inconsistencias y mantiene la integridad del historial de cambios.

- **Rollback automático**: Ante fallos detectados post-despliegue, el pipeline está preparado para revertir automáticamente a la última versión estable y notificar al equipo, garantizando una recuperación rápida sin intervención manual.

- **Monitoreo continuo y retroalimentación**: Tras cada despliegue, herramientas de monitoreo evalúan el rendimiento, los errores y la experiencia del usuario. Esta información alimenta el ciclo de mejora continua, permitiendo iteraciones rápidas y enfocadas en el usuario.


### 7.3.2. Production Deployment Pipeline Components

## 7.3.2. Componentes del Pipeline de Despliegue a Producción

En esta sección, se detallan los componentes que forman parte del pipeline de despliegue a producción, enfocados en la base de datos, el backend y el frontend, y cómo se integran para automatizar todo el proceso de despliegue.

### Componentes del Pipeline de la Base de Datos (Aiven):

1. **Gestión de Migraciones Automáticas**: Cuando se realizan cambios en el modelo de datos del backend (FastAPI), el sistema se encarga de gestionar automáticamente las migraciones de la base de datos. Cada vez que se modifican las entidades, FastAPI aplica los cambios necesarios en la base de datos administrada por Aiven, garantizando que la estructura de la base de datos esté siempre sincronizada con los cambios del código.

2. **Backup Automático**: Aiven crea copias de seguridad automáticas de la base de datos antes de aplicar cualquier migración importante. Esto asegura que, en caso de un fallo durante el proceso de migración, se pueda restaurar la base de datos a su estado anterior sin perder información.

3. **Monitoreo de la Base de Datos**: Aiven ofrece herramientas de monitoreo que permiten al equipo de desarrollo verificar el estado de la base de datos después de aplicar las migraciones. En caso de que se detecten problemas de rendimiento o errores durante la ejecución de consultas, Aiven envía alertas al equipo, lo que facilita la intervención temprana.

4. **Validación del Esquema**: Después de completar las migraciones, es recomendable ejecutar pruebas automatizadas que aseguren que el esquema de la base de datos se ha actualizado correctamente. Esto incluye validar que las tablas, columnas y relaciones se han configurado correctamente.

5. **Despliegue Continuo**: Una vez que todas las migraciones han sido aplicadas y validadas, los cambios se reflejan automáticamente en el entorno de producción, asegurando un flujo de trabajo continuo y eficiente.

### Componentes del Pipeline del Backend (Render para FastAPI):

1. **Integración Continua**: Cuando se realiza un commit en la rama `master`, Render toma el código actualizado del backend (FastAPI), lo compila y lo construye utilizando los procedimientos configurados.

2. **Construcción de la Imagen Docker**: Render construye una imagen Docker del backend, asegurando que todas las dependencias estén incluidas, lo que permite la portabilidad y consistencia del entorno en cualquier máquina.

3. **Despliegue**: Render despliega la nueva versión del backend en el servidor de producción, garantizando que el código esté disponible para los usuarios.

4. **Monitoreo y Alerta**: Después del despliegue, Render se encarga de monitorear la aplicación y enviar alertas en caso de fallos o problemas de rendimiento, lo que permite al equipo de operaciones actuar rápidamente si es necesario.

### Componentes del Pipeline del Frontend (Firebase para Angular):

1. **Compilación del Frontend**: Cuando se detecta un nuevo commit, Firebase CLI inicia el proceso de construcción de la aplicación Angular en modo producción.

2. **Ejecución de Pruebas Automatizadas**: Se ejecutan pruebas unitarias y funcionales para validar que la interfaz de usuario funcione correctamente según lo esperado.

3. **Despliegue en Firebase Hosting**: Si las pruebas son exitosas, Firebase despliega automáticamente la nueva versión de la aplicación web en producción, asegurando que se distribuya a través de una red de distribución de contenido (CDN) global para mejorar el rendimiento.

4. **Invalidación de Caché**: Firebase invalida automáticamente la caché, asegurando que los usuarios reciban siempre la versión más reciente de la aplicación.

## Capítulo VIII: Conclusiones

1. **Optimización de la gestión de citas veterinarias:** El proyecto permitió digitalizar y simplificar el proceso de agendamiento, reprogramación y cancelación de citas, ofreciendo a los usuarios una forma más eficiente de gestionar el cuidado de sus mascotas.

2. **Innovación en el monitoreo de mascotas:** La integración de collares inteligentes destacó como un avance significativo, brindando herramientas para el monitoreo continuo de la salud de las mascotas, lo que facilita un cuidado preventivo y mejora la comunicación entre veterinarios y propietarios.

3. **Impacto en la calidad del cuidado de mascotas:** La combinación de dispositivos IoT con la plataforma desarrollada promueve un cuidado más informado y personalizado, lo que contribuye al bienestar general de las mascotas y reduce riesgos asociados con la falta de seguimiento veterinario.

4. **Desarrollo de una solución escalable:** La plataforma establece una base tecnológica sólida que puede evolucionar, incorporando nuevas funcionalidades y dispositivos IoT para responder a futuras necesidades del mercado y mejorar la experiencia de los usuarios.

5. **Promoción de la adopción tecnológica:** 
El proyecto fomenta el uso de tecnología en un contexto cotidiano, demostrando cómo herramientas avanzadas pueden integrarse de manera efectiva en la vida diaria para solucionar problemas prácticos.


## Capítulo IX: Bibliografía

1. **Tull Soriano, Luis Federico.** *Prototipo de monitor de signos vitales en pacientes veterinarios de especie canina utilizando IoT.* Universidad Nacional Pedro Henríquez Ureña, 2021. [https://repositorio.unphu.edu.do/handle/123456789/3485](https://repositorio.unphu.edu.do/handle/123456789/3485)

2. **Grados Denegri, Felipe Alfredo, y Freddy Hernan Rodriguez Vega.** *Aplicativo móvil para la gestión de servicios clínicos veterinarios en Lima - Metropolitana.* Universidad Autónoma del Perú, 2021. [https://repositorio.autonoma.edu.pe/handle/20.500.13067/1079](https://repositorio.autonoma.edu.pe/handle/20.500.13067/1079)

## Capítulo X: Anexo

- **Landing Page:** [Enlace al landing page](https://pet-heart-health.github.io/landing-page-upet/)
- **Web Frontend:** [Enlace al proyecto web](https://frontend-app-upet.netlify.app)
- **Aplicación Móvil:** [Enlace al proyecto móvil](URL_DEL_MOBILE)
- **Backend:** [Enlace al backend](https://upetbackendapi.onrender.com/docs#/)
- **Mockups:** [Enlace a los mockups](https://www.figma.com/design/HG5VxSXVvjfVC0BGdiWywi/IOT---Mobile-Application?node-id=0-1&node-type=canvas&t=WLj5vcz6RIZRcTvT-0)
- **Prototipo:** [Enlace a los mockups](https://www.figma.com/proto/HG5VxSXVvjfVC0BGdiWywi/IOT---Mobile-Application?node-id=64-5609&node-type=canvas&t=WLj5vcz6RIZRcTvT-0&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=64%3A5606&show-proto-sidebar=1)

