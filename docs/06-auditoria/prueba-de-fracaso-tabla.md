# Prueba de fracaso: tabla de condiciones, señales y controles

**Corte: 22 de octubre de 2026** · Responde las preguntas 51 y 52 del cuestionario.

> Los riesgos (R1 a R8) vienen del
> [plan de desarrollo](../04-planificacion/plan-desarrollo-y-riesgos.md) y de
> [`prueba-de-fracaso.md`](prueba-de-fracaso.md). El **estado** describe la
> evidencia que existe hoy; no se marca "En marcha" sin un archivo o captura
> que lo pruebe. Actualizar cada viernes en la reunión.

**Estados permitidos:** `Con evidencia` · `Evidencia parcial, revisión pendiente` · `Propuesto, sin evidencia` · `Pendiente de autorización` · `Sin control`

| N.º | Condición de fracaso | Riesgo | Señal temprana | Control | Evidencia (archivo o captura) | Estado hoy | Responsable |
|---:|---|---|---|---|---|---|---|
| 1 | El alcance excede el tiempo y el equipo no llega al 80 % del 24/11 | R1 | Tareas atrasadas más de 2 días | MVP acotado, revisión del Gantt cada lunes, recorte del 40 % | [`plan-desarrollo-y-riesgos.md`](../04-planificacion/plan-desarrollo-y-riesgos.md); falta acta con horas confirmadas | Propuesto, sin evidencia | Alex |
| 2 | La IA produce contenido inválido, inventado o lento | R2 | Fallos en la prueba de viabilidad; formato JSON inválido | Prueba de 10 ideas, validación de esquema, cálculos disponibles aunque falle la IA | [`registro-prueba-viabilidad.md`](../07-evidencias/registro-prueba-viabilidad.md) sin completar; Anexo B del informe (1 caso) | Pendiente de autorización | Nelson |
| 3 | Los cálculos son incorrectos | R2 | Diferencia mayor a ±0,01 Bs frente a un caso revisado | 10 casos de referencia, pruebas unitarias, 3 negocios reales | [`revision-formulas-borrador.md`](../03-arquitectura/revision-formulas-borrador.md): recálculo aritmético preliminar; falta revisión independiente documentada y casos reales | Evidencia parcial, revisión pendiente | Nelson y Cristián |
| 4 | Se confunden estimaciones de IA con hechos | R2 | El informe muestra FODA sin etiqueta | Etiqueta "Estimación generada por IA, no es un dato verificado" y supuestos visibles (RNF-03) | Requisito escrito; sin implementar | Propuesto, sin evidencia | Cristián |
| 5 | No se valida que el problema exista ni que el precio sea accesible | R3 | Menos de 8 entrevistas verificadas; falta de cotizaciones | Entrevistas documentadas, 2 cotizaciones, referencias verificadas | [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md): ocho resúmenes reportados, sin fichas completas ni evidencia de consentimiento/autorización. Las [capturas de solicitud](../07-evidencias/guion-cotizaciones.md) no muestran respuestas ni prueban dos proveedores distintos | Evidencia parcial, revisión pendiente | Cristián y Alex |
| 6 | Poca gente quiere pagar | R3 | Disposición de pago menor al precio propuesto | Nivel gratuito, alianzas con universidades, pregunta de pago en las entrevistas | Pregunta incluida en el protocolo; los resúmenes aportados no informan montos de disposición de pago | Propuesto, sin evidencia | Cristián y Alex |
| 7 | Las cuotas gratuitas de IA se agotan o cambian | R4 | Errores o límites en OmniRoute | Evaluar proveedores compatibles y documentar respaldo sin secretos | Anexo B muestra evidencia preliminar de un caso/topología; no acredita proveedor de respaldo ni conmutación | Propuesto, sin evidencia | Nelson |
| 8 | Falta una persona clave o el equipo se desorganiza | R5 | Ausencia o retraso de un integrante | Respaldos cruzados, Trello, flujo Git, reuniones L-M-V | [`roles-y-acuerdos.md`](../../equipo/roles-y-acuerdos.md); faltan acta, Trello y captura de `main` | Propuesto, sin evidencia | Alex |
| 9 | El docente no autoriza a tiempo | R6 | No consta respuesta escrita a la solicitud | Registrar solicitud y respuesta; mientras tanto, solo documentación y `src/` vacío | [`solicitud-autorizacion-docente.md`](../07-evidencias/solicitud-autorizacion-docente.md) documenta el envío del enlace, no una respuesta | Pendiente de autorización | Alex |
| 10 | Se exponen datos personales o un secreto | R7 | Datos reales en pruebas sin consentimiento; claves en el repo | No pedir datos personales, aviso y consentimiento, `.env` fuera del repo | `.gitignore` excluye `.env`; D6 por ratificar | Evidencia parcial, revisión pendiente | Nelson |
| 11 | Las respuestas varían por modelo o sube el costo de IA o del dólar | R8 | Variación entre ejecuciones; cambio de precios | Orden fijo de proveedores, plantillas iguales, límites por usuario, revisión mensual de costos | Ninguna | Propuesto, sin evidencia | Nelson |
| 12 | Las referencias del informe no se sostienen (enlaces rotos o cifras que no coinciden) | R3 | Enlace que no abre; cifra distinta a la fuente | Verificar las 9 fuentes y corregir o quitar lo que no tenga respaldo | [`verificacion-referencias.md`](verificacion-referencias.md) sin completar | Propuesto, sin evidencia | Alex |

## Cómo se actualiza esta tabla

1. Cuando un control tenga archivo o captura, copiar su nombre en la columna "Evidencia" y cambiar el estado a `Con evidencia`.
2. Si un control no se puede aplicar, escribir `Sin control` y qué se hará. Un control falso es peor que uno ausente.
3. Revisar la tabla cada viernes y anotar la fecha del cambio al pie.

| Fecha de revisión | Qué cambió | Quién |
|---|---|---|
| | | |
