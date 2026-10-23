# Evidencia de organización del equipo

> Respalda parcialmente las preguntas 36, 38 y 42. La captura acredita que se
> ve un tablero y algunas tarjetas; no acredita que estén cargadas todas las
> tareas, sus responsables y fechas, que el equipo siga un flujo de revisión,
> ni que `main` esté protegida.
>
> Las capturas de una interacción preliminar de un caso con OmniRoute están
> registradas en [`README.md`](README.md#prueba-preliminar-de-omniroute). La
> prueba ampliada de diez ideas tiene una plantilla separada en
> [`registro-prueba-viabilidad.md`](registro-prueba-viabilidad.md) y requiere
> autorización escrita del docente.

## 1. Tablero de Trello

| Campo | Dato |
|---|---|
| Enlace de invitación para observar el tablero | [Abrir tablero MarketIAa en Trello](https://trello.com/invite/b/6adae6323692211b8f10f761/ATTI14406b1bb31e10484325c7061f29c5d5B9A3E9FB/marketiaa) |
| Fecha de creación reportada | 22/10/2026 |
| Fecha visible de la captura | 23/10/2026 |
| Listas visibles | Backlog, To Do, In Progress, Code Review / QA y Done |
| Contadores visibles en la captura | Backlog: 4; To Do: 4; In Progress: 3; Code Review / QA: 3; Done: 8 |
| Tarjetas del plan A1–A9 y B1–B12 | No se verifica que estén todas; la captura muestra algunas tarjetas y tareas en distintos estados |
| Responsables y fechas en cada tarjeta | No se pueden verificar en esta captura |
| Captura | [`trello-tablero-2026-10-23.png`](trello-tablero-2026-10-23.png) |

La captura y el enlace de invitación aportado permiten documentar el tablero
para observación; no se verificó desde el repositorio el alcance de permisos
que Trello concede al abrir el enlace. La presencia de una lista `Done` no
demuestra que el proyecto esté completo: también se observan tarjetas en
Backlog, To Do, In Progress y Code Review / QA.

## 2. Protección de la rama `main` en GitHub

El repositorio pertenece a la cuenta `zapatanelsonzapata03-design`, así que
quien administre esa cuenta debe hacer este cambio.

1. En el repositorio: **Settings**.
2. Ir a **Branches** (o **Rules → Rulesets**, según lo que muestre GitHub).
3. Crear una regla para la rama `main`.
4. Activar **Require a pull request before merging** y exigir **1 aprobación**.
5. Guardar y tomar captura de la regla.

| Campo | Dato |
|---|---|
| Fecha de configuración | |
| Quién la configuró | |
| Aprobaciones exigidas | |
| Configuración visible en captura | Require a pull request before merging; 1 aprobación requerida; "Require an additional approval for unattributed Copilot pull requests" marcado |
| Captura | [`proteccion-main-2026-10-23.png`](proteccion-main-2026-10-23.png) |

La captura muestra estos controles en la configuración de reglas de rama, pero
el recorte no deja visible el patrón de rama al que se aplica ni confirma por
sí solo que la regla esté guardada y activa específicamente para `main`. Falta
verificar ese alcance en la configuración completa.

## 3. Pull requests y ramas

| Campo | Dato |
|---|---|
| Captura del listado | [`pull-request-revisado-2026-10-23.png`](pull-request-revisado-2026-10-23.png) muestra la lista filtrada de PR cerradas; PR #9 aparece como fusionada |
| Convención de ramas acordada | `feat/<área>-<descripción>` y `docs/<descripción>` |
| Revisor de cada pull request | Una persona distinta a la autora |
| Revisión semanal de pull requests abiertos | Viernes, reunión de las 20:00 |

La captura del listado acredita el estado visible de cierre/fusión, no que cada
PR haya recibido una aprobación de revisión independiente.

## 4. Reuniones

| Campo | Dato |
|---|---|
| Reuniones acordadas en el acta 01 | |
| Notas de 3 líneas al cierre de cada reunión (avance, bloqueo, siguiente paso) | ( ) se están guardando en el grupo |
