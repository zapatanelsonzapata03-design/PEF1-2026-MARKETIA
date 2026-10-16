# Plan de validación estadística y funcional

> Plan propuesto; no hay participantes, mediciones ni resultados registrados.
> Confirmar con el equipo y el docente antes de recopilar datos.

## Propósitos

- Medir tiempo y proporción de ejecuciones que cumplen OE1.
- Verificar exactitud aritmética frente a casos revisados (OE2).
- Evaluar utilidad y transparencia del FODA/demanda (OE3).
- Medir éxito de tareas y satisfacción de usuarios (OE4).
- Calcular costo por informe y contrastar disposición de pago (OE5).

Los indicadores y umbrales propuestos están descritos en
`docs/02-requisitos/objetivos.md`.

## Muestra y recolección

| Evaluación | Muestra propuesta | Método y dato que se registraría |
|---|---:|---|
| Problema y disposición de pago | Al menos 8 emprendedores de Cochabamba | Entrevista breve o encuesta; preguntas y salvaguardas en `docs/07-evidencias/registro-entrevistas.md`. |
| Usabilidad | 5 emprendedores | Observar si completan el flujo sin ayuda y registrar satisfacción en escala 1–5. |
| Rendimiento | 20 ejecuciones | Medir desde “Enviar” hasta informe visible; registrar latencia y resultado por ejecución. |
| Cálculos | 10 casos de referencia | Comparar resultado del sistema con cálculo independiente y tolerancia de ±0,01 Bs. |
| Calidad de IA | 10 ideas y 3 evaluadores | Rúbrica 1–5 en coherencia, relevancia local, supuestos visibles y utilidad. |

Los tamaños anteriores son propuestas del paquete; requieren ratificación.
Definir la selección de participantes, fechas, entorno, quién evalúa y cómo
tratar datos faltantes antes de empezar. No se deben registrar datos personales
innecesarios.

## Hipótesis y análisis propuestos

- **OE1:** proporción de ejecuciones que terminan en ≤ 5 minutos. Umbral
  propuesto: al menos 18 de 20. Reportar numerador, denominador y proporción.
- **OE4:** proporción de participantes que completa el flujo sin ayuda.
  Umbral propuesto: al menos 4 de 5. Reportar también respuestas de
  satisfacción y limitaciones de la muestra.
- **OE2:** evaluar cada caso por separado y reportar errores absolutos de las
  cantidades monetarias; tolerancia propuesta de ±0,01 Bs.
- **OE3:** calcular resultados de la rúbrica por criterio y evaluador; reportar
  promedio y variabilidad, además del umbral propuesto de 3,5/5.
- **OE5:** registrar costo de generación por informe y respuestas agregadas de
  disposición a pagar; el costo máximo aceptable está pendiente de medición.

Para OE1 y OE4 se propone reportar intervalos de confianza del 95 % para las
proporciones, junto con tamaño de muestra. Dado el tamaño pequeño, elegir y
documentar un método adecuado (por ejemplo, intervalo binomial exacto) y
explicar que estos resultados exploratorios no representan automáticamente a
toda la población de Cochabamba. El equipo debe confirmar el análisis antes de
recopilar datos.

## Reglas de protección de participantes

- Explicar propósito académico y pedir consentimiento antes de participar.
- No solicitar nombre, correo, teléfono, cédula ni dirección exacta.
- Permitir no responder; guardar resultados agregados o códigos no
  identificables.
- No compartir descripciones de negocio con un proveedor externo hasta aprobar
  el aviso, el consentimiento y la revisión de privacidad.
- No incluir datos personales, secretos ni respuestas identificables en
  registros, capturas o repositorio.

## Registro de resultados

`resultados.md` es una plantilla sin mediciones. Completarla solo con datos
reales, indicando fecha, versión, método, tamaño de muestra, resultados,
intervalos cuando correspondan, limitaciones y decisión respecto a cada
umbral.
