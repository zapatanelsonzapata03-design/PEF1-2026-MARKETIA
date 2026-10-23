# Accesos, hosting y dependencias externas

**Responsable de completar:** Nelson Zapata Jiménez · **Revisa:** Alex Vásquez Pérez

> Completar solo con lo que se comprobó. **No escribir claves, contraseñas,
> tokens ni el contenido de archivos `.env` en este documento ni en el
> repositorio.** En "Dónde se guarda el secreto" anotar el lugar (por ejemplo,
> variable de entorno del servidor o gestor de contraseñas del equipo), nunca
> el valor.
>
Los campos en blanco significan "no registrado aquí"; no confirman que el
recurso exista o falte. Ver el estado general en
[`09-preparacion.md`](09-preparacion.md).

**Estado permitido:** `Tengo` · `Falta` · `En trámite` · `No aplica`

## 1. Accesos

| Recurso | Para qué se necesita | Quién lo administra | Estado | Fecha de comprobación | Dónde se guarda el secreto | Evidencia (captura sin claves) | Alternativa si falta |
|---|---|---|---|---|---|---|---|
| Repositorio GitHub (`zapatanelsonzapata03-design`) | Código, pull requests, `main` protegida | | | | No aplica | | |
| Permisos de Alex y Cristián en el repositorio | Revisar y aprobar pull requests | | | | No aplica | | |
| Tablero de Trello | Tareas, responsables y fechas | | | | No aplica | | |
| OmniRoute (instalación o servicio) | Enrutar consultas al LLM | No registrado; configuración reportada por el equipo | Tengo (configuración reportada; prueba preliminar de un caso) | 08/10/2026 (capturas del informe y evidencia añadida) | No registrado aquí | [`Evidencia de prueba y topología`](07-evidencias/README.md#prueba-preliminar-de-omniroute) y Anexo B del informe final | Otro proveedor compatible |
| Principal del piloto: Gemini Flash vía OmniRoute (modelo exacto por confirmar) | FODA y demanda | Nelson Zapata Jiménez (motor e IA; acceso individual por comprobar) | Tengo (disponibilidad en OmniRoute reportada por el equipo; prueba identificada con este modelo pendiente) | Reportado por el equipo el 23/10/2026 | No registrado aquí | La evidencia preliminar de OmniRoute está en [`07-evidencias/README.md`](07-evidencias/README.md#prueba-preliminar-de-omniroute), pero no identifica el modelo usado | Claude Haiku como respaldo, sujeto a disponibilidad y prueba |
| Respaldo de pago: Claude Haiku 5.5 (`claude-haiku-5-5`, nombre/ID reportado por el equipo) | Respaldo si Gemini Flash no está disponible o alcanza sus límites | Nelson Zapata Jiménez (acceso individual por comprobar) | En trámite (propuesto por el equipo; disponibilidad del nombre/ID, cuenta y prueba no comprobadas) | Reportado por el equipo el 23/10/2026 | No registrado aquí | No hay evidencia de acceso o prueba en el repositorio | Modelo compatible alternativo de Groq o Mistral, sujeto a selección y prueba |
| Alternativa rápida: modelo abierto pequeño de Groq o Mistral (sin modelo seleccionado) | Alternativa si falla el principal o el respaldo | Nelson Zapata Jiménez (por confirmar) | En trámite (proveedor, modelo, acceso y calidad en español pendientes de prueba) | Reportado por el equipo el 23/10/2026 | No registrado aquí | No hay evidencia de selección o prueba en el repositorio | Revisar Gemini Flash y el respaldo antes de cambiar el piloto |
| Hosting del frontend | Publicar la demostración | | Falta (no consta proveedor ni cuenta elegidos) | | | | |
| Hosting del backend | Ejecutar la API | | Falta (no consta proveedor ni cuenta elegidos) | | | | |
| Base de datos (PostgreSQL o SQLite) | Persistencia, solo si se ratifica D6 | | | | | | Informe solo en pantalla |
| Dominio o URL de la demostración | Acceso del docente y usuarios de prueba | | | | No aplica | | |
| Google Drive y WhatsApp | Documentos, actas y avisos | | | | No aplica | | |

## 2. Permisos y autorizaciones

| Permiso | Quién lo da | Estado | Fecha | Evidencia |
|---|---|---|---|---|
| Autorización para la prueba de viabilidad de la IA | Docente | | | |
| Autorización para iniciar el desarrollo en `src/` | Docente | | | |
| Autorización para aplicar entrevistas | Docente | | | |
| Términos y privacidad del proveedor de IA revisados | Nelson | | | |
| Consentimiento informado aprobado | Docente y equipo | | | |

## 3. Costos previstos

| Concepto | Plan gratuito o de pago | Costo mensual (Bs) | Límite del plan gratuito | Fuente y fecha |
|---|---|---:|---|---|
| Hosting | Pendiente: no se eligió proveedor | | | No hay proveedor, cuenta ni comparación documentados en el repositorio |
| Base de datos | Pendiente: D6 no ratificada | | | `docs/decisiones.md` y arquitectura inicial |
| Gemini Flash vía OmniRoute (principal propuesto) | Plan gratuito reportado por el equipo | Bs 0 reportado; no es una medición de cargos ni un costo por informe verificado | No registrado en el repositorio | Selección comunicada por el equipo el 23/10/2026; falta registrar modelo exacto, cuota y evidencia de uso |
| Claude Haiku 5.5 (`claude-haiku-5-5`, respaldo propuesto) | API de pago reportada por el equipo | No registrado | No aplica | Selección comunicada por el equipo el 23/10/2026; falta confirmar el nombre/ID y registrar la tarifa aplicable |
| Alternativa Groq o Mistral (sin modelo seleccionado) | Plan y costo no registrados | No registrado | No registrado | Alternativa comunicada por el equipo el 23/10/2026; requiere seleccionar y comprobar un modelo |
| LLM (costo de la prueba preliminar de un caso del 08/10/2026) | Plan gratuito reportado | Bs 0 reportado por el equipo; las capturas no muestran una medición de cargos o tokens | No registrado aquí | Capturas del 08/10/2026 en [`docs/07-evidencias/`](07-evidencias/README.md#prueba-preliminar-de-omniroute); costo comunicado por el equipo |
| Dominio | | | | |

## 4. Entorno de ejecución

`src/` no contiene una aplicación ejecutable; no hay pasos de ejecución
disponibles ni una prueba P50 que pueda marcarse como superada. El Anexo B del
informe y las capturas enlazadas documentan únicamente una interacción
preliminar de un caso con OmniRoute; no equivalen a una prueba completa del
sistema ni a una medición del costo por informe.

| Dato | Valor |
|---|---|
| Versión de Python |la ultima versión |
| Versión de Node |la ultima versión |
| Sistema operativo del equipo | windows |
| Pasos para ejecutar la aplicación | No disponibles: desarrollo pendiente de autorización docente |
| ¿Otro integrante pudo ejecutar la aplicación? | No registrado; todavía no hay aplicación en `src/` |

## 5. Pendientes

| Falta | Responsable | Fecha límite | Resuelto |
|---|---|---|---|
| | | | |
