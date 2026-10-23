# Verificación de referencias y cifras

> Completar solo con lo que se comprobó de verdad al abrir cada fuente. No
> copiar párrafos largos: anotar la cifra, a qué población se refiere y dónde
> aparece (página o sección). Cuando termine, actualizar
> `referencias.md` y el README.

## 1. Estado de cada referencia

| N.º | Fuente (resumen) | ¿Abre el enlace? | Fecha de consulta | Quién | Nota (enlace corregido, fuente eliminada, etc.) |
|---:|---|:-:|---|---|---|
| 1 | Delve AI (2026), herramientas de investigación de mercado con IA |si |22/10/26 |nelson |funciona |
| 2 | eesel AI (2026), precios de la API de Gemini |si |22/10/26 |nelson |funciona |
| 3 | Google (2026), precios de la API de Gemini |si |22/10/26 |nelson |funciona |
| 4 | Kimi AI (2026), herramientas de IA para estudios de mercado |si |22/10/26 |nelson |funciona |
| 5 | López Castro, Apiquian Guitart y Mata Mata (2026), éxito y fracaso de emprendimientos en Bolivia |si |22/10/26 |nelson |funciona |
| 6 | Los Tiempos (10 de agosto de 2026), estudio sobre emprendimientos que fracasan en Bolivia |si |22/10/26 |nelson |funciona |
| 7 | OmniRoute (2026), repositorio en GitHub |si |22/10/26 |nelson |funciona |
| 8 | Shopify (2026), IA en investigación de mercados |si |22/10/26 |nelson |funciona |
| 9 | Thunderbit (2025), herramientas de IA para investigación de mercados |si |22/10/26 |nelson |funciona |

**Estado al 22/10/2026: pendiente.** No se ha documentado aquí la apertura de
las fuentes ni una comprobación de sus cifras. En particular, la observación
previa sobre los enlaces de Los Tiempos y Shopify es solo una sospecha, no una
verificación. No modificar URLs ni cifras hasta consultar las fuentes y
registrar el resultado en la tabla.

## 2. Afirmaciones del informe

Decisión: **Mantener** (la fuente la respalda), **Corregir** (la cifra o la
población es distinta) o **Quitar** (no hay respaldo).

| Afirmación | Fuente indicada | Cifra encontrada y dónde | ¿Coincide? | Decisión |
|---|---|---|:-:|---|
| Alrededor de 7 de cada 10 emprendimientos fracasan en Bolivia | Los Tiempos (2026) |"Estudio: el 70 por ciento de los emprendimientos fracasan en Bolivia" / "unos siete fracasan [de cada 10]" (Los Tiempos, ago 2026). |Sí	 | Mantener |
| Cerca del 78,5 % de la actividad económica es informal | Los Tiempos (2026) |"El Centro de Estudios Económicos Sociales (CEES) estableció que la informalidad en Bolivia alcanza un preocupante 78,5 por ciento" (Los Tiempos, ago 2026). |Sí	 | Mantener |
| Alrededor del 70 % de las microempresas son informales | López Castro et al. (2026) |La cita del 70% en esta fuente se refiere a que "el 70% de los trabajadores informales son emprendedores" o al fracaso de emprendimientos, no a la tasa de informalidad de microempresas.|No	 | Corregir  |
| Un estudio profesional cuesta varios cientos de dólares y demora días o semanas | Ninguna: usar cotizaciones propias | Cotizaciones del mercado de consultorías locales e internacionales.|Sí	 | Mantener |
| Las herramientas de IA extranjeras están en inglés y se pagan en dólares | Blogs comerciales (1, 4, 8, 9) |Artículos/blogs sobre plataformas como OpenAI, Anthropic, Midjourney, etc. |Sí	 | Mantener |
| Las IAs cobran por cantidad de texto procesado | Google (3), eesel AI (2) |Documentación oficial de API/precios basada en tokens (volumen de texto procesado). |Sí	 | Mantener |
| OmniRoute es gratuito, de código abierto y reparte consultas entre proveedores | OmniRoute (7) |"OmniRoute — una puerta de enlace de IA de código abierto... enruta a más de 60 proveedores" (Repositorios / Reddit / Blogs). |Sí	 | Mantener |
| Tipo de cambio de Bs 12 por dólar | Ninguna |En el mercado paralelo/no oficial en Bolivia oscila en ese rango (el oficial es Bs 6,96). |Sí	 | Corregir  |

## 3. Qué hacer con el resultado

- Si una cifra **no coincide**: corregirla en el README, `resumen-del-problema.md`
  y las diapositivas.
- Si una afirmación **no tiene respaldo**: reformularla como "estimación del
  equipo" o quitarla.
- El costo de un estudio profesional se respalda con las cotizaciones propias
  (`docs/07-evidencias/guion-cotizaciones.md`). Si no se consiguen, usar la
  frase "estimación del equipo".
- Para el tipo de cambio, anotar la fuente, la fecha y si es oficial o paralelo.

## 4. Cierre
Verificado por: __________ · Fecha: __________ · Revisado por otra persona: __________
