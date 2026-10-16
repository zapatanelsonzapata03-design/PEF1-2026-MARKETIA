# Roles y acuerdos de trabajo

> Las responsabilidades se basan en la información del equipo que ya consta
> en el repositorio; los entregables y acuerdos operativos siguientes son
> propuestas del paquete de mejoras y requieren ratificación en una reunión.

## Responsabilidades y entregables propuestos

| Integrante | Rol | Entregables verificables propuestos | Respaldo propuesto |
|---|---|---|---|
| Alex Vásquez Pérez | Coordinador del proyecto | Registro de decisiones, calendario y actas; referencias y evidencias; informe final y diapositivas. | Cristián García Bustamante en documentación. |
| Nelson Zapata Jiménez | Líder del motor y la IA | Tras autorización docente: contrato y endpoint `/analisis`, motor de cálculos con casos de referencia, integración con LLM y prueba de viabilidad documentada. | Cristián García Bustamante en API y documentación de pruebas. |
| Cristián García Bustamante | Líder de la pantalla y la calidad | Tras autorización docente: formulario, pantalla de informe, protocolo y resultados de pruebas de usabilidad, manual de usuario. | Nelson Zapata Jiménez en interfaz y pruebas cruzadas. |

Nelson concentra varias tareas técnicas en la propuesta; la revisión cruzada y
la documentación buscan reducir el riesgo de dependencia de una sola persona.
Los entregables y respaldos no se consideran acuerdos hasta su ratificación.

## Flujo de trabajo Git propuesto

1. No subir cambios directamente a `main`; solicitar al equipo que configure
   protección de rama si está disponible.
2. Crear ramas por tarea, por ejemplo `feat/<área>-<descripción>` y
   `docs/<descripción>`.
3. Integrar cambios mediante pull request y obtener la aprobación de otro
   integrante.
4. Considerar terminada una tarea cuando cumple su criterio de aceptación,
   tiene las pruebas necesarias y la documentación actualizada.
5. Registrar cada tarea con responsable, estimación y etiqueta; usar un tablero
   solo después de que el equipo confirme la herramienta y su configuración.
6. Acordar una reunión semanal de 30 minutos; el día, hora y canal están
   pendientes.
7. Registrar decisiones ratificadas en `docs/decisiones.md` y distinguirlas de
   propuestas no aprobadas.

Estos pasos son propuestas, no configuración efectiva de GitHub ni acuerdos
ratificados. No se han creado issues, tablero ni protecciones de rama.

## Revisión e integración

Se propone que una persona distinta a quien hizo el cambio revise cada pull
request y compruebe los criterios de aceptación. Para las tareas de motor,
interfaz y documentación, al menos dos integrantes deberían conocer las
decisiones, contratos y pruebas necesarios para continuar el trabajo. El equipo
debe confirmar un mecanismo viable y su frecuencia.

## Continuidad si alguien no está disponible

- Mantener fórmulas, contrato de API, decisiones y casos de prueba
  documentados.
- Usar los respaldos propuestos en la tabla, sujeto a ratificación.
- Realizar revisiones cruzadas para compartir contexto.
- Si Nelson no está disponible, evaluar que Cristián continúe sobre el
  contrato aprobado y las pruebas existentes; reducir alcance solo con acuerdo
  del equipo.

No hay todavía un acta que demuestre aprobación de estos acuerdos.
