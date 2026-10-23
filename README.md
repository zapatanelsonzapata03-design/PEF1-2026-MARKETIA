# PEF1-2026-MarketIA

MarketIA orienta a emprendedores de Cochabamba al planificar un negocio
mediante un informe con cálculos de costos y punto de equilibrio, FODA y una
estimación de demanda, en español y en bolivianos.

**Informe final:** [`docs/01-proyecto/MarketIA_informe_final.pdf`](docs/01-proyecto/MarketIA_informe_final.pdf)

## Problema en 30 segundos
Mucha gente en Cochabamba abre un negocio sin saber si le va a dar ganancia.
Un estudio de viabilidad profesional puede ser caro y demorar días, así que la
persona decide sin un análisis claro. MarketIA ayuda a estimar cuánto necesita
vender para cubrir sus costos y qué riesgos debería revisar.

Las cifras de fracaso e informalidad del informe provienen de Los Tiempos
(2026) y López Castro et al. (2026); están transcritas en
[`referencias.md`](docs/01-proyecto/referencias.md) y **falta verificarlas**.
No se presentan como hechos comprobados hasta entonces.

## Objetivo general
Generar para un negocio en Cochabamba un informe de viabilidad con FODA,
demanda, costos y punto de equilibrio en menos de cinco minutos y a un costo
accesible. Indicadores en [`objetivos.md`](docs/02-requisitos/objetivos.md).

## Usuario y MVP
**Usuario prioritario:** emprendedor o microempresario de Cochabamba que planifica
un negocio de comercio o servicios simples.

**MVP v1.0:** formulario → cálculos fijos (costos y punto de equilibrio) → FODA y
estimación de demanda con IA, etiquetados y con supuestos visibles → informe en
pantalla. La persona ingresa los competidores y precios que conoce.

**No incluye el MVP:** cuentas e inicio de sesión, pagos, aplicación móvil
nativa, cobertura fuera de Cochabamba, búsqueda automática de competencia,
versión para asesores, historial, panel administrativo, otros idiomas y
exportación PDF propia. Los planes de pago del informe son proyección 2027.
Detalle en [`alcance-mvp-y-requisitos.md`](docs/02-requisitos/alcance-mvp-y-requisitos.md).

## Tecnologías candidatas
Python + FastAPI, React, PostgreSQL y un LLM vía OmniRoute (piloto), sujetos a
una prueba de viabilidad. Ver [`arquitectura-inicial.md`](docs/03-arquitectura/arquitectura-inicial.md).

## Equipo
| Integrante | Rol |
|---|---|
| Alex Vásquez Pérez | Coordinador del proyecto |
| Nelson Zapata Jiménez | Líder del motor y la IA |
| Cristián García Bustamante | Líder de la pantalla y la calidad |

Horas, reuniones y flujo de trabajo: [`equipo/roles-y-acuerdos.md`](equipo/roles-y-acuerdos.md).
Tareas en Trello: enlace pendiente de registrar cuando exista evidencia del
tablero en [`docs/07-evidencias/evidencia-organizacion.md`](docs/07-evidencias/evidencia-organizacion.md).
Código y revisiones en GitHub.

## Hitos
| Fecha | Avance |
|---|---|
| Sábado 24 de octubre de 2026 | 40 %: presentación en clase |
| Martes 24 de noviembre de 2026 | 80 %: sistema integrado |
| Sábado 19 de diciembre de 2026 | 100 %: lanzamiento del proyecto finalizado |

## Cómo empezar: lectura recomendada
1. [`docs/01-proyecto/`](docs/01-proyecto/resumen-del-problema.md): problema, evidencia y [referencias](docs/01-proyecto/referencias.md).
2. [`docs/decisiones.md`](docs/decisiones.md): decisiones D1 a D15 y estado de ratificación.
3. [`docs/02-requisitos/`](docs/02-requisitos/alcance-mvp-y-requisitos.md): alcance, MVP, requisitos y [objetivos](docs/02-requisitos/objetivos.md).
4. [`docs/03-arquitectura/`](docs/03-arquitectura/arquitectura-inicial.md): diseño, datos, seguridad y [pruebas](docs/03-arquitectura/datos-seguridad-pruebas.md).
5. [`docs/04-planificacion/`](docs/04-planificacion/plan-desarrollo-y-riesgos.md): Gantt, sprints, horas y riesgos.
6. [`docs/05-estadistica/`](docs/05-estadistica/plan-validacion.md): validación y [resultados](docs/05-estadistica/resultados.md).
7. [`docs/07-evidencias/`](docs/07-evidencias/README.md): entrevistas, cotizaciones y evidencias.
8. [`docs/06-auditoria/`](docs/06-auditoria/cuestionario-aprobacion.md): estado de las 52 preguntas y [prueba de fracaso](docs/06-auditoria/prueba-de-fracaso.md).
9. [`docs/09-preparacion.md`](docs/09-preparacion.md), [`docs/04-planificacion/plan-de-cierre-y-ruta-a-la-aprobacion.md`](docs/04-planificacion/plan-de-cierre-y-ruta-a-la-aprobacion.md) y [`docs/08-presentacion/`](docs/08-presentacion/README.md).

## Qué construir primero
El 15 de octubre el docente respondió “NO APROBADO TODAVÍA”; esa respuesta no
autoriza el desarrollo. No se escribe código en `src/` hasta recibir una nueva
autorización expresa. Después de obtenerla, las primeras tareas propuestas son:
Nelson, esqueleto de la API y motor de cálculos; Cristián, formulario; Alex,
coordinación, informe y evidencias.

## Archivos para asistentes de IA
`.clinerules` y `.github/copilot-instructions.md` son instrucciones para
asistentes de IA que trabajen con el repositorio. Las decisiones ratificadas se
registran en `docs/decisiones.md`; una propuesta no ratificada no es un acuerdo.

## Estado actual
Actualizado el 22 de octubre de 2026. El docente comunicó el 15 de octubre que
el proyecto aún no estaba aprobado; no consta una autorización posterior.
Avance de las acciones que dependen del equipo y de terceros:

- [ ] Acta 01 completada (`docs/actas/acta-01-ratificacion.md`)
- [ ] Nueva autorización docente para el desarrollo y la prueba técnica (`docs/07-evidencias/solicitud-autorizacion-docente.md`)
- [ ] Referencias verificadas (`docs/06-auditoria/verificacion-referencias.md`)
- [ ] Entrevistas aplicadas: __ de 8 (`docs/07-evidencias/registro-entrevistas.md`)
- [ ] Cotizaciones obtenidas: __ de 2
- [ ] 10 casos de fórmulas revisados por una segunda persona
- [ ] Prueba de viabilidad de OmniRoute, solo con autorización (`docs/07-evidencias/registro-prueba-viabilidad.md`)
- [ ] Tablero de Trello y protección de `main` (`docs/07-evidencias/evidencia-organizacion.md`)

Lo que no tiene casilla marcada **no está validado**. El desarrollo en `src/`
empieza solo con una nueva autorización expresa del docente. Las tareas con
fechas anteriores al 22 de octubre deben reprogramarse si siguen pendientes.

## Materia
El informe y el README indican Probabilidad y Estadística · UNIFRANZ · docente
Diego Patrick Cárdenas · paralelo 3. El cuestionario de aprobación está
titulado "Programación II - P2". Se pidió confirmación al docente (decisión
D15); hasta recibir respuesta se mantienen ambos nombres.
