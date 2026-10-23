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
| Repositorio GitHub (`zapatanelsonzapata03-design`) | Código, pull requests, `main` protegida | | | | No aplica | | |
| Permisos de Alex y Cristián en el repositorio | Revisar y aprobar pull requests | | | | No aplica | | |
| Tablero de Trello | Tareas, responsables y fechas | | | | No aplica | | |
| OmniRoute (instalación o servicio) | Enrutar consultas al LLM | | | | | | Otro proveedor compatible |
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
