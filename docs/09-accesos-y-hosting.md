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
|---|---|---|---|---|---|---|---|
| Repositorio GitHub (`zapatanelsonzapata03-design/PEF1-2026-MARKETIA`) | Código, pull requests, `main` protegida | Nelson Zapata | **OK (Activo)** | 22/10/2026 | No aplica | `docs/07-evidencias/main-protegida-regla.png` | Transferir propiedad a Alex o Cristian |
| Permisos de Alex y Cristián en el repositorio | Revisar y aprobar pull requests | Nelson Zapata | **OK (Confirmado)** | 22/10/2026 | No aplica | `docs/07-evidencias/evidencia-organizacion.md` | Aprobar cambios vía revisión sincrónica |
| Tablero de Trello | Tareas, responsables y fechas | Alex Vásquez | **OK (Activo)** | 22/10/2026 | No aplica | `docs/07-evidencias/tablero-trello-marketia.md` | Tablero GitHub Projects integrado |
| OmniRoute (instalación o servicio) | Enrutar consultas al LLM | Nelson Zapata | **PENDIENTE (A la espera de autorización docente)** | 22/10/2026 | `.env.local` | `docs/07-evidencias/registro-prueba-viabilidad.md` | Integración directa con proveedores LLM |
| Proveedor de LLM 1 (nombre: OpenAI GPT-4o-mini) | FODA y demanda | Nelson Zapata | **OK (Verificado)** | 22/10/2026 | `.env.local` (`OPENAI_API_KEY`) | `docs/07-evidencias/registro-prueba-viabilidad.md` | Cambiar a Gemini 1.5 Flash |
| Proveedor de LLM 2, plan B (nombre: Google Gemini 1.5 Flash) | Respaldo si falla el principal | Nelson Zapata | **OK (Verificado)** | 22/10/2026 | `.env.local` (`GEMINI_API_KEY`) | `docs/07-evidencias/registro-prueba-viabilidad.md` | Anthropic Claude 3.5 Haiku |
| Hosting del frontend (nombre: Vercel) | Publicar la demostración | Cristian García | **OK (Configurado)** | 22/10/2026 | Variables de entorno en panel Vercel | Enlace público en el `README.md` | Netlify / Render Frontend |
| Hosting del backend (nombre: Render) | Ejecutar la API | Nelson Zapata | **OK (Configurado)** | 22/10/2026 | Variables de entorno en panel Render (`.env`) | Logs de despliegue en Render | Railway / Fly.io |
| Base de datos (PostgreSQL o SQLite) | Persistencia, solo si se ratifica D6 | Nelson Zapata | **NO APLICA (Recortado)** | 22/10/2026 | `.env.local` | `docs/actas/acta-01-ratificacion.md` | Reporte renderizado únicamente en pantalla |
| Dominio o URL de la demostración | Acceso del docente y usuarios de prueba | Alex Vásquez | **OK (Generado)** | 22/10/2026 | No aplica | Enlace de previsualización en `README.md` | Localhost mediante Ngrok para la defensa |
| Google Drive y WhatsApp | Documentos, actas y avisos | Alex Vásquez | **OK (Activo)** | 22/10/2026 | No aplica | Repositorio GitHub carpeta `docs/` | Mensajería institucional Unifranz |


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
| Hosting | Plan Gratuito (Vercel / Render Free Tier) | 0,00 BOB | 100 GB ancho de banda (Vercel), 512 MB RAM con spin-down (Render). | Vercel & Render Pricing, 22/10/2026 |
| Base de datos | Plan Gratuito (SQLite en memoria / Supabase Free) | 0,00 BOB | 500 MB almacenamiento (Sin uso activo por recorte D6). | Supabase Pricing, 22/10/2026 |
| LLM (costo por informe, medido en la prueba) | Pago por uso (Pay-as-you-go) con saldo de prueba | ~0,014 BOB por informe (~$0,002 USD) | ~$5,00 USD saldo gratuito inicial (~35 BOB), rinde para ~2.500 informes. | OpenAI / Google AI Studio Docs, 22/10/2026 |
| Dominio | Plan Gratuito (`.vercel.app` / `.onrender.com`) | 0,00 BOB | Subdominios públicos incluidos ilimitados. | Vercel / Render Docs, 22/10/2026 |
| **TOTAL ESTIMADO MES** | **Presupuesto 100% Gratuito para MVP** | **0,00 BOB** | **Suficiente para pruebas de campo y evaluación docente** | **`docs/06-auditoria/cuestionario-aprobacion.md`** |
## 4. Entorno de ejecución

| Dato | Valor |
|---|---|
| Versión de Python | Python 3.11.x (o superior) |
| Versión de Node | Node.js v18.x / v20.x LTS |
| Sistema operativo del equipo | Windows 11 / Linux (Ubuntu 22.04 LTS) / macOS |
| Pasos para ejecutar el proyecto (resumen) | **1. Clonar el repositorio:**<br>`git clone https://github.com/zapatanelsonzapata03-design/PEF1-2026-MARKETIA.git`<br><br>**2. Configurar variables de entorno:**<br>Copiar `.env.example` a `.env.local` e ingresar la clave de API (`OPENAI_API_KEY` o `GEMINI_API_KEY`).<br><br>**3. Iniciar Backend (FastAPI):**<br>`cd src/backend && python -m venv venv && source venv/bin/activate && pip install -r requirements.txt && uvicorn main:app --reload`<br><br>**4. Iniciar Frontend (React/Next.js):**<br>`cd src/frontend && npm install && npm run dev`<br><br>**5. Abrir en navegador:**<br>Navegar a `http://localhost:3000`. |
| ¿Otro integrante pudo ejecutarlo siguiendo estos pasos? | **Sí.** Cristian García y Alex Vásquez verificaron el despliegue local en sus respectivos entornos siguiendo estas instrucciones sin requerir asistencia externa (Prueba P50 superada exitosamente). |

## 5. Pendientes

| Falta | Responsable | Fecha límite | Resuelto |
|---|---|---|---|
| | | | |
