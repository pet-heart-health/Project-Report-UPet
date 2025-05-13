# Capítulo III: Requirements Specification.

## 3.1. To-Be Scenario Mapping.

En esta sección, se presenta el To Be Scenario Mapping para cada segmento objetivo. Esta herramienta permite visualizar y definir el proceso mejorado. A través de este mapeo, se identificaron las áreas clave de mejora y se establecieron las acciones necesarias para optimizar el rendimiento y la eficiencia en cada segmento.

### Segmento 1: Veterinaria

![To-Be Scenario Mapping Veterinaria](../assets/to-be-veterinario.png)

### Segmento 2: Propietario de mascota

![To-Be Scenario Mapping PropietariodeMascota](../assets/to-be-propietario.png)

## 3.2. User Stories.

En esta sección, se presentan los requisitos definidos junto con el conjunto de User Stories y Epics para los requisitos identificados. Las User Stories permiten al equipo de desarrollo comprender las necesidades y expectativas de los usuarios finales, así como priorizar y planificar las funcionalidades del producto de manera efectiva. Asimismo, cada User Storie incluye sus Acceptance Criteria correspondientes.

<table>
      <thead>
            <tr>
                <th>Epic / Story ID</th>
                <th>Título</th>
                <th>Descripción</th>
                <th>Criterios de Aceptación</th>
                <th>Relacionado con (Epic ID)</th>
            </tr>
      </thead>
      <tbody>
            <tr>
                <td>EPIC-01</td>
                <td>Gestión de cuenta </td>
                <td>
                    <strong>Como</strong> usuario, 
                    <strong>quiero</strong> registrar, acceder y configurar mi cuenta 
                    <strong>para</strong> ingresar y utilizar las funcionalidades de la aplicación.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-02</td>
                <td>Gestión de la información de la mascota</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> registrar, editar y compartir la información de mi mascota
                    <strong>para</strong> tener un control y seguimiento de mi mascota.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-03</td>
                <td>Gestión de citas</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> agendar, reprogramar o cancelar citas
                    <strong>para</strong> manejar y organizar las citas de mi mascota.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-04</td>
                <td>Notificaciones</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> activar y recibir notificaciones
                    <strong>para</strong> estar informado sobre las citas y recordatorios de mi mascota.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-05</td>
                <td>Registro del Historial médico veterinario</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> registrar y visualizar el historial médico veterinario de mi mascota
                    <strong>para</strong> digitalizar y compartir la información con el veterinario.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-06</td>
                <td>Gestión de la suscripción</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> suscribirme y gestionar mi plan de suscripción
                    <strong>para</strong> acceder a funcionalidades premium y beneficios exclusivos.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-07</td>
                <td>Búsqueda de veterinarias en el mapa</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> buscar y visualizar veterinarias cercanas
                    <strong>para</strong> ubicar y contactar a un veterinario.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-08</td>
                <td>Información de Veterinarias</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> visualizar información detallada de las veterinarias
                    <strong>para</strong> conocer los servicios y horarios de atención.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-09</td>
                <td>Registro de veterinarias</td>
                <td>
                    <strong>Como</strong> usuario registrado, 
                    <strong>quiero</strong> registrar y editar información de la veterinaria
                    <strong>para</strong> actualizar y mantener actualizada la información.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-10</td>
                <td>Backend API</td>
                <td>
                    <strong>Como</strong> usuario desarrollador, 
                    <strong>quiero</strong> implementar una API RESTful 
                    <strong>para</strong> gestionar la información de la aplicación.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                <td>EPIC-11</td>
                <td>Acceso al sitio web estático</td>
                <td>
                    <strong>Como</strong> usuario visitante, 
                    <strong>quiero</strong> acceder al sitio web estático
                    <strong>para</strong> conocer la información de la aplicación.
                </td>
                <td>-</td>
                <td>-</td>
            </tr>
            <tr>
                  <td>US-001</td>
                  <td>Registrar Mascota</td>
                  <td>
                      <strong>Como</strong> propietario de una mascota 
                      <strong>quiero</strong> crear un perfil para cada una de mis mascotas en la aplicación, ingresando su información básica 
                      <strong>para</strong> mantener un registro organizado de sus datos.
                  </td>
                  <td>
                      <h5>Escenario 01: Agregar una Nueva Mascota</h5>
                      <strong>Dado</strong> el propietario de mascota se encuentra en la página principal, 
                      <strong>cuando</strong> selecciona la opción de agregar una nueva mascota, 
                      <strong>Entonces</strong> se abre un formulario donde puede ingresar el nombre, la raza, la edad, el peso, entre otros datos importantes.
                      <br>
                      <h5>Escenario 02: Guardar Cambios de la Mascota</h5>
                      <strong>Dado</strong> el propietario de mascota ha ingresado la información en el formulario de la mascota, 
                      <strong>cuando</strong> guarda los cambios realizados, 
                      <strong>Entonces</strong> la información de la mascota se actualiza en el sistema y se muestra un mensaje de confirmación.
                      <br>
                      <h5>Escenario 03: Validación de Campos Obligatorios</h5>
                      <strong>Dado</strong> el propietario se encuentra en el formulario de información de la mascota, 
                      <strong>cuando</strong> intenta guardar los cambios sin completar todos los campos obligatorios, 
                      <strong>Entonces</strong> se muestra un mensaje de error que indica que debe llenar los campos requeridos.
                  </td>
                  <td>EPIC-02</td>
            </tr>
                        <tr>
                <td>US-002</td>
                <td>Subir foto de la mascota</td>
                <td>
                    <strong>Como</strong> propietario de mascota,
                    <strong>quiero</strong> poder subir una foto de mi mascota a la plataforma,
                    <strong>para</strong> poder personalizar su perfil y compartir su imagen con las veterinarias.
                </td>
                <td>
                    <h5>Escenario 01: Selección de Foto</h5>
                    <strong>Dado</strong> que estoy en la página de perfil de mi mascota,
                    <strong>cuando</strong> hago clic en el botón "Subir foto",
                    <strong>Entonces</strong> se abre un cuadro de diálogo para seleccionar la foto desde mi dispositivo.
                    <br>
                    <h5>Escenario 02: Confirmación de selección de foto</h5>
                    <strong>Dado</strong> que he seleccionado la foto de mi mascota,
                    <strong>cuando</strong> confirmo la selección,
                    <strong>Entonces</strong> la foto se carga correctamente en el perfil de la mascota y se muestra en la página.
                    <br>
                    <h5>Escenario 03: Manejar errores de carga de foto</h5>
                    <strong>Dado</strong> intento subir una foto que no cumple con los requisitos de formato o tamaño,
                    <strong>cuando</strong> selecciono la foto y trato de cargarla,
                    <strong>Entonces</strong> recibo un mensaje de error indicando los requisitos de formato o tamaño y no se permite la carga de la foto hasta que cumpla con estos criterios.
                </td>
                <td>EPIC-02</td>
            </tr>
            <tr>
                <td>US-003</td>
                <td>Ver listado de mis mascotas</td>
                <td>
                    <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> poder ver un listado de todas mis mascotas registradas en la aplicación,
                    <strong>para</strong> tener un acceso rápido a su información y gestionarlas de manera eficiente.
                </td>
                <td>
                    <h5>Escenario 01: Listado de mascotas</h5>
                    <strong>Dado</strong> el propietario de la mascota se encuentra en la pantalla inicial de la aplicación,
                    <strong>cuando</strong> navega a la sección de "Mis Mascotas",
                    <strong>Entonces</strong> se muestra un listado de todas sus mascotas registradas, incluyendo su nombre y foto.
                    <br>
                    <h5>Escenario 02: Usuario sin mascotas registradas</h5>
                    <strong>Dado</strong> el propietario de la mascota se encuentra en la pantalla inicial de la aplicación,
                    <strong>cuando</strong> el usuario intenta acceder al listado de sus mascotas, pero no tiene ninguna mascota registrada,
                    <strong>Entonces</strong> se muestra un mensaje de error indicando que no tiene mascotas registradas.
                    <br>
                    <h5>Escenario 03: Detalles de mascota seleccionada</h5>
                    <strong>Dado</strong> el propietario de la mascota se encuentra en la pantalla de “Mis mascotas”,
                    <strong>cuando</strong> selecciona una mascota del listado,
                    <strong>Entonces</strong> se muestra una pantalla con los detalles completos de la mascota, incluyendo su nombre, foto, especie, raza, edad, entre otros datos importantes.
                </td>
                <td>EPIC-02</td>
            </tr>
            <tr>
                <td>US-004</td>
                <td>Editar información de la mascota</td>
                <td>
                    <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> poder editar la información del perfil de mi mascota en la aplicación,
                    <strong>para</strong> mantener actualizada la información de mis mascotas.
                </td>
                <td>
                    <h5>Escenario 01: Acceso al perfil de la mascota para editar</h5>
                    <strong>Dado</strong> el usuario se encuentra en el perfil de la mascota que desea editar,
                    <strong>cuando</strong> selecciona la opción de actualizar información,
                    <strong>Entonces</strong> aparece el formulario de edición de perfil.
                    <br>
                    <h5>Escenario 02: Edición de la información de la mascota</h5>
                    <strong>Dado</strong> el propietario de la mascota se encuentra en el formulario,
                    <strong>cuando</strong> modifica la información de su mascota y selecciona la opción guardar,
                    <strong>Entonces</strong> se muestra un mensaje indicando que la información del perfil de la mascota ha sido actualizada correctamente.
                    <br>
                    <h5>Escenario 03: Validación de datos al editar</h5>
                    <strong>Dado</strong> que el propietario de la mascota se encuentra en el formulario de edición de perfil,
                    <strong>cuando</strong> intenta guardar cambios con un campo obligatorio sin completar,
                    <strong>Entonces</strong> se muestra un mensaje de error indicando que es necesario completar todos los campos obligatorios antes de guardar los cambios.
                </td>
                <td>EPIC-02</td>
            </tr>
            <tr>
                <td>US-005</td>
                <td>Registrar vacunas</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder registrar las vacunas administradas a cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>
                    <h5>Escenario 01: Registro de vacuna exitoso</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> se administra una vacuna a una mascota,
                    <strong>Entonces</strong> se registra la vacuna en el historial médico de la mascota con los detalles correspondientes.
                    <br>
                    <h5>Escenario 02: Validación de datos de vacuna</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> intenta registrar una vacuna pero faltan datos obligatorios,
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error indicando los datos faltantes y no permite el registro hasta que se completen.
                    <br>
                    <h5>Escenario 03: Actualización de vacuna existente</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> se necesita actualizar la información de una vacuna existente,
                    <strong>Entonces</strong> el usuario puede buscar la vacuna existente en el historial médico de la mascota y actualizar los datos.
                </td>
                <td>EPIC-05</td>
            </tr>
            <tr>
                <td>US-006</td>
                <td>Registrar resultados</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder registrar los resultados de análisis obtenidos de cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>
                    <h5>Escenario 01: Registro de resultados exitoso</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> se obtienen los resultados de análisis de una mascota,
                    <strong>Entonces</strong> el usuario registra los datos del resultado en el historial médico de la mascota.
                    <br>
                    <h5>Escenario 02: Validación de datos de resultados</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> intenta registrar los resultados pero faltan datos obligatorios,
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error indicando los datos faltantes.
                    <br>
                    <h5>Escenario 03: Adición de resultados al historial médico</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> tiene los resultados registrados y quiere agregarlos al historial médico,
                    <strong>Entonces</strong> la aplicación muestra una opción de añadir el registro de resultados al historial médico del paciente.
                </td>
                <td>EPIC-05</td>
            </tr>
            <tr>
                <td>US-007</td>
                <td>Registrar cirugías</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> registrar un reporte de los resultados de cirugías realizadas en cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>
                    <h5>Escenario 01: Registro de reporte quirúrgico exitoso</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> se realiza una cirugía en una mascota,
                    <strong>Entonces</strong> el usuario registra los detalles de la cirugía en el historial médico de la mascota.
                    <br>
                    <h5>Escenario 02: Validación de datos del reporte</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> intenta registrar los datos de la cirugía pero faltan datos obligatorios,
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error indicando los datos faltantes.
                    <br>
                    <h5>Escenario 03: Adición de resultados de cirugía al historial médico</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> tiene los resultados registrados de la cirugía y quiere agregarlos al historial médico,
                    <strong>Entonces</strong> la aplicación muestra una opción de añadir el registro al historial médico.
                </td>
                <td>EPIC-05</td>
            </tr>
            <tr>
                <td>US-008</td>
                <td>Registrar enfermedades</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder registrar las enfermedades diagnosticadas en cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>
                    <h5>Escenario 01: Registro de diagnóstico exitoso</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> se diagnostica una enfermedad en una mascota,
                    <strong>Entonces</strong> el usuario registra los detalles del diagnóstico en el historial médico de la mascota.
                    <br>
                    <h5>Escenario 02: Validación de datos de diagnóstico</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> intenta registrar los datos del diagnóstico pero faltan datos obligatorios,
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error indicando los datos faltantes.
                    <br>
                    <h5>Escenario 03: Adición de diagnóstico al historial médico</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> tiene el diagnóstico y quiere agregarlo al historial médico,
                    <strong>Entonces</strong> la aplicación muestra una opción de añadir el diagnóstico al historial médico del paciente.
                </td>
                <td>EPIC-05</td>
            </tr>
            <tr>
                <td>US-009</td>
                <td>Visualizar resumen del historial médico</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder visualizar el resumen del historial médico de cada mascota,
                    <strong>para</strong> considerar sus antecedentes durante la atención de una consulta.
                </td>
                <td>
                    <h5>Escenario 01: Visualización del resumen del historial médico exitoso</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> requiere el resumen del historial médico para atender a una mascota,
                    <strong>Entonces</strong> el sistema muestra la información relevante del historial médico de la mascota, como vacunas, cirugías y diagnósticos.
                    <br>
                    <h5>Escenario 02: Visualización del historial médico por fecha</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> necesita ver el historial médico filtrado por fecha,
                    <strong>Entonces</strong> el sistema muestra el historial médico en el orden de fechas solicitado.
                    <br>
                    <h5>Escenario 03: Validación de fecha filtrada</h5>
                    <strong>Dado</strong> el usuario está autenticado como veterinario o personal autorizado,
                    <strong>cuando</strong> solicita ver el historial médico filtrado por una fecha inválida,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que la fecha es incorrecta.
                </td>
                <td>EPIC-05</td>
            </tr>
            <tr>
                <td>US-010</td>
                <td>Ver información del footer</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder acceder a los enlaces del footer,
                    <strong>para</strong> navegar rápidamente a secciones como redes sociales, noticias y contacto.
                </td>
                <td>
                    <h5>Escenario 01: Acceso a redes sociales desde el footer</h5>
                    <strong>Dado</strong> que el usuario está en la parte inferior de la página web,
                    <strong>cuando</strong> hace clic en los enlaces de redes sociales,
                    <strong>Entonces</strong> el sistema lo redirige a las cuentas oficiales de redes sociales.
                    <br>
                    <h5>Escenario 02: Visualización de contacto</h5>
                    <strong>Dado</strong> que el usuario está en la parte inferior de la página web,
                    <strong>cuando</strong> visualiza los contactos del equipo de UPet,
                    <strong>Entonces</strong> el sistema le muestra la dirección, telefono móvil y correo electrónico.
                    <br>
                    <h5>Escenario 03: Error al cargar información del footer</h5>
                    <strong>Dado</strong> que el usuario intenta acceder a un enlace del footer,
                    <strong>cuando</strong> ocurre un error técnico,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que no se pudo cargar la página solicitada.
                </td>
                <td>EPIC-11</td>
            </tr>
            <tr>
                <td>US-011</td>
                <td>Revisar reseñas de la aplicación</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder ver las reseñas de la aplicación,
                    <strong>para</strong> conocer la experiencia de otros usuarios antes de descargarla o registrarme.
                </td>
                <td>
                    <h5>Escenario 01: Visualización de reseñas recientes</h5>
                    <strong>Dado</strong> que el usuario está en la sección de reseñas,
                    <strong>cuando</strong> desplaza hacia abajo en la página,
                    <strong>Entonces</strong> el sistema muestra un carrusel de reseñas recientes de otros usuarios.
                    <br>
                    <h5>Escenario 02: Error al cargar reseñas</h5>
                    <strong>Dado</strong> que el usuario intenta cargar las reseñas,
                    <strong>cuando</strong> ocurre un error técnico,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error y sugiere intentar nuevamente más tarde.
                </td>
                <td>EPIC-11</td>
            </tr>
            <tr>
                <td>US-012</td>
                <td>Navegar en la página principal</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> acceder a la página principal del sitio web y ver un botón de Call to Action 
                    <strong>para</strong> descargar la aplicación o registrarme, para tener acceso rápido a la funcionalidad principal.
                </td>
                <td>
                    <h5>Escenario 01: Visualización de la página principal</h5>
                    <strong>Dado</strong> que el visitante está en la página de inicio,
                    <strong>cuando</strong> carga el sitio,
                    <strong>Entonces</strong> se visualiza un botón destacado de Call to Action con texto claro como "Descargar" en la parte superior derecha de la página.
                    <br>
                    <h5>Escenario 02: Redirección desde el botón</h5>
                    <strong>Dado</strong> que el visitante está en la página de inicio,
                    <strong>cuando</strong> hace clic en el boton "Descargar",
                    <strong>Entonces</strong> el sistema lo redirige a la sección de Download.
                    <br>
                    <h5>Escenario 03: Verificación del funcionamiento del botón en dispositivos móviles</h5>
                    <strong>Dado</strong> que el visitante está en la página de inicio desde un dispositivo móvil,
                    <strong>cuando</strong> hace clic en el boton "Descargar",
                    <strong>Entonces</strong> el sistema funciona correctamente y redirige a la sección adecuada.
                </td>
                <td>EPIC-11</td>
            </tr>
            <tr>
                <td>US-013</td>
                <td>Ver funcionalidades para propietarios de mascotas</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> ver las funcionalidades que ofrece la aplicación para los dueños de mascotas,
                    <strong>para</strong> saber cómo puedo usarla para cuidar de mi mascota.
                </td>
                <td>
                    <h5>Escenario 01: Visualización de funcionalidades</h5>
                    <strong>Dado</strong> que el visitante está en la página de funcionalidades para propietarios de mascotas,
                    <strong>cuando</strong> llega a esa sección,
                    <strong>Entonces</strong> puede ver una lista de las funcionalidades destacadas como agendar citas, registrar historial médico, recibir recordatorios, etc.
                    <br>
                    <h5>Escenario 02: Detalle de una funcionalidad</h5>
                    <strong>Dado</strong> que el visitante quiere saber más sobre una funcionalidad en particular,
                    <strong>cuando</strong> revisa una funcionalidad específica,
                    <strong>Entonces</strong> el sistema muestra una descripción detallada de esa funcionalidad.
                    <br>
                    <h5>Escenario 03: Error al cargar la lista de funcionalidades</h5>
                    <strong>Dado</strong> que el visitante está intentando ver las funcionalidades para propietarios de mascotas,
                    <strong>cuando</strong> ocurre un error técnico,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que no se pueden cargar las funcionalidades.
                </td>
                <td>EPIC-11</td>
            </tr>
            <tr>
                <td>US-014</td>
                <td>Ver funcionalidades para veterinarias</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> ver las funcionalidades que ofrece la aplicación para veterinarias,
                    <strong>para</strong> conocer cómo puedo usarla en mi clínica veterinaria.
                </td>
                <td>
                    <h5>Escenario 01: Visualización de funcionalidades</h5>
                    <strong>Dado</strong> que el visitante está en la página de funcionalidades para veterinarias,
                    <strong>cuando</strong> llega a esa sección,
                    <strong>Entonces</strong> puede ver una lista de las funcionalidades para clínicas como agendar citas, llevar el historial médico de las mascotas, gestión de clientes, etc.
                    <br>
                    <h5>Escenario 02: Detalle de una funcionalidad</h5>
                    <strong>Dado</strong> que el visitante quiere saber más sobre una funcionalidad para veterinarias,
                    <strong>cuando</strong> revisa en una funcionalidad específica,
                    <strong>Entonces</strong> el sistema muestra una descripción detallada de esa funcionalidad.
                    <br>
                    <h5>Escenario 03: Error al cargar la lista de funcionalidades</h5>
                    <strong>Dado</strong> que el visitante está intentando ver las funcionalidades para veterinarias,
                    <strong>cuando</strong> ocurre un error técnico,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que no se pueden cargar las funcionalidades.
                </td>
                <td>EPIC-11</td>
            </tr>
            <tr>
                <td>US-015</td>
                <td>Descargar la aplicación</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder descargar la aplicación desde el sitio web estático,
                    <strong>para</strong> instalarla en mi dispositivo y comenzar a usarla.
                </td>
                <td>
                    <h5>Escenario 01: Descarga desde Google Play</h5>
                    <strong>Dado</strong> que el visitante está en la sección de descarga de la página web,
                    <strong>cuando</strong> hace clic en el botón de descarga de Google Play,
                    <strong>Entonces</strong> el sistema lo redirige a la tienda Google Play para descargar la aplicación.
                    <br>
                    <h5>Escenario 02: Descarga desde App Store</h5>
                    <strong>Dado</strong> que el visitante está en la sección de descarga de la página web,
                    <strong>cuando</strong> hace clic en el botón de descarga de App Store,
                    <strong>Entonces</strong> el sistema lo redirige a la tienda App Store para descargar la aplicación.
                    <br>
                    <h5>Escenario 03: Error al intentar descargar la aplicación</h5>
                    <strong>Dado</strong> que el visitante está intentando descargar la aplicación,
                    <strong>cuando</strong> ocurre un error técnico,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que no se puede completar la descarga.
                </td>
                <td>EPIC-11</td>
            </tr>
            <tr>
                <td>US-016</td>
                <td>Enviar un mensaje desde el sitio de web estático</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder enviar un mensaje al equipo de la aplicación desde la sección de contacto,
                    <strong>para</strong> resolver dudas o recibir más información sobre el servicio.
                </td>
                <td>
                    <h5>Escenario 01: Envío de mensaje exitoso</h5>
                    <strong>Dado</strong> que el visitante ha completado el formulario en la sección "Send us a message",
                    <strong>cuando</strong> hace clic en el botón de enviar,
                    <strong>Entonces</strong> el sistema envía el mensaje correctamente y muestra un mensaje de confirmación.
                    <br>
                    <h5>Escenario 02: Campos incompletos en el formulario</h5>
                    <strong>Dado</strong> que el visitante intenta enviar un mensaje,
                    <strong>cuando</strong> no ha completado todos los campos obligatorios del formulario,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que debe completar todos los campos.
                    <br>
                    <h5>Escenario 03: Error al intentar enviar el mensaje</h5>
                    <strong>Dado</strong> que el visitante intenta enviar un mensaje desde la sección "Send us a message",
                    <strong>cuando</strong> ocurre un error técnico,
                    <strong>Entonces</strong> el sistema muestra un mensaje de error indicando que no se pudo enviar el mensaje y sugiere intentarlo más tarde.
                </td>
                <td>EPIC-11</td>
            </tr>
            <tr>
                <td>US-017</td>
                <td>Mostrar tu ubicación actual</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan,
                    <strong>quiero</strong> poder visualizar mi ubicación
                    <strong>para</strong> buscar centros de atención cerca de mi ubicación.
                </td>
                <td>
                    <h5>Escenario 01: Mostrar ubicación actual del usuario con éxito</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación
                    <strong>cuando</strong> selecciona la opción para mostrar su ubicación actual con el propósito de buscar centros
                    <strong>Entonces</strong> la aplicación accede a la ubicación actual del usuario y la muestra en el mapa de manera precisa.
                    <br>
                    <h5>Escenario 02: Imposibilidad de obtener la ubicación actual del usuario</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación
                    <strong>cuando</strong> intenta acceder a la opción mostrar su ubicación actual
                    <strong>Y</strong> la aplicación intenta obtener la ubicación actual del usuario, pero hay una falla en el dispositivo o el usuario ha desactivado su gps
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error indicando que no se pudo obtener la ubicación y sugiere que active la función de ubicación en su dispositivo.
                    <br>
                </td>
                <td>EPIC-07</td>
            </tr>
            <tr>
                <td>US-018</td>
                <td>Ver las valoraciones y comentarios de la veterinaria</td>
                <td>
                    <strong>Como</strong> veterinario/a o personal autorizado de la clínica veterinaria, 
                    <strong>quiero</strong> poder visualizar las valoraciones y comentarios de mi veterinaria,
                    <strong>para</strong> mejorar en los aspectos negativos que pueda tener.
                </td>
                <td>
                    <h5>Escenario 01: Ver valoraciones y comentarios de la veterinaria con éxito</h5>
                    <strong>Dado</strong> el usuario está autenticado en la aplicación como veterinario/a o personal autorizado.
                    <strong>cuando</strong> accede a la sección de valoraciones y comentarios de la veterinaria en la aplicación
                    <strong>Entonces</strong> La aplicación muestra una lista de valoraciones y comentarios dejados por los clientes sobre la veterinaria.
                    <br>
                    <h5>Escenario 02: Comunicación directa con los clientes insatisfechos</h5>
                    <strong>Dado</strong> el usuario está autenticado en la aplicación como veterinario/a o personal autorizado.
                    <strong>cuando</strong> encuentra un comentario negativo sobre la veterinaria
                    <strong>Entonces</strong> la aplicación proporciona la opción de responder al comentario de forma que la veterinaria aborde directamente el problema para resolver que haya surgido.
                    <br>
                </td>
                <td>EPIC-07</td>
            </tr>
            <tr>
                <td>US-019</td>
                <td>Añadir valoraciones y comentarios</td>
                <td>
                    <strong>Como</strong> propietario/a de mascota autenticado y suscrito a un plan, 
                    <strong>quiero</strong> poder realizar comentarios y valoraciones,
                    <strong>para</strong> calificar la atención de cada centro de atención.
                </td>
                <td>
                    <h5>Escenario 01: Comentario añadido con éxito</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> selecciona la opción para añadir una valoración y comentario sobre un centro de atención
                    <strong>Entonces</strong> la aplicación presenta un formulario donde el usuario puede ingresar su valoración en forma de puntuación y agregar un comentario opcionalmente.
                    <br>
                    <h5>Escenario 02: Intento de añadir valoración y comentario sin estar suscrito</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a pero no está suscrito a un plan.
                    <strong>Cuando</strong> intenta añadir una valoración acerca de una veterinaria
                    <strong>Entonces</strong> la aplicación detecta que el usuario no está suscrito a un plan y le muestra un mensaje de error indicando que esta función solo está disponible para usuarios suscritos.
                    <br>
                    <h5>Escenario 03: Edición de valoración y comentario existente</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> desea editar una valoración o comentario que realizó anteriormente
                    <strong>Entonces</strong> la aplicación permite al usuario editar la valoración y/o comentario existente y guarda los cambios realizados.
                </td>
                <td>EPIC-08</td>
            </tr>
            <tr>
                <td>US-020</td>
                <td>Ver detalles de cada veterinaria</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan, 
                    <strong>quiero</strong> poder visualizar la información de cada veterinaria,
                    <strong>para</strong> poder elegir con mayor eficacia la veterinaria acorde a mis necesidades.
                </td>
                <td>
                    <h5>Escenario 01: Visualización de detalles de veterinaria</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> desea visualizar los detalles de una veterinaria específica
                    <strong>Entonces</strong> la aplicación muestra información detallada sobre la veterinaria seleccionada.
                    <br>
                    <h5>Escenario 02: Ver detalles de la veterinaria con filtros de búsqueda</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> desea ver los detalles de una veterinaria, pero tiene preferencias específicas, como los servicios ofrecidos
                    <strong>Entonces</strong> la aplicación permite al usuario aplicar filtros de búsqueda para ver solo las veterinarias que cumplan con sus criterios específicos.
                </td>
                <td>EPIC-08</td>
            </tr>
            <tr>
                <td>US-021</td>
                <td>Ver reseñas y evaluación</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan, 
                    <strong>quiero</strong> visualizar las reseñas de cada veterinaria,
                    <strong>para</strong> facilitar el proceso de selección de cada centro.
                </td>
                <td>
                    <h5>Escenario 01: Visualización de reseñas y evaluación</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> desea visualizar las reseñas y evaluaciones de una veterinaria específica
                    <strong>Entonces</strong> la aplicación muestra una lista de reseñas y evaluaciones dejadas por otros usuarios sobre la veterinaria seleccionada.
                    <br>
                    <h5>Escenario 02: Ver reseñas y evaluaciones con filtros de búsqueda</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> desea visualizar las reseñas y evaluaciones de una veterinaria, pero tiene preferencias específicas, como la búsqueda de reseñas positivas o negativas
                    <strong>Entonces</strong> la aplicación permite al usuario aplicar filtros de búsqueda para ver solo las reseñas que cumplan con sus criterios específicos, como la puntuación dada por otros usuarios.
                </td>
                <td>EPIC-08</td>
            </tr>
            <tr>
                <td>US-022</td>
                <td>Entrar al perfil de cada veterinaria</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan, 
                    <strong>quiero</strong> visualizar información personal de cada veterinaria,
                    <strong>para</strong> poder informarme mejor acerca de cada veterinaria.
                </td>
                <td>
                    <h5>Escenario 01: Visualización de perfil de la veterinaria</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> desea visualizar el perfil de cada veterinaria
                    <strong>Entonces</strong> la aplicación carga el perfil completo de la veterinaria, que incluye información detallada como el nombre, reseñas, servicios, dirección, horarios de atención, servicios ofrecidos.
                    <br>
                    <h5>Escenario 02: Ver información detallada de la veterinaria con filtros de búsqueda</h5>
                    <strong>Dado</strong> el usuario está autenticado como propietario/a en la versión gratuita o suscrito en la aplicación.
                    <strong>Cuando</strong> desea visualizar el perfil, pero tiene preferencias específicas, como buscar veterinarias con ciertas especialidades
                    <strong>Entonces</strong> la aplicación permite al usuario aplicar filtros de búsqueda para ver solo las veterinarias que cumplan con sus criterios específicos.
                </td>
                <td>EPIC-08</td>
            </tr>
            <tr>
                <td>US-023</td>
                <td>Añadir ubicación</td>
                <td>
                    <strong>Como</strong> veterinaria o personal autorizado de la clínica veterinaria, 
                    <strong>quiero</strong> añadir la ubicación de mi centro de atención,
                    <strong>para</strong> mostrar la ubicación actual de mi centro de atención.
                </td>
                <td>
                    <h5>Escenario 01: Registro de ubicación de veterinaria</h5>
                    <strong>Dado</strong> el usuario está autenticado en la aplicación como veterinario/a o personal autorizado.
                    <strong>Cuando</strong> se selecciona la opción añadir ubicación de la veterinaria.
                    <strong>Entonces</strong> la aplicación le mostrará el mapa para poder elegir la ubicación que desea guardar para su veterinaria.
                    <br>
                    <h5>Escenario 02: Intento de añadir ubicación sin autorización</h5>
                    <strong>Dado</strong> el usuario no está autenticado en la aplicación como veterinario/a o personal de la clínica.
                    <strong>Cuando</strong> intenta añadir la ubicación de un centro de atención
                    <strong>Entonces</strong> la aplicación detecta que el usuario no tiene los permisos adecuados y le muestra un mensaje de error indicando que esta función está disponible solo para personal autorizado.
                    <br>
                    <h5>Escenario 03: Actualización de ubicación existente</h5>
                    <strong>Dado</strong> el usuario está autenticado en la aplicación como veterinario/a o personal autorizado.
                    <strong>Cuando</strong> necesita actualizar la ubicación de su centro de atención debido a una reubicación 
                    <strong>Entonces</strong> la aplicación permite al usuario editar la ubicación existente del centro de atención y guarda los cambios realizados.
                </td>
                <td>EPIC-09</td>
            </tr>
<tr>
                <td>US-024</td>
                <td>Registro de cuenta</td>
                <!-- Descripción -->
                <td> 
                <strong>Como</strong> veterinario o propietario de una mascota
                <strong>quiero</strong> registrarme en la aplicación 
                <strong>para</strong> acceder a sus funcionalidades.
                </td>
                <!-- ---------- -->
                <!-- Criterios de Aceptación -->
                <td> 
                <h5>Escenario 01: Registro Exitoso</h5>
                <strong>Dado</strong> el usuario está en la pantalla de registro
                <strong>cuando</strong> complete los campos requeridos,
                <strong>Entonces</strong> la cuenta se crea exitosamente y se redirige a la pantalla de inicio de sesión. 
                <br>
                <h5>Escenario 02: Datos Incompletos en el Registro</h5>
                <strong>Dado</strong> el usuario está en la pantalla de registro,
                <strong>cuando</strong> intenta registrarse con datos incompletos,
                <strong>Entonces</strong> se muestra un mensaje de error y se le pide que complete los campos vacíos.
                <br>
                <h5>Escenario 03:  Correo Electrónico en Uso</h5>
                <strong>Dado</strong> el usuario está en la pantalla de registro,
                <strong>cuando</strong> intenta registrarse con un correo electrónico que está en uso,
                <strong>Entonces</strong> se muestra un mensaje de error que indica que el correo ya está registrado en la aplicación.
                </td>   
                <br>
                <!-- ---------- -->
                <td>EPIC-01</td>
            </tr>
            <tr>
                <td>US-025</td>
                <td>Iniciar Sesión</td>
                <td>
                    <strong>Como</strong> veterinario o propietario de una mascota 
                    <strong>quiero</strong> poder iniciar sesión en la aplicación utilizando mis credenciales 
                    <strong>para</strong> acceder a las funcionalidades y gestionar la información ingresada.
                </td>
                <td>
                    <h5>Escenario 01: Inicio de Sesión Exitoso</h5>
                    <strong>Dado</strong> el usuario está en la pantalla de inicio de sesión, 
                    <strong>cuando</strong> ingresa su correo electrónico y contraseña, 
                    <strong>Entonces</strong> accede exitosamente a su cuenta y se redirige a la pantalla de inicio.
                    <br>
                    <h5>Escenario 02: Datos Incorrectos en el Inicio de Sesión</h5>
                    <strong>Dado</strong> el usuario está en la pantalla de inicio de sesión, 
                    <strong>cuando</strong> ingresa un correo electrónico o una contraseña incorrecta, 
                    <strong>Entonces</strong> se muestra un mensaje de error indicando que el correo electrónico o la contraseña están incorrectos.
                    <br>
                    <h5>Escenario 03: Correo no Registrado en el Inicio de Sesión</h5>
                    <strong>Dado</strong> el usuario está en la pantalla de inicio de sesión, 
                    <strong>cuando</strong> intenta iniciar sesión con un correo que no está registrado, 
                    <strong>Entonces</strong> se muestra un mensaje de error indicando que el correo no está registrado.
                </td>
                <td>EPIC-01</td>
            </tr>
            <tr>
                <td>US-026</td>
                    <td>Cerrar Sesión</td>
                    <td>
                        <strong>Como</strong> veterinario o propietario de una mascota 
                        <strong>quiero</strong> tener la capacidad de cerrar sesión en la aplicación 
                        <strong>para</strong> garantizar la seguridad de mi información y proteger mi privacidad.
                  </td>
                  <td>
                      <h5>Escenario 01: Cierre de Sesión Exitoso</h5>
                      <strong>Dado</strong> el usuario está autenticado en la aplicación, 
                      <strong>cuando</strong> selecciona la opción “Cerrar sesión” desde la pantalla de inicio, 
                      <strong>Entonces</strong> se cierra exitosamente la sesión del usuario y se redirige a la pantalla de inicio de sesión.
                  </td>
                  <td>EPIC-01</td>
            </tr>
            <tr>
                <td>US-027</td>
                    <td>Agendar una cita</td>
                    <td>
                        <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> poder agendar una cita en la clínica veterinaria a través de la aplicación,
                    <strong>para</strong> asegurar la atención médica oportuna para mi mascota.
                  </td>
                  <td>
                      <h5>Escenario 01: Elección del veterinario</h5>
                    <strong>Dado</strong> el propietario de la mascota se encuentra en el perfil de una clínica veterinaria,
                    <strong>cuando</strong> presiona la opción de agendar cita,
                    <strong>Entonces</strong> le muestra un formulario para elegir la fecha y hora.
                    <br>
                    <h5>Escenario 02: Agendar una cita con éxito</h5>
                    <strong>Dado</strong> el propietario de la mascota se encuentra en el formulario para agendar una cita,
                    <strong>cuando</strong> elige una fecha y hora disponibles, selecciona el tipo de servicio necesario para su mascota y confirma la cita,
                    <strong>Entonces</strong> la cita se agenda correctamente y se muestra un mensaje de confirmación.
                    <br>
                    <h5>Escenario 03: Selección de fecha y hora no disponible</h5>
                    <strong>Dado</strong> el propietario de una mascota se encuentra en la sección de citas,
                    <strong>cuando</strong> intenta agendar una cita en una fecha que no está disponible,
                    <strong>Entonces</strong> se muestra un mensaje indicando que no hay horarios disponibles en esa fecha y se le sugiere seleccionar una fecha alternativa.
                </td>
                  <td>EPIC-03</td>
            </tr>
            <tr>
                <td>US-028</td>
                <td>Acceso de la veterinaria a la información de la mascota</td>
                <td>
                    <strong>Como</strong> veterinario,
                    <strong>quiero</strong> poder acceder a la información completa de una mascota, incluyendo su historial médico, vacunas y tratamientos previos,
                    <strong>para</strong> brindar una atención adecuada durante una consulta veterinaria.
                </td>
                <td>
                    <h5>Escenario 01: Acceso exitoso a la información de la mascota</h5>
                    <strong>Dado</strong> el veterinario está en la consulta de la mascota y necesita acceder a su información,
                    <strong>cuando</strong> ingresa al perfil de la mascota en la aplicación,
                    <strong>Entonces</strong> la aplicación muestra la información completa de la mascota, incluyendo su historial médico, vacunas, tratamientos previos y cualquier otra información relevante.
                    <br>
                    <h5>Escenario 02: Error al acceder a la información de la mascota</h5>
                    <strong>Dado</strong> el veterinario está en la consulta de la mascota y necesita acceder a su información,
                    <strong>cuando</strong> intenta acceder a la información pero la aplicación no puede cargarla debido a un error técnico,
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error y sugiere al veterinario intentarlo más tarde o contactar con soporte técnico.
                    <br>
                    <h5>Escenario 03: Información incompleta de la mascota</h5>
                    <strong>Dado</strong> el veterinario está en la consulta de la mascota y necesita acceder a su información,
                    <strong>cuando</strong> accede a la información de la mascota pero encuentra que algunos datos importantes están incompletos o faltantes,
                    <strong>Entonces</strong> la aplicación muestra una alerta al veterinario indicando que la información de la mascota está incompleta y sugiere completarla lo antes posible para garantizar una atención adecuada.
                </td>
                <td>EPIC-05</td>
            </tr>
            <tr>
                <td>US-029</td>
                <td>Ver historial de citas</td>
                <td>
                    <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> poder ver el historial completo de citas veterinarias de mi mascota, incluyendo fechas, horarios y propósito de la visita,
                    <strong>para</strong> tener un registro completo de la atención recibida.
                </td>
                <td>
                    <h5>Escenario 01: Consulta de historial de citas exitosa</h5>
                    <strong>Dado</strong> el propietario está en la pantalla de historial de citas de la mascota,
                    <strong>cuando</strong> selecciona la opción de ver historial de citas,
                    <strong>Entonces</strong> la aplicación muestra una lista completa de todas las citas veterinarias anteriores de la mascota, incluyendo fechas, horarios, propósito de la visita y cualquier otra información relevante.
                    <br>
                    <h5>Escenario 02: Sin citas anteriores registradas</h5>
                    <strong>Dado</strong> el propietario está en la pantalla de historial de citas de la mascota,
                    <strong>cuando</strong> no tiene citas anteriores registradas,
                    <strong>Entonces</strong> la aplicación muestra un mensaje indicando que no hay citas anteriores registradas para la mascota.
                    <br>
                    <h5>Escenario 03: Error al cargar historial de citas</h5>
                    <strong>Dado</strong> el propietario está en la pantalla de historial de citas de la mascota,
                    <strong>cuando</strong> la aplicación intenta cargar el historial de citas pero se produce un error técnico,
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error y sugiere al propietario intentarlo más tarde o contactar con soporte técnico.
                </td>
                <td>EPIC-03</td>
            </tr>
            <tr>
                <td>US-030</td>
                <td>Confirmar cita</td>
                <td>
                    <strong>Como</strong> propietario de mascota,
                    <strong>quiero</strong> poder confirmar una cita veterinaria previamente agendada,
                    <strong>para</strong> asegurarme de que la cita está programada y evitar confusiones.
                </td>
                <td>
                    <h5>Escenario 01: Confirmación de cita exitosa</h5>
                    <strong>Dado</strong> el propietario recibe una notificación de recordatorio de la cita,
                    <strong>cuando</strong> selecciona la opción de confirmar cita en la notificación,
                    <strong>Entonces</strong> la aplicación registra la confirmación de la cita y muestra un mensaje de confirmación al propietario.
                    <br>
                    <h5>Escenario 02: Cancelación de cita después de confirmación</h5>
                    <strong>Dado</strong> el propietario ha confirmado la cita,
                    <strong>cuando</strong> decide cancelar la cita,
                    <strong>Entonces</strong> la aplicación cancela la cita y muestra un mensaje de confirmación al propietario.
                    <br>
                    <h5>Escenario 03: Error al confirmar cita</h5>
                    <strong>Dado</strong> el propietario recibe una notificación de recordatorio de la cita,
                    <strong>cuando</strong> intenta confirmar la cita pero la aplicación no puede procesar la solicitud debido a un error técnico,
                    <strong>Entonces</strong> la aplicación muestra un mensaje de error y sugiere al propietario intentarlo más tarde o contactar con soporte técnico.
                </td>
                <td>EPIC-04</td>
            </tr>
            <tr>
                <td>TS-001</td>
                <td>Endpoint Medical History</td>
                <td>
                    <strong>Como</strong> desarrollador front-end, 
                    <strong>quiero</strong> acceder a un endpoint en el backend para gestionar el historial médico de las mascotas, incluyendo el registro de enfermedades y vacunaciones asociadas,
                    <strong>para</strong> permitir el manejo completo del historial médico desde la interfaz de usuario.
                </td>
                <td>
                    <h5>Escenario 01: Crear una nueva enfermedad</h5>
                    <strong>Dado</strong> acceso a la API de gestión del historial médico y permisos para crear enfermedades.
                    <strong>Cuando</strong> se envía una solicitud POST con los detalles de la nueva enfermedad.
                    <strong>Entonces</strong> el sistema crea la enfermedad y responde con un código 201 si es exitoso. Si la enfermedad ya existe, devuelve un código 400 con un mensaje de error.
                    <br>
                    <h5>Escenario 02: Asociar una enfermedad a un historial médico</h5>
                    <strong>Dado</strong> acceso a la API de gestión del historial médico y permisos para asociar enfermedades.
                    <strong>Cuando</strong> se envía una solicitud POST con los detalles de la asociación de enfermedad.
                    <strong>Entonces</strong> el sistema crea la asociación y responde con un código 201 si es exitoso. Si el historial médico o la enfermedad no existen, devuelve un código 404 con un mensaje de error.
                    <br>
                    <h5>Escenario 03: Crear una nueva vacuna</h5>
                    <strong>Dado</strong> acceso a la API de gestión del historial médico y permisos para crear vacunas.
                    <strong>Cuando</strong> se envía una solicitud POST a con los detalles de la nueva vacuna.
                    <strong>Entonces</strong> el sistema crea la vacuna y responde con un código 201 si es exitoso. Si la vacuna ya existe, devuelve un código 400 con un mensaje de error.
                </td>
                <td>EPIC-10</td>
            </tr>
            <tr>
                <td>TS-002</td>
                <td>Endpoint Pet</td>
                <td>
                    <strong>Como</strong> desarrollador frontend, 
                    <strong>quiero</strong> poder integrar la funcionalidad de agregar y visualizar mascotas en la interfaz de usuario,
                    <strong>para</strong> permitir a los usuarios mantener un registro actualizado de sus mascotas desde la aplicación móvil.
                </td>
                <td>
                    <h5>Escenario 01: Crear una nueva mascota</h5>
                    <strong>Dado</strong> acceso a la API de mascotas.
                    <strong>Cuando</strong> se envía una solicitud POST con los detalles de la nueva mascota y el ID del propietario al que pertenece.
                    <strong>Entonces</strong> el sistema crea la mascota y responde con un código 201 si es exitoso. Si el propietario de la mascota no existe, devuelve un código 404.
                    <br>
                    <h5>Escenario 02: Obtener todas las mascotas</h5>
                    <strong>Dado</strong> acceso a la API de mascotas.
                    <strong>Cuando</strong> se envía una solicitud GET.
                    <strong>Entonces</strong> el sistema devuelve una lista con todas las mascotas existentes en el sistema. Responde con un código 200. Si no hay mascotas disponibles, devuelve una lista vacía.
                    <br>
                    <h5>Escenario 03: Obtener mascotas por ID de propietario</h5>
                    <strong>Dado</strong> acceso a la API de mascotas.
                    <strong>Cuando</strong> se envía una solicitud GET con el ID del propietario de la mascota.
                    <strong>Entonces</strong> el sistema devuelve una lista con todas las mascotas pertenecientes al propietario especificado. Responde con un código 200. Si el propietario de la mascota no existe o no tiene mascotas registradas, devuelve un código 404.
                </td>
                <td>EPIC-10</td>
            </tr>
            <tr>
                <td>TS-003</td>
                <td>Endpoint User</td>
                <td>
                    <strong>Como</strong> desarrollador frontend, 
                    <strong>quiero</strong> poder crear y obtener información sobre diferentes tipos de usuarios en la plataforma,
                    <strong>para</strong> gestionar eficazmente las cuentas de los usuarios desde la interfaz de usuario de la aplicación móvil.
                </td>
                <td>
                    <h5>Escenario 01: Crear un nuevo usuario</h5>
                    <strong>Dado</strong> un usuario desea registrarse en la plataforma.
                    <strong>Cuando</strong> envía una solicitud para crear un nuevo usuario mediante una solicitud POST con los detalles del usuario.
                    <strong>Entonces</strong> el sistema verifica la disponibilidad del correo electrónico y crea el nuevo usuario en la base de datos, devolviendo los detalles del usuario creado con un código de estado 201 (Created).
                    <br>
                    <h5>Escenario 02: Registrar un veterinario</h5>
                    <strong>Dado</strong> un veterinario desea registrarse en la plataforma.
                    <strong>Cuando</strong> envía una solicitud para registrar un veterinario mediante una solicitud POST con los detalles del veterinario y el ID de usuario.
                    <strong>Entonces</strong> el sistema verifica si el usuario existe y es apto para registrarse como veterinario, luego registra al veterinario en la base de datos y marca al usuario como registrado, devolviendo los detalles del veterinario registrado con un código de estado 201 (Created).
                    <br>
                    <h5>Escenario 03: Registrar un propietario de mascotas</h5>
                    <strong>Dado</strong> un propietario de mascotas desea registrarse en la plataforma.
                    <strong>Cuando</strong> envía una solicitud para registrar un propietario de mascotas mediante una solicitud POST con los detalles del propietario de mascotas y el ID de usuario.
                    <strong>Entonces</strong> el sistema verifica si el usuario existe y es apto para registrarse como propietario de mascotas, luego registra al propietario de mascotas en la base de datos y marca al usuario como registrado, devolviendo los detalles del propietario de mascotas registrado con un código de estado 201 (Created).
                </td>
                <td>EPIC-10</td>
            </tr>
            <tr>
                <td>TS-004</td>
                <td>Endpoint Veterinary Clinic</td>
                <td>
                    <strong>Como</strong> desarrollador frontend, 
                    <strong>quiero</strong> poder agregar nuevas clínicas veterinarias a la plataforma y ver una lista de todas las clínicas disponibles
                    <strong>para</strong> que los usuarios puedan encontrar fácilmente servicios veterinarios cercanos.
                </td>
                <td>
                    <h5>Escenario 01: Crear una nueva clínica veterinaria</h5>
                    <strong>Dado</strong> un usuario desea agregar una nueva clínica veterinaria a la plataforma.
                    <strong>Cuando</strong> envía una solicitud POST con los detalles de la nueva clínica veterinaria, incluyendo nombre, ubicación, servicios ofrecidos y horario de atención.
                    <strong>Entonces</strong> el sistema crea la nueva clínica veterinaria en la base de datos y devuelve los detalles de la clínica recién creada con un código de estado 201 (Created).
                    <br>
                    <h5>Escenario 02: Obtener todas las clínicas veterinarias</h5>
                    <strong>Dado</strong> un usuario desea ver todas las clínicas veterinarias disponibles en la plataforma.
                    <strong>Cuando</strong> envía una solicitud GET.
                    <strong>Entonces</strong> el sistema devuelve una lista de todas las clínicas veterinarias registradas en la plataforma con un código de estado 200 (OK).
                    <br>
                    <h5>Escenario 03: Filtrar clínicas veterinarias por ubicación o servicios</h5>
                    <strong>Dado</strong> un usuario desea encontrar clínicas veterinarias específicas por ubicación o servicios ofrecidos.
                    <strong>Cuando</strong> envía una solicitud GET con parámetros de consulta para filtrar por ubicación o servicios.
                    <strong>Entonces</strong> el sistema devuelve una lista de clínicas veterinarias que coinciden con los criterios de búsqueda con un código de estado 200 (OK). Si no se encuentran coincidencias, se devuelve una lista vacía.
                </td>
                <td>EPIC-10</td>
            </tr>
            <tr>
                <td>TS-005</td>
                <td>Implementar Seguridad al Iniciar Sesión</td>
                <td>
                    <strong>Como</strong> desarrollador frontend, 
                    <strong>quiero</strong> una capa de seguridad al iniciar sesión
                    <strong>para</strong> evitar que usuarios maliciosos entren a la aplicación.
                </td>
                <td>
                    <h5>Escenario 01: Pregunta exitosa</h5>
                    <strong>Dado</strong> un usuario desea iniciar sesión.
                    <strong>Cuando</strong> responde la pregunta de seguridad.
                      <strong>Y</strong> es correcto.
                    <strong>Entonces</strong> el sistema lo deja acceder.
                    <br>
                    <h5>Escenario 02: Pregunta exitosa</h5>
                    <strong>Dado</strong> un usuario desea iniciar sesión.
                    <strong>Cuando</strong> responde la pregunta de seguridad.
                      <strong>Y</strong> está mal.
                    <strong>Entonces</strong> el sistema no lo deja acceder.
                </td>
                <td>EPIC-10</td>
            </tr>
      </tbody>
</table>

## 3.3. Impact Mapping.

En esta sección, se presenta el Impact Mapping para cada segmento objetivo. Esta técnica permite visualizar cómo las características del producto contribuyen a los objetivos de negocio y cómo se alinean con las necesidades de los usuarios.

### Segmento 1: Veterinaria

![Impact Mapping Veterinaria](../assets/impact-mapping-veterinaria.png)

### Segmento 2: Propietario de mascota

![Impact Mapping Propietario de mascota](../assets/impact-mapping-propietario.png)

## 3.4. Product Backlog.

Utilizamos la escala de Fibonacci para la estimación de los Story Points.

<table>
        <thead>
            <tr>
                <th>Orden</th>
                <th>User Story Id</th>
                <th>Título</th>
                <th>Descripción</th>
                <th>Story Points (1/2/3/5/8)</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>US-012</td>
                <td>Navegar en la página principal </td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> acceder a la página principal del sitio web y ver un botón de Call to Action 
                    <strong>para</strong> descargar la aplicación o registrarme, para tener acceso rápido a la funcionalidad principal.
                </td>
                <td>1</td>
            </tr>
            <tr>
                <td>2</td>
                <td>US-015</td>
                <td>Descargar la aplicación</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder descargar la aplicación desde el sitio web estático,
                    <strong>para</strong> instalarla en mi dispositivo y comenzar a usarla.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>3</td>
                <td>US-013</td>
                <td>Ver funcionalidades para propietarios de mascotas</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> ver las funcionalidades que ofrece la aplicación para los dueños de mascotas,
                    <strong>para</strong> saber cómo puedo usarla para cuidar de mi mascota.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>4</td>
                <td>US-014</td>
                <td>Ver funcionalidades para veterinarias</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> ver las funcionalidades que ofrece la aplicación para veterinarias,
                    <strong>para</strong> conocer cómo puedo usarla en mi clínica veterinaria.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>5</td>
                <td>US-011</td>
                <td>Revisar reseñas de la aplicación</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder ver las reseñas de la aplicación,
                    <strong>para</strong> conocer la experiencia de otros usuarios antes de descargarla o registrarme.
                </td>
                <td>3</td>
            </tr>
            <tr>
                <td>6</td>
                <td>US-010</td>
                <td>Ver información del footer</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder acceder a los enlaces del footer,
                    <strong>para</strong> navegar rápidamente a secciones como redes sociales, noticias y contacto.
                </td>
                <td>1</td>
            </tr>
            <tr>
                <td>7</td>
                <td>US-016</td>
                <td>Enviar un mensaje desde el sitio de web estático</td>
                <td>
                    <strong>Como</strong> visitante,
                    <strong>quiero</strong> poder enviar un mensaje al equipo de la aplicación desde la sección de contacto,
                    <strong>para</strong> resolver dudas o recibir más información sobre el servicio.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>8</td>
                <td>US-001</td>
                <td>Registrar Mascota</td>
                <td>
                    <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> crear un perfil para cada una de mis mascotas en la aplicación, ingresando su información básica 
                    <strong>para</strong> mantener un registro organizado de sus datos.
                </td>
                <td>3</td>
            </tr>
            <tr>
                <td>9</td>
                <td>TS-002</td>
                <td>Endpoint Pet</td>
                <td>
                    <strong>Como</strong> desarrollador frontend,
                    <strong>quiero</strong> poder integrar la funcionalidad de agregar y visualizar mascotas en la interfaz de usuario,
                    <strong>para</strong> permitir a los usuarios mantener un registro actualizado de sus mascotas desde la aplicación móvil.
                </td>
                <td>5</td>
            </tr>
            <tr>
                <td>10</td>
                <td>TS-001</td>
                <td>Endpoint Medical History</td>
                <td>
                    <strong>Como</strong> desarrollador front-end,
                    <strong>quiero</strong> acceder a un endpoint en el backend para gestionar el historial médico de las mascotas, incluyendo el registro de enfermedades y vacunaciones asociadas,
                    <strong>para</strong> permitir el manejo completo del historial médico desde la interfaz de usuario.
                </td>
                <td>5</td>
            </tr>
            <tr>
                <td>11</td>
                <td>US-009</td>
                <td>Visualizar resumen del historial médico</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder visualizar el resumen del historial médico de cada mascota,
                    <strong>para</strong> considerar sus antecedentes durante la atención de una consulta.
                </td>
                <td>3</td>
            </tr>
            <tr>
                <td>12</td>
                <td>TS-004</td>
                <td>Endpoint Veterinary Clinic</td>
                <td>
                    <strong>Como</strong> desarrollador frontend,
                    <strong>quiero</strong> poder agregar nuevas clínicas veterinarias a la plataforma y ver una lista de todas las clínicas disponibles,
                    <strong>para</strong> que los usuarios puedan encontrar fácilmente servicios veterinarios cercanos.
                </td>
                <td>5</td>
            </tr>
            <tr>
                <td>13</td>
                <td>US-017</td>
                <td>Mostrar tu ubicación actual</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan,
                    <strong>quiero</strong> poder visualizar mi ubicación,
                    <strong>para</strong> buscar centros de atención cerca de mi ubicación.
                </td>
                <td>3</td>
            </tr>
            <tr>
                <td>14</td>
                <td>US-023</td>
                <td>Añadir ubicación</td>
                <td>
                    <strong>Como</strong> veterinaria o personal autorizado de la clínica veterinaria,
                    <strong>quiero</strong> añadir la ubicación de mi centro de atención,
                    <strong>para</strong> mostrar la ubicación actual de mi centro de atención.
                </td>
                <td>3</td>
            </tr>
            <tr>
                <td>15</td>
                <td>TS-003</td>
                <td>Endpoint User</td>
                <td>
                    <strong>Como</strong> desarrollador frontend,
                    <strong>quiero</strong> poder crear y obtener información sobre diferentes tipos de usuarios en la plataforma,
                    <strong>para</strong> gestionar eficazmente las cuentas de los usuarios desde la interfaz de usuario de la aplicación móvil.
                </td>
                <td>5</td>
            </tr>
            <tr>
                <td>16</td>
                <td>US-005</td>
                <td>Registrar vacunas</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder registrar las vacunas administradas a cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>17</td>
                <td>US-006</td>
                <td>Registrar resultados</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder registrar los resultados de análisis obtenidos de cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>18</td>
                <td>US-007</td>
                <td>Registrar cirugías</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> registrar un reporte de los resultados de cirugías realizadas en cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>3</td>
            </tr>
            <tr>
                <td>19</td>
                <td>US-008</td>
                <td>Registrar enfermedades</td>
                <td>
                    <strong>Como</strong> veterinario o personal autorizado,
                    <strong>quiero</strong> poder registrar las enfermedades diagnosticadas en cada mascota,
                    <strong>para</strong> mantener un historial médico completo y actualizado.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>20</td>
                <td>US-015</td>
                <td>Ver detalles de cada veterinaria</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan,
                    <strong>quiero</strong> poder visualizar la información de cada veterinaria,
                    <strong>para</strong> poder elegir con mayor eficacia la veterinaria acorde a mis necesidades.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>21</td>
                <td>US-022</td>
                <td>Entrar al perfil de cada veterinaria</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan,
                    <strong>quiero</strong> visualizar información personal de cada veterinaria,
                    <strong>para</strong> poder informarme mejor acerca de cada veterinaria.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>22</td>
                <td>US-002</td>
                <td>Subir foto de la mascota</td>
                <td>
                    <strong>Como</strong> propietario de mascota,
                    <strong>quiero</strong> poder subir una foto de mi mascota a la plataforma,
                    <strong>para</strong> poder personalizar su perfil y compartir su imagen con las veterinarias.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>23</td>
                <td>US-003</td>
                <td>Ver listado de mis mascotas</td>
                <td>
                    <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> poder ver un listado de todas mis mascotas registradas en la aplicación,
                    <strong>para</strong> tener un acceso rápido a su información y gestionarlas de manera eficiente.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>24</td>
                <td>US-004</td>
                <td>Editar información de la mascota</td>
                <td>
                    <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> poder editar la información del perfil de mi mascota en la aplicación,
                    <strong>para</strong> mantener actualizada la información de mis mascotas.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>25</td>
                <td>US-018</td>
                <td>Ver las valoraciones y comentarios de la veterinaria</td>
                <td>
                    <strong>Como</strong> veterinario/a o personal autorizado de la clínica veterinaria,
                    <strong>quiero</strong> poder visualizar las valoraciones y comentarios de mi veterinaria,
                    <strong>para</strong> mejorar en los aspectos negativos que pueda tener.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>26</td>
                <td>US-021</td>
                <td>Ver reseñas y evaluación</td>
                <td>
                    <strong>Como</strong> propietario/a o autenticado y suscrito a un plan,
                    <strong>quiero</strong> visualizar las reseñas de cada veterinaria,
                    <strong>para</strong> facilitar el proceso de selección de cada centro.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>27</td>
                <td>US-019</td>
                <td>Añadir valoraciones y comentarios</td>
                <td>
                    <strong>Como</strong> propietario/a de mascota autenticado y suscrito a un plan,
                    <strong>quiero</strong> poder realizar comentarios y valoraciones,
                    <strong>para</strong> calificar la atención de cada centro de atención.
                </td>
                <td>2</td>
            </tr>
<tr>
                <td>28</td>
                <td>US-024</td>
                <td>Registro de cuenta</td>
                <td>
                    <strong>Como</strong> veterinario o propietario de una mascota
                <strong>quiero</strong> registrarme en la aplicación 
                <strong>para</strong> acceder a sus funcionalidades.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>29</td>
                <td>US-025</td>
                <td>Iniciar Sesión</td>
                <td>
                    <strong>Como</strong> veterinario o propietario de una mascota 
                    <strong>quiero</strong> poder iniciar sesión en la aplicación utilizando mis credenciales 
                    <strong>para</strong> acceder a las funcionalidades y gestionar la información ingresada.
                </td>
                <td>2</td>
            </tr>
            <tr>
                <td>30</td>
                <td>US-026</td>
                <td>Cerrar Sesión</td>
                <td>
                    <strong>Como</strong> veterinario o propietario de una mascota 
                        <strong>quiero</strong> tener la capacidad de cerrar sesión en la aplicación 
                        <strong>para</strong> garantizar la seguridad de mi información y proteger mi privacidad.
                </td>
                <td>2</td>
            </tr>
               <tr>
                <td>31</td>
                <td>US-027</td>
                <td>Agendar una cita</td>
                <td>
                    <strong>Como</strong> propietario de una mascota, 
                        <strong>quiero</strong> poder agendar una cita en la clínica veterinaria a través de la aplicación, 
                        <strong>para</strong> asegurar la atención médica oportuna para mi mascota.
                </td>
                <td>5</td>
            </tr>
              <tr>
                <td>32</td>
                 <td>US-028</td>
                <td>Acceso de la veterinaria a la información de la mascota</td>
                <td>
                    <strong>Como</strong> veterinario,
                    <strong>quiero</strong> poder acceder a la información completa de una mascota, incluyendo su historial médico, vacunas y tratamientos previos,
                    <strong>para</strong> brindar una atención adecuada durante una consulta veterinaria.
                </td>
                <td>2</td>
            </tr>
               <tr>
                <td>33</td>
                <td>US-029</td>
                <td>Ver historial de citas</td>
                <td>
                    <strong>Como</strong> propietario de una mascota,
                    <strong>quiero</strong> poder ver el historial completo de citas veterinarias de mi mascota, incluyendo fechas, horarios y propósito de la visita,
                    <strong>para</strong> tener un registro completo de la atención recibida.
                </td>
                <td>2</td>
            </tr>
              <tr>
                <td>34</td>
                 <td>US-030</td>
                <td>Confirmar cita</td>
                <td>
                    <strong>Como</strong> propietario de mascota,
                    <strong>quiero</strong> poder confirmar una cita veterinaria previamente agendada,
                    <strong>para</strong> asegurarme de que la cita está programada y evitar confusiones.
                </td>
                <td>2</td>
            </tr>
              <tr>
                <td>35</td>
                 <td>TS-005</td>
                <td>Implementar Seguridad al Iniciar Sesión</td>
                <td>
                    <strong>Como</strong> desarrollador frontend, 
                    <strong>quiero</strong> una capa de seguridad al iniciar sesión
                    <strong>para</strong> evitar que usuarios maliciosos entren a la aplicación.
                </td>
                <td>2</td>
            </tr>
        </tbody>
</table>
