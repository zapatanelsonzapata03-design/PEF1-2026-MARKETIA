# Prueba de fracaso y controles

Cada fila convierte un riesgo en una condición comprobable. Los controles son
propuestas; el estado indica qué evidencia existe hoy. Los riesgos completos
(con probabilidad, señal, responsable y plan B) están en el
[plan](../04-planificacion/plan-desarrollo-y-riesgos.md).

| El proyecto fracasa si… | Riesgo | Control | Responsable | Evidencia / estado | Fecha de revisión |
|---|---|---|---|---|---|
| El LLM produce contenido inválido, engañoso o lento | R2 | Prueba de viabilidad, validación de formato, supuestos y etiquetas visibles, cálculos disponibles aunque falle la IA | Nelson | Prueba no ejecutada; Anexo B del informe (1 caso) | 19 oct |
| El alcance excede el tiempo | R1 | MVP ratificado, recorte del 40 %, revisión del Gantt cada lunes | Alex | Plan y acuerdos propuestos; falta acta | 16 oct |
| No se valida que el problema exista ni que el precio sea accesible | R3 | Entrevistas a 8 o más emprendedores y referencias verificadas | Cristián | Protocolo listo; sin entrevistas | 22 oct |
| Los cálculos son incorrectos | R2 | 10 casos de referencia, pruebas unitarias, 3 negocios reales | Nelson y Cristián | 10 casos sintéticos documentados; falta revisión y casos reales | 21 oct |
| Se confunden estimaciones con hechos | R2 | Etiqueta "Estimación generada por IA, no es un dato verificado" y supuestos visibles | Cristián | Requisito RNF-03; sin implementar | Sprint 2 |
| Cuotas gratuitas de IA se agotan o cambian | R4 | Varios proveedores de respaldo, guardar respuestas repetidas | Nelson | Configuración de OmniRoute (Anexo B) | 19 oct |
| El equipo se desorganiza o falta una persona clave | R5 | Flujo Git, Trello, respaldos cruzados, reuniones L-M-V | Alex | Acuerdos propuestos; falta acta y capturas | 16 oct |
| Se expone información de usuarios o un secreto | R7 | No pedir datos personales, aviso y consentimiento, `.env` fuera del repo | Nelson | Diseño propuesto (D6); `.gitignore` ya excluye `.env` | 19 oct |
| El docente no autoriza a tiempo | R6 | Solicitud escrita el 16 oct; mientras tanto, solo documentación | Alex | Borrador de solicitud; sin respuesta | 20 oct |
| Poca gente quiere pagar | R3 | Nivel gratuito, alianzas con universidades, pregunta de disposición de pago | Cristián y Alex | Pregunta incluida en el protocolo; sin datos | 22 oct |
