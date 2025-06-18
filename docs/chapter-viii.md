# Capítulo VIII: Experiment-Driven Development
## 8.1. Experiment Planning

### 8.1.1. As-Is Summary

La aplicación actual se centra en ofrecer una plataforma para facilitar el contacto de veterinarios para tratar sus mascotas, proporcionando funcionalidades básicas como la gestión de perfiles de usuarios, reportes médicos y datos de los animales, y un sistema de recordatorios para citas agendadas con el veterinario. Sin embargo, el rendimiento general es inconsistente, con la función de elección de ubicación funcionando irregularmente, y cambios no mostrándose hasta actualizar la página, lo que afecta la experiencia del usuario. La interfaz presenta limitaciones en términos de personalización, y no se adapta adecuadamente a diferentes condiciones de luz.

### 8.1.2. Raw Material: Assumptions, Knowledge Gaps, Ideas, Claims
**Assumptions:**
- *Modo Oscuro*: Se asume que los usuarios valoran que el diseño de la interfaz se acomode a sus preferencias visuales.

- *Olvido de vacunación*: Se asume que muchos dueños de mascotas olvidan las fechas de vacunación si no cuentan con recordatorios automáticos.

**Knowledge Gaps:**
- *Preferencias de Interfaz*: Falta información sobre las preferencias que tienen los usuarios respecto al diseño de la interfaz.

- *Frecuencia del olvido*: No se tiene información precisa sobre cuántos usuarios han olvidado citas o vacunas importantes para sus mascotas.

**Ideas:**
- *Entrevistas*: Realizar entrevistas a los usuarios, en los que preguntamos y recolectamos información sobre sus preferencias.

- *Funcionalidad de recordatorios*: Implementar una funcionalidad que envíe notificaciones automáticas antes de las fechas de vacunación, y medir su impacto con encuestas o métricas de cumplimiento.

**Claims:**
- *Experiencia más cómoda*: Se afirma que el Modo Oscuro proporcionará una experiencia más cómoda a los usuarios.

- *Mejora de cumplimiento*: Se afirma que al incluir recordatorios automáticos de vacunación, se mejora la salud preventiva de las mascotas y se reduce el riesgo de enfermedades comunes.

### 8.1.3. Experiment-Ready Questions

| Question | Confidence | Risk | Impact | Interest | Total Score |
|----------|------------|------|--------|----------|--|
| ¿Un Modo Oscuro mejoraría la experiencia? | 8 - Varias aplicaciones lo tienen, y el porcentaje de uso es notable. | 2 - Bajo riesgo, ya que es una funcionalidad sencilla de colores | 5 - Mejora la experiencia, pero no es esencial. | 5 - Interés moderado en los usuarios. | 20 |
| ¿La implementación de recordatorios de vacunación aumentará el cumplimiento del calendario de salud de las mascotas? | 7 – Es una práctica común en apps de salud y organización, pero no tenemos datos específicos de nuestros usuarios aún. | 3 – Riesgo bajo-moderado: requiere integración con historial médico y sistema de notificaciones. | 8 – Tiene alto impacto en la salud de las mascotas y fidelización de usuarios. | 7 – Alta probabilidad de interés: dueños responsables valoran el cuidado preventivo. | 25 |
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

### 8.1.4. Question Backlog

| Prioridad | Pregunta |
|-----------|----------|
| 1 | ¿Un Modo Oscuro mejoraría la experiencia? |
| 2 | ¿Los recordatorios ayudarán a que los dueños de mascotas cumplan a tiempo con las vacunas? |
|  |  |
|  |  |
|  |  |

### 8.1.5. Experiment Cards

| Question | ¿Un Modo Oscuro mejoraría la experiencia? |
|----------|-----------|
| Why | Al agregar un modo oscuro, la visibilidad y comodidad de la interfaz sería mayor para los usuarios que prefieran estos colores, especialmente en ambientes de luz baja. |
| What | Implementar un botón que cambie entre ambos modos de color. |
| Hypothesis | Se espera que, al añadir el modo oscuro, el tiempo de uso de la aplicación por parte del 50% de los usuarios aumente en un 30%. |

| Question | ¿Los recordatorios ayudarán a que los dueños de mascotas cumplan a tiempo con las vacunas? |
|----------|-----------|
| Why | Porque muchos usuarios no llevan un control estricto del calendario de vacunación de sus mascotas, lo que puede afectar su salud. Un recordatorio automático podría ayudarles a no olvidar fechas importantes. |
| What | Implementar una funcionalidad que permita registrar fechas de vacunación y enviar notificaciones previas al usuario (por ejemplo, 3 días antes, 1 día antes y el mismo día). |
| Hypothesis | Se espera que, con los recordatorios activos, al menos el 60% de los usuarios registrados con mascotas vacunadas cumplan sus citas a tiempo durante el primer mes. |

# 8.2. Experiment Design
### 8.2.1. Experiment Cards

|  | Hypothesis |
|--|-----------|
| Question | ¿Un Modo Oscuro mejoraría la experiencia? |
| Belief | Al agregar un modo oscuro, la visibilidad y comodidad de la interfaz sería mayor para los usuarios que prefieran estos colores, especialmente en ambientes de luz baja. |
| Hypothesis | Se espera que, al añadir el modo oscuro, el tiempo de uso de la aplicación por parte del 50% de los usuarios aumente en un 30%. |
| Null Hypothesis | Al añadir el modo oscuro, el tiempo de uso de la aplicación por parte del 50% de los usuarios no se verá afectada en gran medida. |

|  | Hypothesis |
|--|-----------|
| Question | ¿Los recordatorios automáticos ayudarán a que los dueños de mascotas cumplan a tiempo con las vacunas? |
| Belief | Muchos usuarios olvidan las fechas de vacunación de sus mascotas. Al ofrecer recordatorios automáticos, facilitamos el cumplimiento del calendario de salud preventiva. |
| Hypothesis | Se espera que, al implementar los recordatorios, al menos el 60% de los usuarios con mascotas registradas completen sus vacunas programadas en la fecha estimada durante el primer mes. |
| Null Hypothesis | La implementación de recordatorios no generará un cambio significativo en el cumplimiento de las fechas de vacunación programadas por los usuarios.|

### 8.2.2. Measures

| Question | ¿Un Modo Oscuro mejoraría la experiencia? |
|----------|-----------|
| Measure | Medir el tiempo de uso de los usuarios, registrando los tiempos de inicio de sesión, y su cierre correspondiente. Sacando un promedio de la mitad de los usuarios, se evaluará su impacto. |

| Question | ¿Los recordatorios automáticos ayudarán a que los dueños de mascotas cumplan a tiempo con las vacunas?  |
|----------|-----------|
| Measure | Medir la cantidad de vacunas registradas como "cumplidas a tiempo", comparando el comportamiento de los usuarios antes y después de habilitar los recordatorios. También se pueden usar encuestas de percepción sobre la utilidad del sistema.|

### 8.2.3. Conditions

| Question | ¿Un Modo Oscuro mejoraría la experiencia? |
|----------|-----------|
| Condición Experimental | El tiempo de uso aumentará en un 30%, medido a través de registros de tiempo de sesión. |
| Condición de Control | No habrá un aumento significativo del tiempo de uso por parte de los usuarios. |

| Question | 	¿Los recordatorios automáticos ayudarán a que los dueños de mascotas cumplan a tiempo con las vacunas de sus animales? |
|----------|-----------|
| Condición Experimental | 	El porcentaje de cumplimiento de vacunas a tiempo será igual o mayor al 60% entre los usuarios que recibieron recordatorios. |
| Condición de Control | 	El porcentaje de cumplimiento de vacunas a tiempo se mantendrá igual o por debajo del comportamiento base (< 40%) en usuarios sin recordatorios. |

### 8.2.4. Scale Calculations and Decisions.
<table>
  <tr>
    <td rowspan="2"><strong>Scale Calculation</strong></td>
    <td rowspan="2"><strong>Decision</strong></td>
    <td colspan="4"><strong>Factor</strong></td>
  </tr>
  <tr>
    <td>Desfavorable</td>
    <td>Aceptable</td>
    <td>Ideal</td>
    <td>Excelente</td>
  </tr>
  <tr>
    <td>Creemos que, al añadir el modo oscuro, la comodidad visual de los usuarios aumentará en un 30%. Sabremos que esto es cierto cuando el tiempo de uso de la aplicación por parte del 50% de los usuarios aumente en un 30%.</td>
    <td>Implementaremos un botón en el menú lateral de la aplicación que, al presionarse, intercambiaré entre modos de color.</td>
    <td></td>
    <td></td>
    <td></td>
    <td>X</td>
  </tr>
</table>
### 8.2.5. Methods Selection.

| Herramienta | Google Analytics | Catchpoint | Amazon Redline13 | Lighthouse |
|-------------|------------------|------------|------------------|------------|
| Precio | Plan gratis, y plan de pago en base a uso. |  |  |  |
| Análisis | Análisis de tráfico y uso de usuarios. |  |  |  |
| Facilidad de Uso | Interfaz detallada, pero manejable. |  |  |  |
| Ventajas | Amplia integración con otros servicios, y gran capacidad de generación de reportes. |  |  |  |

### 8.2.6. Data Analytics: Goals, KPIs and Metrics Selection.

Se llevaron a cabo pruebas de rendimiento, accesibilidad y mejores prácticas con Lighthouse en nuestra aplicación UPet para evaluar su desempeño y optimizar la experiencia de usuario:

### 8.2.7. Web and Mobile Tracking Plan.

Como se busca una optimización y mejora continua de la plataforma UPet, se monitorearán una serie de datos importantes durante el uso de la aplicación Web y aplicación Móvil por parte de los usuarios. Para eso, establecemos un plan compuesto por los siguientes pasos:

1. 

## Capítulo IX: Bibliografía

1. **Tull Soriano, Luis Federico.** *Prototipo de monitor de signos vitales en pacientes veterinarios de especie canina utilizando IoT.* Universidad Nacional Pedro Henríquez Ureña, 2021. [https://repositorio.unphu.edu.do/handle/123456789/3485](https://repositorio.unphu.edu.do/handle/123456789/3485)

2. **Grados Denegri, Felipe Alfredo, y Freddy Hernan Rodriguez Vega.** *Aplicativo móvil para la gestión de servicios clínicos veterinarios en Lima - Metropolitana.* Universidad Autónoma del Perú, 2021. [https://repositorio.autonoma.edu.pe/handle/20.500.13067/1079](https://repositorio.autonoma.edu.pe/handle/20.500.13067/1079)

## Capítulo X: Anexo

- **Landing Page:** [Enlace al landing page](https://pet-heart-health.github.io/landing-page-upet/)
- **Web Frontend:** [Enlace al proyecto web](https://frontend-app-upet.netlify.app)
- **Aplicación Móvil:** [Enlace al proyecto móvil](URL_DEL_MOBILE)
- **Backend:** [Enlace al backend](https://backend-app-upet-production.up.railway.app/docs#)
- **Mockups:** [Enlace a los mockups](https://www.figma.com/design/HG5VxSXVvjfVC0BGdiWywi/IOT---Mobile-Application?node-id=0-1&node-type=canvas&t=WLj5vcz6RIZRcTvT-0)
- **Prototipo:** [Enlace a los mockups](https://www.figma.com/proto/HG5VxSXVvjfVC0BGdiWywi/IOT---Mobile-Application?node-id=64-5609&node-type=canvas&t=WLj5vcz6RIZRcTvT-0&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=64%3A5606&show-proto-sidebar=1)
- **Vídeo TP:** [Enlace al vídeo](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202216558_upc_edu_pe/Eazd8BrgjJNBkK0j-dDMHiYBwBIH0VsMdtIp7s9Gd1zaLQ?e=h2Gugv)
