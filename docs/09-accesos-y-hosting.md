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
| Proveedor de LLM 1 (nombre: ________) | FODA y demanda | | | | | | |
| Proveedor de LLM 2, plan B (nombre: ________) | Respaldo si falla el principal | | | | | | |
| Hosting del frontend (nombre: ________) | Publicar la demostración | | | | | | |
| Hosting del backend (nombre: ________) | Ejecutar la API | | | | | | |
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
| Hosting | | | | |
| Base de datos | | | | |
| LLM (costo de la prueba preliminar de un caso) | Plan gratuito reportado | Bs 0 (dato reportado por el equipo; no se ve una medición de cargos o tokens en las capturas) | No registrado aquí | Capturas del 08/10/2026 en [`docs/07-evidencias/`](07-evidencias/README.md#prueba-preliminar-de-omniroute); costo comunicado por el equipo |
| Dominio | | | | |

## 4. Entorno de ejecución

`src/` no contiene una aplicación ejecutable; no hay pasos de ejecución
disponibles ni una prueba P50 que pueda marcarse como superada. El Anexo B del
informe y las capturas enlazadas documentan únicamente una interacción
preliminar de un caso con OmniRoute; no equivalen a una prueba completa del
sistema ni a una medición del costo por informe.

| Dato | Valor |
|---|---|
| Versión de Python | |
| Versión de Node | |
| Sistema operativo del equipo | |
| Pasos para ejecutar la aplicación | No disponibles: desarrollo pendiente de autorización docente |
| ¿Otro integrante pudo ejecutar la aplicación? | No registrado; todavía no hay aplicación en `src/` |

## 5. Pendientes

| Falta | Responsable | Fecha límite | Resuelto |
|---|---|---|---|
| | | | |
