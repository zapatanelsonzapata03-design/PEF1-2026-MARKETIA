# Acta 01: ratificación de decisiones y acuerdos de trabajo

> Completar durante o después de la reunión. **No marcar acuerdos que no
> ocurrieron.** Marcar con una X una sola casilla por decisión.

- **Fecha y hora reportadas:** 22 de octubre de 2026, 23:00 (la captura adjunta no acredita que la reunión se realizara)
- **Medio reportado:** videollamada (pendiente de confirmar)
- **Asistentes registrados:** Alex Vásquez Pérez · Nelson Zapata Jiménez · Cristián García Bustamante (la captura adjunta no acredita asistencia)
- **Modera:** Alex Vásquez Pérez · **Toma el acta:** (por completar)

## 1. Decisiones (detalle completo en `docs/decisiones.md`)

| ID | Propuesta en una línea | Aprobada | Modificada | Rechazada | Cambios acordados |
|---|---|:-:|:-:|:-:|---|
| D1 | Usuario prioritario: emprendedor o microempresario de Cochabamba con un negocio simple de comercio o servicios |si | | | |
| D2 | MVP: formulario → cálculos fijos → FODA y demanda con IA etiquetados → informe en pantalla |si | | | |
| D3 | El usuario ingresa los competidores que conoce; búsqueda automática en v2 (corregir Meta 1) |si | | | |
| D4 | PDF: impresión del navegador en el MVP; PDF propio en v1.1 |si | | | |
| D5 | Exclusiones: cuentas, pagos, app móvil, otras ciudades, panel admin, historial, asesores, otros idiomas |si | | | |
| D6 | PostgreSQL solo con entrada e informe, id aleatorio, retención 90 días, aviso antes de enviar a la IA |si | | | |
| D7 | LLM: OmniRoute como principal para el piloto, sujeto a prueba de viabilidad; plan B otro proveedor |si | | | |
| D8 | Idioma español y moneda bolivianos |si | | | |
| D9 | Git: ramas por tarea, pull request con aprobación de otra persona, `main` protegida |si | | | |
| D10 | Solicitar por escrito al docente: prueba técnica, inicio del desarrollo y protocolo de entrevistas |si | | | |
| D11 | Roles: Nelson (motor e IA), Cristián (pantalla y calidad), Alex (coordinación, informe, costos); corregir el informe |si | | | |
| D12 | Meta 1: reducir 70 % el tiempo frente a hacerlo a mano, con línea base en 3 casos |si | | | |
| D13 | Muestras: 8 a 10 entrevistas, 5 de usabilidad, 30 en la prueba piloto (ideal 43) |si | | | |
| D14 | Herramientas: Trello, GitHub, Drive y WhatsApp |si | | | |
| D15 | Confirmar con el docente la materia (Probabilidad y Estadística o Programación II - P2) | | | | a espera de la confirmacion|
| D16 | Contrato API único del MVP: `POST /analisis` y `GET /health`; endpoints separados quedan para v1.1 | | | | |

## 2. Acuerdos de trabajo (ver `equipo/roles-y-acuerdos.md`)

| Punto | Propuesta | Resultado acordado |
|---|---|---|
| Horas por persona, fase A (hasta el 24 oct) | 21 horas | |
| Disponibilidad por persona, fase B | 3 horas por día | |
| Reuniones | lunes, miércoles y viernes, 20:00 a 20:45, videollamada | |
| Planificación y cierre de sprint | lunes (inicio) y viernes de la 2.ª semana (cierre), 60 min | |
| Disponibilidad real de Alex |3 horas por día |reportado |
| Disponibilidad real de Nelson |3 horas por día |reportado |
| Disponibilidad real de Cristián |3 horas por día |reportado |

Si alguien no puede cumplir las horas, se aplica el recorte del 40 % del
documento de requisitos. ¿Se aprueba esa regla? ( ) Sí ( ) No

## 3. Compromisos

| Tarea | Responsable | Fecha límite | Hecho |
|---|---|---|:-:|
| Enviar solicitud formal al docente y registrar su respuesta | Alex | Por acordar | No (el envío del enlace del repositorio el 15/10 no acredita una solicitud formal ni respuesta) |
| Aplicar entrevistas | Cristián y Alex | Por acordar | Parcial (8 resúmenes; faltan fichas completas y evidencia de consentimiento) |
| Pedir 2 cotizaciones | Alex | Por acordar | Parcial (2 consultas enviadas el 22/10; sin respuestas; la referencia pública de TikTok no es una cotización) |
| Verificar referencias | Alex | Por acordar | Parcial (Nelson registró la revisión; falta revisión por otra persona y corregir/delimitar el informe) |
| Revisar los 10 casos de fórmulas | Cristián | Por acordar | No (no consta revisión independiente firmada) |
| Prueba ampliada de viabilidad de OmniRoute (10 ideas, con autorización) | Nelson | Tras la autorización | Parcial (hay evidencia preliminar de un caso del 08/10; la prueba ampliada requiere autorización) |
| Verificar protección de `main` | Nelson | Por acordar | Parcial (la captura no muestra el patrón de rama ni confirma que la regla esté activa para `main`) |
| Crear tablero de Trello y compartir enlace | Alex | 22/10/26 | Sí |

## 4. Evidencia de la reunión
Captura del chat de WhatsApp del 22/10/2026:
[evidencia-coordinacion-reunion.png](evidencia-coordinacion-reunion.png).
Muestra la coordinación para realizar la reunión y mensajes de disponibilidad
de integrantes. Por sí sola no confirma que la reunión se haya realizado ni
acredita la asistencia completa o los acuerdos tratados.

## 5. Confirmación de los asistentes
- Alex Vásquez Pérez: (si ) confirmado el 22/10/26
- Nelson Zapata Jiménez: (si ) confirmado el 22/10/26
- Cristián García Bustamante: (si ) confirmado el 22/10/26

## 6. Para copiar al registro de `docs/decisiones.md`

| Fecha | IDs ratificados | Quiénes participaron | Evidencia |
|---|---|---|---|
| 22/10/2026 | (ej.: D1 a D9, D11 a D14) | Alex Vásquez Pérez, Nelson Zapata Jiménez y Cristián García Bustamante| `docs/actas/acta-01-ratificacion.md` y captura en `docs/07-evidencias/` |

Cada integrante confirma por escrito (por ejemplo, un mensaje en el grupo,
guardado como captura) que el acta refleja lo acordado.

> Nota de revisión (23/10/2026): los estados de los compromisos se ajustaron a
> la evidencia registrada en el repositorio. La captura adjunta muestra
> coordinación y disponibilidad para reunirse; no demuestra que la reunión se
> realizara ni acredita por sí sola su fecha, asistencia o acuerdos. Completar
> esos datos con evidencia real si corresponde.
