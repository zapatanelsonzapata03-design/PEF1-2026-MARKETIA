# Roles y acuerdos de trabajo

> Los roles provienen del README y del informe final. El reparto de tareas, las
> horas y las reuniones son **propuestas listas para ratificar** en el
> [acta 01](../docs/actas/acta-01-ratificacion.md). Se vuelven acuerdos cuando
> el acta se completa y se guarda su evidencia.

## 1. Roles y entregables verificables

| Integrante | Rol | Entregables verificables | Respaldo |
|---|---|---|---|
| Alex Vásquez Pérez | Coordinador del proyecto | Decisiones y actas, calendario, referencias y evidencias, costos del proyecto, informe final, diapositivas | Cristián (documentación) |
| Nelson Zapata Jiménez | Líder del motor y la IA | Diseño del sistema y configuración de OmniRoute, prueba de viabilidad, endpoint `/analisis`, motor de cálculos con 10 casos aprobados, integración con el LLM, pruebas técnicas y de fórmulas | Cristián (API y pruebas) |
| Cristián García Bustamante | Líder de la pantalla y la calidad | Prototipo de pantallas, formulario, pantalla de informe, persistencia mínima, pruebas de recorrido y de usabilidad, guías de usuario | Nelson (interfaz y pruebas cruzadas) |

### Ajuste necesario en el informe (decisión D11)
El informe asigna algunas tareas en sentido contrario a los roles. Para que
repositorio e informe digan lo mismo, se propone corregir el informe:

| Dónde en el informe | Dice | Debe decir |
|---|---|---|
| Etapa 1, tarea 2 (diseño del sistema y OmniRoute) | Cristián | Nelson |
| Etapa 1, tarea 3 (prototipo de pantallas) | Nelson | Cristián |
| Etapa 1, tarea 4 (prueba FODA e informe con IA) | Cristián | Nelson |
| Etapas 2 y 3, tareas 11, 12 y 13 (módulos de datos, IA y costos) | Cristián (y Alex en la 13) | Nelson (Alex apoya en la 13 con las fórmulas) |
| Etapas 2 y 3, tarea 14 (pantalla web) | Nelson | Cristián |
| Tabla de pruebas: "De fórmulas" | Cristián | Nelson, con revisión de Cristián |
| Tabla de pruebas: "De facilidad de uso" | Nelson | Cristián |

## 2. Disponibilidad (propuesta)

| Periodo | Compromiso por persona | Qué incluye |
|---|---|---|
| Fase A: 15 al 24 de octubre | **21 horas** en total (≈ 16 h por semana, intensivo) | Tareas de la fase A (15 a 18 h según la persona) y 4 reuniones |
| Fase B: 26 de octubre al 19 de diciembre | **3 horas por día** | Días de trabajo por semana y distribución entre reuniones y trabajo individual, pendientes de confirmar |

La estimación de tareas de la fase B es de **112 h**. La disponibilidad de 3 h
por día es una propuesta reportada; falta confirmar cuántos días por semana
trabajará cada persona y cuánto tiempo se destinará a reuniones. Por eso, la
capacidad total y el margen frente a las 112 h aún no se pueden calcular. El
cálculo anterior que suponía 8 h semanales por persona queda reemplazado. Si
alguien no puede cumplir las horas que se ratifiquen, se aplica el recorte del
40 % del [documento de requisitos](../docs/02-requisitos/alcance-mvp-y-requisitos.md).

Estas cifras son propuestas y deben confirmarse en el acta.
Cada integrante debe confirmarlas o corregirlas en el acta.

## 3. Reuniones (propuesta)

| Reunión | Cuándo | Duración | Medio |
|---|---|---|---|
| Reunión de seguimiento | Lunes, miércoles y viernes, 20:00 | 45 min | Videollamada |
| Planificación de sprint | Lunes de la primera semana de cada sprint, 20:00 | 60 min (reemplaza la del lunes) | Videollamada |
| Cierre y retrospectiva | Viernes de la segunda semana del sprint, 20:00 | 60 min (reemplaza la del viernes) | Videollamada |
| Ratificación (acta 01) | Viernes 16 de octubre de 2026, 20:00 | 60 min | Videollamada |

Calendario de la fase A: viernes 16, lunes 19, miércoles 21 y viernes 23 de
octubre. Presentación en clase: sábado 24 de octubre. Los sprints de dos
semanas están en el [plan](../docs/04-planificacion/plan-desarrollo-y-riesgos.md).

Cada reunión termina con una nota de 3 líneas en el grupo: qué se avanzó, qué
bloquea y qué sigue. Una vez por sprint se guarda un acta breve en `docs/actas/`.

## 4. Herramientas y flujo de trabajo

1. **Trello:** una tarjeta por tarea con responsable, fecha y estado (pendiente,
   en curso, en revisión, terminada).
2. **GitHub:** `main` protegida; no se sube directo a ella.
3. Ramas por tarea: `feat/<área>-<descripción>` y `docs/<descripción>`.
4. Todo cambio entra por pull request con aprobación de **otra persona**.
5. Una tarea está terminada cuando cumple su criterio de aceptación, tiene
   pruebas y la documentación actualizada.
6. Las decisiones se registran en [`docs/decisiones.md`](../docs/decisiones.md).
7. Evidencia de que esto se cumple: capturas del tablero y de la configuración de
   `main` en `docs/07-evidencias/`. Hasta que existan, estos pasos son
   acuerdos propuestos, no configuración comprobada.

## 5. Revisión e integración
Una persona distinta a quien hizo el cambio revisa cada pull request y
comprueba los criterios de aceptación. Al menos dos integrantes conocen las
decisiones, el contrato de API y las pruebas de cada componente. Cada semana,
en la reunión del viernes, se revisan los pull requests abiertos.

## 6. Continuidad si alguien no está disponible
- Fórmulas, contrato de API, decisiones y casos de prueba están documentados.
- Cada componente tiene un respaldo (tabla 1).
- Si falta Nelson: Cristián continúa sobre el contrato aprobado y las pruebas
  existentes, y se aplica el recorte del 40 %.
- Si falta Cristián: Nelson continúa con una interfaz mínima y Alex asume las
  pruebas con usuarios.
- Si falta Alex: Cristián asume actas y evidencias, y Nelson el seguimiento del
  calendario.
