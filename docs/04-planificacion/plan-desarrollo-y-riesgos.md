# Plan inicial de desarrollo y riesgos

> Borrador para validación del equipo. El repositorio no contiene estimaciones,
> fechas detalladas, presupuesto ni acuerdos de integración; no se inventan en
> este plan.

## Orden de trabajo propuesto

Las responsabilidades sugeridas se basan en los roles descritos en
`equipo/roles-y-acuerdos.md`. El equipo debe confirmar cada asignación y aportar
estimaciones y fechas.

| Orden | Tarea / entregable | Responsable sugerido | Depende de | Estimación y fecha |
|---|---|---|---|---|
| 1 | Confirmar usuarios, problema, evidencia y alcance del MVP. | Alex Vásquez Pérez, coordinador | Ninguna | Pendiente del equipo. |
| 2 | Especificar requisitos, criterios de aceptación y datos del formulario. | Alex Vásquez Pérez y Cristián García Bustamante | 1 | Pendiente del equipo. |
| 3 | Definir fuentes de mercado, permisos y tratamiento de datos. | Alex Vásquez Pérez y Nelson Zapata Jiménez | 1 y 2 | Pendiente del equipo. |
| 4 | Validar OmniRoute y documentar el método y los casos de prueba de cálculos. | Nelson Zapata Jiménez | 2 y 3 | Pendiente del equipo y de autorización docente. |
| 5 | Aprobar el diseño técnico y contratos entre componentes. | Nelson Zapata Jiménez y Cristián García Bustamante | 2, 3 y 4 | Pendiente del equipo. |
| 6 | Implementar las funciones aprobadas del MVP. | Nelson Zapata Jiménez (motor/API) y Cristián García Bustamante (interfaz) | 5 y autorización docente | Pendiente del equipo. |
| 7 | Integrar, probar con criterios acordados y corregir defectos. | Cristián García Bustamante, con el equipo | 6 | Pendiente del equipo. |
| 8 | Completar documentación y preparar evidencia/presentación. | Alex Vásquez Pérez, con el equipo | Resultados de 1–7 | Pendiente del equipo. |

No hay fechas de inicio, duración por tarea, capacidad semanal ni presupuesto
en el repositorio. El hito mencionado en el README es la presentación del
24 de octubre de 2026; no se infiere de ese dato un cronograma completo.

## Dependencias y posibles bloqueos

- La aprobación del docente precede al inicio del desarrollo en `src/`.
- La selección de fuentes y permisos puede bloquear la investigación de mercado.
- La validación de OmniRoute puede bloquear el análisis con IA.
- La definición de fórmulas y casos de referencia puede bloquear los cálculos.
- Los requisitos y contratos entre componentes deben acordarse antes de la
  integración.

Las dependencias son una propuesta lógica basada en las funciones planeadas;
el equipo debe confirmarlas al elaborar el Gantt.

## Integración y revisión: acuerdo pendiente

El archivo de roles y acuerdos declara que los acuerdos aún están pendientes.
Se propone que el equipo revise cambios antes de integrarlos a la rama de
trabajo principal, mantenga decisiones y requisitos documentados, y que
Cristián coordine la revisión de calidad mientras Alex confirma el alcance.
Este mecanismo no debe considerarse un acuerdo hasta que el equipo lo apruebe.

## Riesgos principales y mitigación propuesta

| Riesgo | Señal o impacto | Mitigación propuesta | Estado |
|---|---|---|---|
| No disponer de datos de mercado fiables o autorizados. | El informe no puede respaldar competencia, precios o tendencias. | Identificar y revisar fuentes y permisos antes de depender de ellas; registrar fuente, fecha y limitaciones de cada dato. | Pendiente de investigación. |
| El LLM generar análisis incorrectos o difíciles de verificar. | Recomendaciones engañosas, resultados inconsistentes o incumplimiento del tiempo. | Probar casos representativos, separar resultados generados de cálculos fijos y definir revisión/limitaciones visibles. | Pendiente de validación de OmniRoute y de criterios. |
| El alcance o las integraciones exceder el tiempo y capacidad disponibles. | Retrasos en el MVP, integración o pruebas. | Priorizar el MVP, validar temprano las dependencias y estimar las tareas con el equipo antes de fijar fechas. | No hay estimaciones en el repositorio. |

## Continuidad si una persona clave no está disponible

El repositorio no contiene un plan acordado de reemplazo. Como propuesta, se
recomienda documentar requisitos, fórmulas, decisiones, instrucciones de
prueba y estado de cada tarea; asignar una persona de respaldo por componente;
y hacer revisiones cruzadas periódicas. El equipo debe acordar cómo aplicar
esta propuesta.

## Próxima planificación necesaria

Para convertir este esquema en un Gantt ejecutable, el equipo debe añadir
duraciones, fechas, disponibilidad, dependencias confirmadas y hitos de
desarrollo, integración, pruebas, correcciones y documentación.
