# Sección 6: Diseño y viabilidad técnica

**Actualización documental:** 22 de octubre de 2026

**Estado:** propuesta; no describe una implementación ni resultados validados.

Esta sección organiza la arquitectura y las opciones técnicas para su revisión.
Las tecnologías, contratos y proveedores continúan sujetos a ratificación del
equipo. No se debe marcar como aprobado un criterio ni iniciar desarrollo por
la existencia de este documento.

## Estado según la evidencia del repositorio

| Tema | Evidencia disponible | Estado |
|---|---|---|
| Arquitectura | El diagrama y la descripción de componentes están en [`arquitectura-inicial.md`](arquitectura-inicial.md) | Diseño propuesto; decisiones por ratificar |
| Contrato API | La arquitectura propone `POST /analisis` y endpoints auxiliares; no hay implementación | Contrato inicial incompleto, pendiente de ratificación |
| Viabilidad de OmniRoute | El Anexo B del informe final contiene evidencia preliminar de un caso | No equivale a benchmark; diez casos, latencia y costo no están registrados |
| Alternativa ante fallos del proveedor | La arquitectura considera otro proveedor compatible como plan B | Alternativa conceptual; no hay conmutación automática implementada |
| Seguridad y tratamiento de datos | Los controles y datos están descritos como propuestas en [`datos-seguridad-pruebas.md`](datos-seguridad-pruebas.md) | Pendiente de ratificación y validación |
| Latencia y costo | La arquitectura propone una mediana de latencia de hasta 60 segundos y comparar el costo con OE5 | No hay mediciones registradas |
| Autorización | La solicitud registra el envío del enlace del repositorio el 15/10/2026, pero no una respuesta escrita que autorice la prueba o el desarrollo | No consta autorización en la evidencia disponible |

La evidencia de un solo caso incluida en el informe es preliminar. No se afirma
que se haya ejecutado el benchmark de diez ideas ni que existan mediciones de
latencia, tokens o costo. La plantilla para registrar una prueba futura está en
[`../07-evidencias/registro-prueba-viabilidad.md`](../07-evidencias/registro-prueba-viabilidad.md);
solo se completa con autorización correspondiente y mediciones reales.

## Contrato API: alternativas propuestas para ratificación

La arquitectura vigente documenta `POST /analisis` como contrato general. El
material recibido propone dividir las operaciones en estos endpoints:

| Método y ruta propuesta | Responsabilidad conceptual | Estado |
|---|---|---|
| `POST /api/v1/calcular` | Calcular margen de contribución y punto de equilibrio mediante fórmulas deterministas | Alternativa de diseño; no implementada |
| `POST /api/v1/analizar-foda` | Solicitar análisis cualitativo y devolver una respuesta estructurada | Alternativa de diseño; no implementada |

La separación entre cálculos fijos y estimaciones de IA coincide con el diseño
general descrito en la arquitectura. Sin embargo, las rutas, campos, tipos,
redondeos, validaciones, errores y estructura de respuesta de estas alternativas
no están ratificados. El equipo debe acordar un único contrato y actualizar la
arquitectura antes de cualquier implementación. No se incluyen aquí ejemplos de
negocios ni resultados que puedan confundirse con pruebas realizadas.

## Respaldo ante fallos de IA

La arquitectura contempla evaluar un proveedor compatible como alternativa.
La selección de proveedores, sus términos, privacidad, costo y desempeño deben
verificarse antes de usarlos. No se afirma que exista un proveedor secundario
configurado, manejo automático de errores ni código de fallback. No incluir
claves, tokens ni archivos de entorno en el repositorio.

## Pendientes de viabilidad

Una vez obtenida la autorización docente aplicable, el equipo puede ejecutar el
protocolo documentado para registrar formato, latencia, costo, fallos y
condiciones de la prueba. El criterio preliminar ya documentado para latencia
es mediana de hasta 60 segundos; el costo debe compararse con OE5. Hasta que se
registren datos observados, ambos aspectos siguen pendientes y no se deben
presentar cifras del material recibido como resultados.

## Correspondencia con la auditoría

La matriz del cuestionario del repositorio conserva sus propios estados y
referencias. El material recibido asigna a P25–P30 descripciones que no
coinciden por completo con la descripción usada en esa matriz (por ejemplo,
P30 aparece allí vinculado a ratificar el contrato API). Por ello, este
documento no cambia los estados de la auditoría ni marca criterios como
“Cumple”. Antes de modificar la correspondencia P25–P30, el equipo debe
contrastar los números con el cuestionario oficial.
