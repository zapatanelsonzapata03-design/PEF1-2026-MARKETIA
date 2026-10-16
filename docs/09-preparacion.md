# Preparación para desarrollar

Estado según lo que consta en el repositorio. "No registrado" significa que no
hay evidencia aquí, no necesariamente que el recurso no exista.

## 1. Estado de los requisitos

| Requisito o decisión | Estado en el repositorio | Paso necesario | Fecha propuesta |
|---|---|---|---|
| Ratificación de D1 a D15 | Propuestas listas; acta sin completar | Reunión y [acta 01](actas/acta-01-ratificacion.md) | Vie 16 oct |
| Autorización para la prueba de viabilidad técnica | No registrada | Enviar [solicitud](07-evidencias/solicitud-autorizacion-docente.md); guardar respuesta | Enviar 16 oct; respuesta antes del 20 oct |
| Autorización para iniciar el desarrollo | No registrada | Misma solicitud; `src/` sin código hasta tener respuesta | Respuesta antes del 24 oct |
| Usuario y problema validados | Protocolo listo; sin entrevistas | Aplicar entrevistas ([protocolo](07-evidencias/protocolo-entrevistas.md)) | 17 al 20 oct |
| Referencias verificadas | Transcritas del informe; sin verificar | Verificar enlaces y cifras ([referencias](01-proyecto/referencias.md)) | Lun 19 oct |
| Cotizaciones locales | No registradas | [Guion](07-evidencias/guion-cotizaciones.md) | 16 al 19 oct |
| Datos y permisos para la prueba de LLM | No registrados | Usar solo casos de ejemplo; consentimiento si hay personas | Antes de A4 |
| Proveedor y hosting | No registrados | Elegir y documentar tras A4 | Antes del 6 nov |
| Base de datos y política de retención | No registradas | Confirmar recurso y aprobar D6 | Antes de B6 |
| Diez casos de referencia | **Diez casos sintéticos documentados**; faltan 3 negocios reales | Revisión independiente y 3 casos reales | Mié 21 oct |
| Horas semanales y reuniones | **Propuestas** (21 h en fase A; 8 h semanales después; lun, mié y vie 20:00) | Confirmar en el acta | Vie 16 oct |
| Herramienta de tareas | Trello (según el informe); sin evidencia | Captura del tablero en `07-evidencias/` | Mar 20 oct |
| Protección de `main` y pull requests | No comprobada | Configurar en GitHub y guardar captura | Mar 20 oct |
| Materia del proyecto | README e informe: Probabilidad y Estadística; cuestionario: Programación II - P2 | Confirmar con el docente (D15) | Respuesta antes del 20 oct |

## 2. Qué construye cada uno primero
Hasta tener la autorización docente, el trabajo se limita a documentación y
planificación; no se inicia desarrollo en `src/`.

| Integrante | Ahora (fase A) | Primero al autorizarse el desarrollo (26 oct) |
|---|---|---|
| Alex | Acta, solicitud al docente, referencias, cotizaciones, informe y diapositivas | Informe final, coordinación y evidencias |
| Nelson | Prueba de viabilidad (con autorización), validación de los casos de fórmulas | B1 esqueleto y contrato de API; B2 motor de cálculos |
| Cristián | Entrevistas, criterios de aceptación, plan de pruebas | B4 formulario con validación |

## 3. Nuevo integrante: qué leer
README → `docs/decisiones.md` → `docs/02-requisitos/` → `docs/04-planificacion/`
→ `equipo/roles-y-acuerdos.md`. El informe final está en
`docs/01-proyecto/MarketIA_informe_final.pdf`.

No colocar claves, contraseñas, tokens ni archivos de entorno en este
repositorio.
