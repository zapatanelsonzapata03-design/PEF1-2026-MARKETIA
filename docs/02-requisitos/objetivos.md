# Objetivos y criterios de éxito

El objetivo general registrado en el README es generar, para una idea de negocio
en Cochabamba, un informe de viabilidad con FODA, demanda, costos y punto de
equilibrio en menos de cinco minutos y a un costo accesible.

Los umbrales de la tabla siguiente proceden del paquete de mejoras y son
**propuestas para ratificar**. No son resultados de pruebas ni compromisos
aprobados. OE5 contiene un costo que debe medirse; no se inventa un valor.

| ID | Objetivo específico | Indicador y umbral propuesto | Evidencia necesaria |
|---|---|---|---|
| OE1 | Generar el informe con rapidez. | Al menos 18 de 20 ejecuciones (90 %) terminan en 5 minutos o menos, desde el envío hasta que el informe aparece. | Registro de 20 ejecuciones, condiciones y versión evaluada. |
| OE2 | Entregar cálculos reproducibles. | Coincidencia en 10 casos de referencia, con tolerancia de ±0,01 Bs en resultados monetarios. | Fórmulas aprobadas, casos y resultados revisados independientemente. |
| OE3 | Entregar orientación FODA/demanda útil y transparente. | Promedio de al menos 3,5/5 en una rúbrica de coherencia, relevancia local, supuestos visibles y utilidad para actuar, con 3 evaluadores y 10 ideas. | Rúbrica, evaluadores, casos y evaluaciones documentadas. |
| OE4 | Permitir completar el flujo sin ayuda. | Al menos 4 de 5 emprendedores completan el flujo sin ayuda y la satisfacción media es al menos 4/5. | Protocolo, observaciones y respuestas de 5 participantes. |
| OE5 | Mantener un costo accesible. | Costo de generación por informe ≤ Bs **pendiente de medir**; precio objetivo definido con datos de la encuesta. | Resultado de la prueba de viabilidad y respuestas de usuarios. |

## Trazabilidad

| Problema planteado | Objetivo | Solución propuesta | Resultado esperado |
|---|---|---|---|
| Decidir sin conocer el punto de equilibrio ni los riesgos. | OE2 y OE3 | Cálculos deterministas, FODA y estimación de demanda con supuestos visibles. | La persona usuaria puede revisar el punto de equilibrio y los riesgos identificados. |
| Obtener un análisis puede tomar tiempo y dinero. | OE1 y OE5 | Generación del informe en el tiempo meta y medición del costo por informe. | Informe disponible dentro del umbral y costo medido para compararlo con la disposición de pago. |
| Las herramientas pueden no responder al contexto local. | OE3 y OE4 | Interfaz en español, moneda Bs y pruebas con el grupo prioritario en Cochabamba. | Resultados evaluados en el contexto definido y flujo completado por usuarios de prueba. |

## Cómo evaluar el éxito

El proyecto alcanzaría los criterios propuestos si OE1–OE5 cumplen sus umbrales
con evidencia registrada en `docs/05-estadistica/resultados.md`. Ese archivo
existe como plantilla, pero todavía no contiene mediciones. Antes de recopilar
datos, el equipo debe ratificar umbrales, participantes, métodos y condiciones
de prueba.

Para OE1 y OE4, el informe estadístico debe incluir tamaño de muestra,
proporción observada e intervalo de confianza del 95 %. Con muestras pequeñas,
se debe especificar un método apropiado y describir la incertidumbre; un
resultado de prueba no demuestra por sí solo que el comportamiento se
generalice a toda la población.
