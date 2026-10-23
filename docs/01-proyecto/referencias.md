# Referencias y evidencia del problema

Las referencias de esta página provienen del **informe final**
([`MarketIA_informe_final.pdf`](MarketIA_informe_final.pdf), sección
"Referencias" y Anexo A). Figuran con los datos que trae el informe. **Estado al
22/10/2026:** Nelson comprobó que los nueve enlaces abren y contrastó las
afirmaciones del informe (ver
[`verificacion-referencias.md`](../06-auditoria/verificacion-referencias.md)).
Hay afirmaciones marcadas para corregir o delimitar y falta revisión por otra
persona; hasta entonces no se presentan como respaldo comprobado.

## 1. Lista de referencias

| N.º | Referencia | Dónde se usa en el informe | Verificada (fecha y quién) |
|---:|---|---|---|
| 1 | Delve AI. (2026). *Las 12 mejores herramientas de investigación de mercado con IA para probar en 2026.* https://www.delve.ai/es/blog/herramientas-investigacion-mercado-ia | Secciones 3 y 5 | verificado por nelson el 22/10/26 |
| 2 | eesel AI. (2026). *Precios de la API de Gemini 2026: tarifa completa y costes ocultos.* https://www.eesel.ai/es/blog/precios-api-gemini | Secciones 5, 6 y 7 | verificado por nelson el 22/10/26 |
| 3 | Google. (2026). *Precios de la API de Gemini.* Google AI for Developers. https://ai.google.dev/pricing | Secciones 5, 6 y 7 | verificado por nelson el 22/10/26 |
| 4 | Kimi AI. (2026). *10 herramientas de IA para estudios de mercado y conclusiones más inteligentes.* https://www.kimi.com/es-419/resources/best-ai-for-market-research | Secciones 3 y 5 | verificado por nelson el 22/10/26 |
| 5 | López Castro, V. I., Apiquian Guitart, A. I., y Mata Mata, L. (2026). *Éxito y fracaso de los emprendimientos en Bolivia: Educación financiera postpandemia.* Revista Perspectivas. https://perspectivas.ucb.edu.bo/index.php/a/article/view/305 | Sección 3 | verificado por nelson el 22/10/26 |
| 6 | Los Tiempos. (2026, 10 de agosto). *Estudio: el 70 por ciento de los emprendimientos fracasan en Bolivia.* https://www.lostiempos.com/actualidad/economia/20260810/estudio-70-ciento-emprendimientos-fracasan-bolivia | Sección 3 | verificado por nelson el 22/10/26 |
| 7 | OmniRoute. (2026). *OmniRoute: the free AI gateway* [Software]. GitHub. https://github.com/diegosouzapw/OmniRoute | Sección 5 | verificado por nelson el 22/10/26 |
| 8 | Shopify. (2026). *Cómo usar la IA en investigación de mercados.* https://www.shopify.com/es/blog/ia-investigacion-de-mercados | Secciones 3 y 5 | verificado por nelson el 22/10/26 |
| 9 | Thunderbit. (2025). *Top 15 mejores herramientas de IA para investigación de mercados en 2026.* https://thunderbit.com/es/blog/best-ai-for-market-research | Secciones 3 y 5 | verificado por nelson el 22/10/26 |

Fecha de consulta de las nueve referencias: 22/10/2026 (Nelson). Los enlaces
abren; la sospecha previa sobre guiones faltantes (Los Tiempos y Shopify) queda
descartada según ese registro.

## 2. Afirmaciones del informe y su respaldo

| Afirmación | Fuente indicada | Estado | Acción |
|---|---|---|---|
| Alrededor de 7 de cada 10 emprendimientos fracasan en Bolivia. | Los Tiempos (2026) | Verificada por Nelson (22/10/2026): la nota habla de 70 % / unos siete de cada diez | Mantener. |
| Cerca del 78,5 % de la actividad económica es informal. | Los Tiempos (2026) | Verificada por Nelson (22/10/2026): cifra atribuida al CEES en la nota | Mantener; citar al CEES como origen. |
| Alrededor del 70 % de las microempresas son informales, lo que dificulta créditos y asesoría. | López Castro et al. (2026) | **No coincide** (verificación 22/10/2026): el artículo no da ese dato para microempresas | **Quitar la afirmación o reformularla** con la cifra real de la fuente; no atribuirla a López Castro et al. Corregir también el informe PDF. |
| Un estudio profesional cuesta varios cientos de dólares y demora días o semanas. | Ninguna | **Sin cotizaciones recibidas**; los importes de entrevistas son declaraciones no verificadas | Obtener 2 cotizaciones reales con [`guion-cotizaciones.md`](../07-evidencias/guion-cotizaciones.md); si no se obtienen, quitar la generalización o identificar claramente la declaración reportada. |
| Las herramientas de IA extranjeras están en inglés y se pagan en dólares. | Kimi AI, Delve AI, Thunderbit, Shopify | Fuentes comerciales; no se documentó revisión de idiomas y precios de servicios concretos | Verificar 2 o 3 herramientas concretas (captura de idioma y precio) o quitar la generalización. |
| Las IAs cobran por cantidad de texto procesado. | Google (2026); eesel AI (2026) | Sin verificar | Citar la página de precios de Google (fuente primaria) y dejar eesel solo como apoyo. |
| OmniRoute es gratuito, de código abierto y reparte las consultas entre varios proveedores. | OmniRoute (2026) | Sin verificar | Revisar el repositorio (licencia, funcionamiento) y los términos de cada proveedor gratuito. |
| Tipo de cambio de Bs 12 por dólar, "valor actual que maneja el equipo". | Ninguna | Sin fuente ni fecha que respalde Bs 12 o la comparación con el valor oficial | **Corregir o quitar**; no presentar valores como hechos hasta documentar fuente y fecha. |

## 3. Calidad de las fuentes

- Las referencias 1, 2, 4, 8 y 9 son blogs o páginas comerciales. Sirven como
  apoyo, pero no deben ser la evidencia principal del problema.
- La evidencia principal del problema son las referencias 5 y 6, más la
  evidencia local propia (entrevistas y cotizaciones).
- Para precios de IA, usar la fuente primaria (referencia 3).

## 4. Evidencia local propia

- Entrevistas a emprendedores de Cochabamba:
  [`protocolo-entrevistas.md`](../07-evidencias/protocolo-entrevistas.md) y
  [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md).
- Cotizaciones de estudios de viabilidad:
  [`guion-cotizaciones.md`](../07-evidencias/guion-cotizaciones.md).
- Hay ocho resúmenes de entrevistas reportados (sin fichas completas ni
  consentimiento verificable) y dos solicitudes de cotización sin respuesta.
  No se presentan como validación formal; ver
  [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md).
