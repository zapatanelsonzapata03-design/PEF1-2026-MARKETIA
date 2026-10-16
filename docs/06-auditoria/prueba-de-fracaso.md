# Prueba de fracaso y controles

Esta tabla convierte riesgos del paquete de mejoras en escenarios comprobables.
Los controles son propuestas, no evidencia de que el riesgo ya esté mitigado.

| El proyecto podría fracasar si… | Control propuesto | Evidencia / estado |
|---|---|---|
| El LLM produce contenido inválido, engañoso o demasiado lento. | Realizar la prueba de viabilidad antes de depender del proveedor, validar el formato, mostrar supuestos y etiquetas, y conservar cálculos disponibles cuando el LLM falle. | Prueba no ejecutada; autorización pendiente. |
| El alcance excede el tiempo disponible. | Ratificar el MVP, estimar tareas y revisar avances semanalmente; usar el recorte de alcance solo si el equipo lo aprueba. | Decisiones y Gantt propuestos; disponibilidad real pendiente. |
| No se valida que el problema exista o que el precio sea accesible. | Revisar referencias y completar entrevistas/encuesta con al menos ocho emprendedores. | Fuentes y respuestas todavía no registradas. |
| Los cálculos son incorrectos. | Ratificar fórmulas, completar diez casos de referencia y ejecutar pruebas unitarias independientes. | Tres ejemplos ilustrativos documentados; siete casos y ejecución pendientes. |
| Las personas usuarias confunden estimaciones con hechos. | Separar visualmente los cálculos de la IA y mostrar la etiqueta “Estimación generada por IA, no es un dato verificado”, junto con los supuestos. | Requisito propuesto, aún no implementado ni probado. |
| El equipo se desorganiza o una persona clave no está disponible. | Acordar flujo Git, documentar contratos y decisiones, asignar respaldo por componente y revisar cambios entre integrantes. | Acuerdo propuesto; ratificación pendiente. |
| Se expone información de usuarios o un secreto. | No pedir datos personales directos, informar el envío al proveedor, minimizar datos, acordar retención/borrado y no almacenar secretos en el repositorio. | Diseño propuesto; revisión de privacidad y controles técnicos pendientes. |
| El docente no autoriza la prueba o el desarrollo a tiempo. | Solicitar la autorización; mientras se espera, trabajar solo en documentación y casos de referencia no sensibles. | No hay respuesta docente registrada. |

Para cada riesgo, el equipo debe ratificar probabilidad, impacto, responsable,
señal temprana y plan alternativo en `docs/04-planificacion/plan-desarrollo-y-riesgos.md`.
