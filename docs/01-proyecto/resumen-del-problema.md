# Resumen del problema y valor

> Síntesis elaborada a partir del README, del informe final y del paquete de mejoras. La
> explicación breve, las consecuencias y la propuesta de valor deben
> contrastarse con evidencia y entrevistas antes de presentarlas como hechos
> demostrados.

## Explicación en 30 segundos, sin tecnología

> Mucha gente en Cochabamba abre un negocio sin saber si le va a dar ganancia.
> Un estudio de viabilidad profesional puede ser caro y demorar días, así que
> la persona puede terminar decidiendo sin un análisis claro. MarketIA propone
> ayudar a estimar cuánto necesita vender para cubrir sus costos y qué riesgos
> debería revisar.

Esta redacción es una propuesta de exposición, no un resultado de investigación.
El README del proyecto aún debe respaldar con fuentes las afirmaciones sobre
costo, duración y frecuencia de decisiones sin análisis.

## Usuarios

El usuario prioritario propuesto es un emprendedor o microempresario de
Cochabamba que está planificando abrir un negocio de comercio o servicios
simples. Asesores e incubadoras y estudiantes quedan como usuarios secundarios
para una versión posterior. El equipo debe ratificar esta prioridad y validarla
con participantes.

## Consecuencias a validar

El paquete de mejoras propone investigar si las personas:

- Invierten ahorros sin conocer su punto de equilibrio.
- Fijan precios sin saber su margen.
- Descubren tarde a la competencia o los costos fijos.
- Abandonan un negocio o lo operan en la informalidad.

Estas consecuencias son hipótesis de trabajo. El repositorio no contiene
entrevistas o encuestas que las confirmen.

## Por qué la solución propuesta responde al problema

La necesidad que el equipo quiere atender es tomar decisiones sobre una idea
de negocio con orientación accesible. El MVP propone combinar:

1. Cálculo determinista del punto de equilibrio, que puede compararse con casos
   de referencia.
2. FODA como resumen estructurado de riesgos y oportunidades.
3. Estimación de demanda con supuestos explícitos, sin presentarla como dato
   verificado.
4. Un informe en pantalla con resultados legibles.

El paquete enumera como alternativas a contrastar un estudio profesional,
plantillas de hoja de cálculo y herramientas extranjeras. No hay una
comparación documentada ni evidencia suficiente para afirmar que estas
alternativas han sido descartadas por los usuarios.

## Evidencia disponible y faltante

El README original atribuye cifras sobre fracaso de emprendimientos e
informalidad a Los Tiempos (2026) y López Castro et al. (2026), y afirma que
los estudios profesionales cuestan cientos de dólares y demoran días. Las
referencias del informe ya están transcritas en `referencias.md` y falta
verificarlas; las cotizaciones y la evidencia local todavía no constan.

Plan de evidencia propuesto:

- Completar y revisar las referencias bibliográficas antes de citar cifras.
- Comparar al menos dos cotizaciones de estudios locales, guardando evidencia
  en `docs/07-evidencias/`.
- Realizar entrevistas o una encuesta a ocho o más emprendedores de
  Cochabamba, con protocolo aprobado y registro agregado/anónimo. Ver
  `docs/07-evidencias/registro-entrevistas.md`.
- Usar las respuestas para evaluar problema, consecuencias, información
  deseada y disposición de pago; informar método y limitaciones en
  `docs/05-estadistica/`.

No se inventan fuentes, precios, tiempos ni respuestas. Hasta recopilar esa
evidencia, no se puede afirmar que el problema o la accesibilidad del precio
estén validados.

## Alternativas que tiene hoy un emprendedor (según el informe final)

| | Estudio profesional | IA del extranjero | MarketIA (propuesta) |
|---|---|---|---|
| Costo | Varios cientos de dólares (sin cotización propia aún) | Suscripción en dólares | Bs 0 a Bs 80 al mes (proyección 2027) |
| Tiempo | Días o semanas | Minutos | Menos de 5 minutos (meta) |
| Idioma y contexto | Local | Inglés y otros países | Español y datos de Bolivia |
| Facilidad para un microemprendedor | Baja | Media-baja | Alta (meta; no probada) |

Esta comparación proviene del informe y **no está respaldada todavía** con
cotizaciones ni capturas de herramientas reales; ver
[`referencias.md`](referencias.md). Quien lea el repositorio debe tomarla como
una hipótesis del equipo, no como resultado.

## Fuentes citadas en el informe
Las referencias del informe están transcritas en
[`referencias.md`](referencias.md), con el estado de verificación de cada una.

## Valor esperado e indicadores

El objetivo general del README plantea un informe de viabilidad en menos de
cinco minutos y a costo accesible. La meta de tiempo se propone medir desde el
envío hasta que el informe aparezca; el precio accesible debe definirse con
datos de encuesta y el costo técnico por informe. Ver `docs/02-requisitos/objetivos.md`
para indicadores propuestos.
