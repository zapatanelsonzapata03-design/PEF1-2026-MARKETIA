# Revisión preliminar frente al cuestionario de 52 preguntas

**Fecha:** 23 de octubre de 2026 · **Base:** documentos disponibles en el repositorio, capturas de `docs/07-evidencias/` y PDF del cuestionario (Ing. Diego Cárdenas, Programación II - P2).

> Esta es una revisión documental preliminar de consistencia, no una evaluación
> independiente de un docente o de otro integrante. La verificación de
> referencias atribuida a Nelson y las declaraciones de campo se reportan como
> constan en los documentos; este archivo no las valida de forma independiente.

**Criterio.** ✅ Documentado: hay contenido verificable que responde la pregunta. 🟡 Parcial: la respuesta existe, pero falta evidencia real, revisión independiente o ratificación. ❌ Bloquea: falta un requisito previo para iniciar el desarrollo.

## Resultado

**No aprueba todavía.** En esta revisión documental preliminar, 36 de 52 preguntas están documentadas, 14 son parciales y 2 bloquean el inicio (46 y 48). Esta clasificación no es una aprobación docente ni una revisión independiente.

## Matriz

| N.º | Res. | Motivo |
|---:|:-:|---|
| 1, 2, 5 | ✅ | Problema, usuario (D1) y valor definidos en `resumen-del-problema.md` y `objetivos.md` |
| 3 | 🟡 | Ocho resúmenes sin fichas ni consentimiento; cotizaciones sin respuesta; contrastes de referencias reportados por Nelson, aún sin revisión independiente |
| 4 | 🟡 | Consecuencias solo cualitativas y preliminares |
| 6 | 🟡 | Adecuación de la solución sin validar con usuarios (nadie vio el wireframe) |
| 7–10 | ✅ | OE1–OE6 medibles, con trazabilidad y plan de validación |
| 11–18 | ✅ | RF-01 a RF-05, criterios dado/cuando/entonces, RNF-01 a RNF-07, alcance y exclusiones |
| 19 | 🟡 | 112 h de tareas estimadas; disponibilidad reportada de 3 h por persona al día. Faltan días laborables semanales para calcular capacidad y margen; requiere ratificación |
| 20, 21, 24 | ✅ | Recorte del 40 %, MVP v1.0 y versiones posteriores separadas |
| 22 | 🟡 | El valor del MVP no se ha probado con usuarios |
| 23 | 🟡 | Hitos 40 % / 80 % / 100 % definidos, pero dependen de la autorización docente |
| 25 | 🟡 | Sin evidencia de experiencia ni prueba previa con FastAPI, React, PostgreSQL y OmniRoute |
| 26–28 | ✅ | Riesgos técnicos, prueba de viabilidad planificada con umbrales, justificación de tecnologías |
| 29 | 🟡 | Hosting no elegido; `09-accesos-y-hosting.md` sin completar |
| 30 | 🟡 | Dos contratos API en competencia; se propone D16 (`POST /analisis`) y falta ratificar |
| 31 | ✅ | Fuentes y categorías de datos identificadas |
| 32 | 🟡 | Controles descritos, pero D6 sigue sin ratificación |
| 33 | 🟡 | Diez casos sintéticos con recálculo aritmético; revisión independiente, ejecución y casos reales pendientes |
| 34 | ✅ | Estrategia de pruebas documentada; no hay pruebas ejecutadas |
| 35, 37, 39, 40 | ✅ | Gantt A1–A9 y B1–B12 con horas, integración, pruebas, correcciones, documentación y bloqueos |
| 36 | 🟡 | Responsables en el plan, pero Trello no muestra todas las tareas con responsable y fecha |
| 38 | ✅ | Columna "Depende de" completa en el plan |
| 41, 43–45 | ✅ | Roles, tres riesgos principales, mitigaciones y respaldos entre integrantes |
| 42 | 🟡 | Flujo acordado, pero la captura no prueba que la regla aplique a `main` ni hay revisiones individuales |
| 46 | ❌ | Acta 01 en blanco; D1–D16 sin ratificar; sin respuesta escrita del docente; materia sin confirmar (D15) |
| 47 | ✅ | Identifica el requisito que no domina (método de demanda) y su mitigación |
| 48 | ❌ | Sin autorización docente, hosting, cuentas ni acceso confirmado a OmniRoute |
| 49, 50 | ✅ | `09-preparacion.md` y README dicen qué construir primero y qué es el MVP |
| 51 | ✅ | Diez condiciones de fracaso |
| 52 | 🟡 | Controles propuestos, sin comprobar |

## Qué se corrigió en el repositorio

- Referencias: el registro atribuido a Nelson del 22/10 ya estaba en `verificacion-referencias.md`, pero `referencias.md`, el resumen del problema y el README no estaban sincronizados. Se actualizaron para reflejar ese registro, sin presentarlo como verificación independiente. La atribución del 70 % a microempresas informales no coincide con la fuente según ese registro; no hay soporte para la generalización del costo de estudios profesionales, el idioma/precio de herramientas de IA ni el tipo de cambio de Bs 12. Deben corregirse o delimitarse y revisarse por otra persona.
- Se corrigió el texto desactualizado que decía que no había ninguna evidencia local.
- Se agregó la propuesta D16 (contrato único `POST /analisis`) a `decisiones.md` y al acta, para cerrar la duplicidad de contratos de la pregunta 30.

No se modificó `src/` (la preparación no exige código y no hay autorización) ni el PDF del informe.

## Ruta mínima para aprobar (solo acciones reales del equipo)

1. **Acta 01:** reunión de los tres integrantes, completar el acta con los acuerdos reales, confirmaciones individuales y captura. Cierra 46 y mejora 2, 19, 41, 42, 45.
2. **Docente:** enviar `solicitud-autorizacion-docente.md` y guardar su respuesta escrita. Respuesta sobre desarrollo, prueba técnica, entrevistas y materia. Cierra 46, 48 y 23.
3. **Entrevistas:** fichas completas y consentimiento de E01–E08, o repetir con el protocolo. Mejora 3, 4, 6, 22.
4. **Cotizaciones:** dos respuestas reales con precio y plazo. Mejora 3.
5. **Fórmulas:** Cristián revisa y firma los diez casos (`revision-formulas-borrador.md`). Mejora 33.
6. **GitHub:** captura de la regla completa con el patrón `main` y una PR aprobada por otra persona. Cierra 42.
7. **Trello:** todas las tareas A1–A9 y B1–B12 con responsable y fecha. Cierra 36.
8. **Hosting y accesos:** elegir proveedor y completar `09-accesos-y-hosting.md` sin secretos. Cierra 29 y 48.
9. **Informe PDF:** aplicar las correcciones y delimitaciones de referencias y alinear roles con D11.
10. **Prueba de viabilidad de OmniRoute** solo tras la autorización: 10 ideas, registrar formato, tiempo y costo. Cierra 25.

Al completar las acciones 1, 2 y 8 podrían cerrarse los bloqueantes 46 y 48,
además de mejorar los criterios 23 y 29; el resultado debe recalcularse según
la evidencia que efectivamente se reúna. Completar esta lista no garantiza
52/52 ni aprobación final: cada criterio requiere su evidencia y la decisión
corresponde al docente.
