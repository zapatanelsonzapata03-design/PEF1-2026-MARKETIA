# Preparación para desarrollar

Estado según la evidencia disponible en el repositorio al 22 de octubre de
2026. "No registrado" significa que no hay evidencia aquí, no necesariamente
que el recurso o la actividad no exista. Las fechas propuestas que ya pasaron
no demuestran que una tarea se haya realizado; el equipo debe reprogramar lo
pendiente.

## 1. Estado de los requisitos

| Requisito o decisión | Estado documentado | Paso pendiente |
|---|---|---|
| Ratificación de D1 a D15 | Acta 01 sin completar; las decisiones siguen siendo propuestas | Reunión del equipo y registro de acuerdos reales en [`acta-01-ratificacion.md`](actas/acta-01-ratificacion.md) |
| Autorización para prueba técnica y desarrollo | La solicitud registra el envío del enlace del repositorio el 15/10/2026; no consta respuesta escrita ni autorización | Consultar al equipo/docente si corresponde presentar una solicitud formal; esperar autorización escrita antes de probar o desarrollar |
| Protocolo de entrevistas | Se aportaron ocho resúmenes; no constan fichas completas de las 24 preguntas, consentimiento ni autorización escrita | Verificar la documentación y permisos antes de presentar los resúmenes como evidencia validada |
| Referencias y cifras del informe | Transcritas; verificación pendiente | Comprobar enlaces, cifras, población y ubicación en la fuente en [`verificacion-referencias.md`](06-auditoria/verificacion-referencias.md) |
| Cotizaciones locales | Dos capturas muestran consultas enviadas; no registran respuestas ni cotizaciones recibidas | Obtener respuestas de dos proveedores distintos y guardar cotizaciones reales |
| Datos y permisos para prueba de LLM | No registrados; prueba técnica no autorizada | No usar datos reales ni realizar la prueba antes de obtener autorización |
| Proveedor y hosting | No registrados | Decidir y documentar recursos después de las verificaciones y autorizaciones necesarias |
| Base de datos y política de retención | Decisión propuesta, sin ratificación documentada | Confirmar recursos y aprobar la decisión en acta |
| Casos de referencia | Diez casos sintéticos documentados y un recálculo aritmético preliminar; revisión independiente y pruebas del sistema pendientes | Cristián debe recalcular por su cuenta y documentar su revisión si la realiza; usar casos reales solo con autorización y anonimización |
| Horas semanales y reuniones | Propuestas, sin ratificación en acta | Confirmar en reunión y registrar el acuerdo |
| Herramienta de tareas | Trello se menciona en el informe; no hay evidencia del tablero | Registrar enlace y captura en [`evidencia-organizacion.md`](07-evidencias/evidencia-organizacion.md) si el tablero existe |
| Protección de `main` y pull requests | No comprobada en la evidencia del repositorio | Verificar configuración y guardar captura, sin afirmar que está activa antes de comprobarlo |
| Accesos y hosting | Plantilla de control creada, sin completar | Registrar únicamente recursos y permisos efectivamente comprobados en [`09-accesos-y-hosting.md`](09-accesos-y-hosting.md) |
| Materia del proyecto | README e informe: Probabilidad y Estadística; cuestionario: Programación II - P2. No consta aclaración docente | Confirmar la materia con el docente (D15) |

## 2. Qué construye cada integrante

Hasta recibir una nueva autorización expresa del docente, el trabajo se limita
a documentación y planificación; `src/` permanece sin código.

| Integrante | Trabajo documental pendiente | Después de autorizarse el desarrollo |
|---|---|---|
| Alex Vásquez Pérez (coordinador) | Coordinar acuerdos, solicitud docente, referencias, cotizaciones, informe y evidencias | Coordinación, informe final y evidencias |
| Nelson Zapata Jiménez (motor e IA) | Preparar el registro de prueba y validar casos de fórmulas; la prueba de OmniRoute requiere autorización | B1 esqueleto y contrato de API; B2 motor de cálculos |
| Cristián García Bustamante (pantalla y calidad) | Revisar protocolo, criterios de aceptación y plan de pruebas; entrevistas sujetas a autorización | B4 formulario con validación |

La fecha de inicio prevista anteriormente no es autorización. El equipo debe
reprogramar las tareas pendientes y ratificar cualquier cambio en el acta.

## 3. Incorporación al equipo

README → `docs/decisiones.md` → `docs/02-requisitos/` →
`docs/04-planificacion/` → `equipo/roles-y-acuerdos.md`. El informe final está
en `docs/01-proyecto/MarketIA_informe_final.pdf`.

No colocar claves, contraseñas, tokens ni archivos de entorno en este
repositorio.
