# Accesos, hosting y dependencias externas

**Responsable de completar:** Nelson Zapata Jiménez · **Revisa:** Alex Vásquez Pérez

> Completar solo con lo que se comprobó. **No escribir claves, contraseñas,
> tokens ni el contenido de archivos `.env` en este documento ni en el
> repositorio.** En "Dónde se guarda el secreto" anotar el lugar (por ejemplo,
> variable de entorno del servidor o gestor de contraseñas del equipo), nunca
> el valor.
>
> Esta es una plantilla de control aún sin completar. Los campos en blanco
> significan "no registrado aquí"; no confirman que el recurso exista o falte.
> Ver el estado general en [`09-preparacion.md`](09-preparacion.md).

**Estado permitido:** `Tengo` · `Falta` · `En trámite` · `No aplica`

## 1. Accesos

| Recurso | Para qué se necesita | Quién lo administra | Estado | Fecha de comprobación | Dónde se guarda el secreto | Evidencia (captura sin claves) | Alternativa si falta |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Repositorio GitHub (`zapatanelsonzapata03-design/PEF1-2026-MARKETIA`)

 | Almacenar código, control de versiones, Pull Requests y rama `main` protegida

 | Nelson Zapata

 | **OK (Activo)**<br> | 22/10/2026

 | No aplica | `docs/07-evidencias/main-protegida-regla.png`<br> | Transferir propiedad a Alex o Cristian |
| Permisos de Alex y Cristian en el repositorio | Revisar y aprobar Pull Requests con revisión cruzada obligatoria

 | Nelson Zapata

 | **OK (Confirmado)**<br> | 22/10/2026

 | No aplica | `docs/07-evidencias/evidencia-organizacion.md` (PR #1 Aprobado)

 | Aprobar cambios via revisión sincrónica |
| Tablero de Trello | Gestión de 21 tarjetas con tareas, responsables y fechas

 | Alex Vásquez

 | **OK (Activo)**<br> | 22/10/2026

 | No aplica | `docs/07-evidencias/tablero-trello-marketia.md`<br> | Tablero GitHub Projects integrado |
| OmniRoute (instalación o servicio) | Enrutar consultas al LLM de forma unificada

 | Nelson Zapata

 | **PENDIENTE (A la espera de autorización docente)**<br> | 22/10/2026

 | `.env.local`<br> | `docs/07-evidencias/registro-prueba-viabilidad.md`<br> | Integración directa con proveedores LLM |
| Proveedor de LLM 1 (nombre: **OpenAI GPT-4o-mini**)

 | Generación de análisis FODA y estimación cualitativa de demanda

 | Nelson Zapata

 | **OK (Verificado)**<br> | 22/10/2026

 | `.env.local` (`OPENAI_API_KEY`)

 | `docs/07-evidencias/registro-prueba-viabilidad.md`<br> | Cambiar a Gemini 1.5 Flash |
| Proveedor de LLM 2, plan B (nombre: **Google Gemini 1.5 Flash**)

 | Respaldo si falla el proveedor principal o por exceso de latencia ($> 60\text{ s}$)

 | Nelson Zapata

 | **OK (Verificado)**<br> | 22/10/2026

 | `.env.local` (`GEMINI_API_KEY`)

 | `docs/07-evidencias/registro-prueba-viabilidad.md`<br> | Anthropic Claude 3.5 Haiku |
| Hosting del frontend (nombre: **Vercel**) | Publicar la interfaz de usuario en React/Next.js para la demostración

 | Cristian García | **OK (Configurado)** | 22/10/2026 | Variables de entorno en panel Vercel | Enlace público en el `README.md` | Netlify / Render Frontend |
| Hosting del backend (nombre: **Render**) | Ejecutar la API REST desarrollada en Python / FastAPI

 | Nelson Zapata

 | **OK (Configurado)** | 22/10/2026 | Variables de entorno en panel Render (`.env`)

 | Logs de despliegue en Render | Railway / Fly.io |
| Base de datos (PostgreSQL o SQLite) | Persistencia (Solo si se ratifica D6; en MVP recortado es procesamiento en memoria/pantalla)

 | Nelson Zapata

 | **NO APLICA (Recortado)**<br> | 22/10/2026

 | `.env.local`<br> | `docs/actas/acta-01-ratificacion.md` (Decisión D6)

 | Reporte renderizado únicamente en pantalla

 |
| Dominio o URL de la demostración | Acceso del docente y usuarios de prueba a la demostración web | Alex Vásquez

 | **OK (Generado)** | 22/10/2026 | No aplica | Enlace de previsualización en `README.md` | Localhost mediante Ngrok para la defensa |
| Google Drive y WhatsApp | Coordinación interna, almacenamiento de actas, referencias y avisos

 | Alex Vásquez

 | **OK (Activo)**<br> | 22/10/2026

 | No aplica | Repositorio GitHub carpeta `docs/`<br> | Mensajería institucional Unifranz |

---


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
| LLM (costo por informe, medido en la prueba) | | | | |
| Dominio | | | | |

## 4. Entorno de ejecución

| Dato | Valor |
|---|---|
| Versión de Python | |
| Versión de Node | |
| Sistema operativo del equipo | |
| Pasos para ejecutar el proyecto (resumen) | |
| ¿Otro integrante pudo ejecutarlo siguiendo estos pasos? | |

## 5. Pendientes

| Falta | Responsable | Fecha límite | Resuelto |
|---|---|---|---|
| | | | |
