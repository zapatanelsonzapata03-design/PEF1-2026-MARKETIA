# PEF1-2026-MarketIA

MarketIA propone orientar a emprendedores de Cochabamba al planificar un
negocio, mediante un informe con cálculos de costos y punto de equilibrio,
FODA y una estimación de demanda.

## Problema planteado

El proyecto plantea que los emprendedores pueden carecer de orientación
accesible y oportuna para evaluar su idea. El README anterior incluía cifras
de fracaso e informalidad y afirmaciones de costos sin referencias completas
en el repositorio. No se presentan como hechos verificados hasta completar
`docs/01-proyecto/referencias.md` y reunir evidencia local.

## Objetivo general

Generar para un negocio en Cochabamba un informe de viabilidad con FODA,
demanda, costos y punto de equilibrio en menos de cinco minutos y a un costo
accesible para un microemprendedor. Los indicadores para comprobarlo están en
[`docs/02-requisitos/objetivos.md`](docs/02-requisitos/objetivos.md); son
propuestas pendientes de ratificación y medición.

## Usuario prioritario y MVP propuestos

**Usuario:** emprendedor o microempresario de Cochabamba que está planificando
un negocio de comercio o servicios simples. Debe ratificarse y validarse con
usuarios.

**MVP v1.0 propuesto:** formulario → cálculos fijos → FODA y estimación de
demanda con IA, etiquetados y con supuestos visibles → informe en pantalla.
En el MVP, la persona ingresaría los competidores y precios que conoce; no se
haría búsqueda automática. La exportación PDF propia y la investigación
automática de mercado se postergan. Revisar y ratificar el alcance en
[`docs/02-requisitos/alcance-mvp-y-requisitos.md`](docs/02-requisitos/alcance-mvp-y-requisitos.md)
y las decisiones en [`docs/decisiones.md`](docs/decisiones.md).

## Qué no incluye el MVP propuesto

Cuentas e inicio de sesión, pagos, aplicación móvil nativa, cobertura fuera de
Cochabamba, búsqueda automática de competencia/precios, versión para asesores,
historial, panel administrativo, idiomas distintos del español ni exportación
PDF propia. Son propuestas del paquete de mejoras y requieren ratificación del
equipo.

## Tecnologías y equipo

Tecnologías candidatas del README original: Python + FastAPI, React,
PostgreSQL y un LLM vía OmniRoute como piloto. Su uso depende de las decisiones
y pruebas de viabilidad documentadas en
[`docs/03-arquitectura/arquitectura-inicial.md`](docs/03-arquitectura/arquitectura-inicial.md).

| Integrante | Rol |
|---|---|
| Alex Vásquez Pérez | Coordinador del proyecto |
| Nelson Zapata Jiménez | Líder del motor y la IA |
| Cristián García Bustamante | Líder de la pantalla y la calidad |

## Cómo empezar: lectura recomendada

1. [`docs/01-proyecto/resumen-del-problema.md`](docs/01-proyecto/resumen-del-problema.md):
   problema y evidencia por reunir.
2. [`docs/decisiones.md`](docs/decisiones.md): propuestas de decisión y estado
   de ratificación.
3. [`docs/02-requisitos/alcance-mvp-y-requisitos.md`](docs/02-requisitos/alcance-mvp-y-requisitos.md)
   y [`docs/02-requisitos/objetivos.md`](docs/02-requisitos/objetivos.md):
   funcionalidades, criterios y metas.
4. [`docs/03-arquitectura/arquitectura-inicial.md`](docs/03-arquitectura/arquitectura-inicial.md)
   y [`docs/03-arquitectura/datos-seguridad-pruebas.md`](docs/03-arquitectura/datos-seguridad-pruebas.md):
   diseño, datos, seguridad y pruebas propuestas.
5. [`docs/04-planificacion/plan-desarrollo-y-riesgos.md`](docs/04-planificacion/plan-desarrollo-y-riesgos.md)
   y [`docs/09-preparacion.md`](docs/09-preparacion.md): tareas, riesgos y
   requisitos previos.
6. [`docs/06-auditoria/cuestionario-aprobacion.md`](docs/06-auditoria/cuestionario-aprobacion.md):
   estado documental de las 52 preguntas.
7. [`docs/01-proyecto/referencias.md`](docs/01-proyecto/referencias.md),
   [`docs/05-estadistica/plan-validacion.md`](docs/05-estadistica/plan-validacion.md)
   y [`docs/07-evidencias/README.md`](docs/07-evidencias/README.md): fuentes,
   validación y evidencias por reunir.
8. [`docs/06-auditoria/prueba-de-fracaso.md`](docs/06-auditoria/prueba-de-fracaso.md)
   y [`docs/08-presentacion/README.md`](docs/08-presentacion/README.md):
   riesgos de fracaso y preparación de la exposición.

`.clinerules` y `.github/copilot-instructions.md` son instrucciones para
asistentes de IA que trabajen con el repositorio; indican cómo respetar las
restricciones del proyecto. Las decisiones ratificadas deben registrarse en
`docs/decisiones.md`; una propuesta no ratificada no es un acuerdo.

## Estado y próximos pasos

El README original registra como hito la presentación del 24 de octubre de
2026. El Gantt de la fase A del
[plan de desarrollo](docs/04-planificacion/plan-desarrollo-y-riesgos.md)
propone fechas entre el 15 y el 24 de octubre; el equipo debe confirmarlas,
actualizarlas si ya no son viables y asignar disponibilidad real. No hay
autorización docente, resultados de entrevistas, cotizaciones ni pruebas
técnicas registrados en el repositorio.

Antes de desarrollar: ratificar las decisiones, validar referencias y
necesidades, completar los datos reales pendientes en
[`docs/09-preparacion.md`](docs/09-preparacion.md), y solicitar autorización
docente. **`src/` debe permanecer sin código hasta que el docente autorice el
desarrollo.**

## Materia

El README original registra Probabilidad y Estadística · UNIFRANZ · docente
Diego Patrick Cárdenas · paralelo 3. El cuestionario adjunto está titulado
“Programación II - P2”. Esta diferencia requiere confirmación del docente; no
se unifica hasta que exista una respuesta registrada.
