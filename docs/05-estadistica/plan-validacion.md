# Plan de validación estadística y funcional

> Plan listo para ratificar; no hay participantes, mediciones ni resultados
> registrados. Confirmar con el equipo y el docente antes de recopilar datos.

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
| Problema y disposición de pago | Al menos 8 emprendedores de Cochabamba | Entrevista semiestructurada; guion y salvaguardas en `docs/07-evidencias/protocolo-entrevistas.md`. |
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

## Tamaño de muestra y regla de decisión (alineado con el informe final)

El informe plantea una prueba piloto de 30 personas y la hipótesis
H₀: p ≤ 0,80 contra H₁: p > 0,80, con nivel de significancia de 0,05
(Z crítico = 1,645). Con esa regla, **el número mínimo de respuestas
favorables** para rechazar H₀ es:

| n (muestra) | Mínimo con aproximación normal | Mínimo con binomial exacto |
|---:|---|---|
| 20 | 19 (95,0 %) | 20 (100,0 %) |
| 30 | 28 (93,3 %) | 28 (93,3 %) |
| 43 | 39 (90,7 %) | 40 (93,0 %) |
| 96 | 84 (87,5 %) | 84 (87,5 %) |

Lectura: con 30 personas, 27 respuestas favorables (90 %) **no bastan** para
afirmar que se superó el 80 %; se necesitan al menos 28 de 30 por la
aproximación normal, y el método exacto es igual o más exigente. Con muestras
menores a 20 no existe resultado que permita rechazar H₀. Si no se alcanza la
muestra, el informe debe **reportar la proporción con su intervalo de confianza
del 95 % y decir que el resultado es exploratorio**, en lugar de afirmar que se
cumplió la meta.

Tamaños de muestra para estimar una proporción con 95 % de confianza y
p = 0,5: n ≈ 96 con margen de error de 10 puntos, y n ≈ 43 con 15 puntos (como
indica el informe).

## Qué se puede afirmar con cada fuente de datos

| Fuente | Muestra | Uso permitido | Uso no permitido |
|---|---:|---|---|
| Entrevistas exploratorias | 8 a 10 | Describir problemas, costos y disposición de pago declarados; orientar el diseño | Estimar porcentajes de toda Cochabamba |
| Pruebas tempranas de usabilidad | 5 | Detectar fallos de uso | Probar hipótesis |
| Prueba piloto | 30 (ideal 43) | Contraste de H₀ con la tabla anterior e IC del 95 % | Generalizar sin mencionar que la muestra es de conveniencia |

## Línea base para la Meta 1 del informe (reducir 70 % el tiempo)
Antes del 13 de noviembre, cronometrar cuánto tarda una persona del equipo en
hacer **a mano** el análisis completo (FODA, demanda, costos y punto de
equilibrio) de 3 negocios de ejemplo, y registrar el tiempo promedio. Ese valor
es la línea base contra la que se mide la reducción.

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
