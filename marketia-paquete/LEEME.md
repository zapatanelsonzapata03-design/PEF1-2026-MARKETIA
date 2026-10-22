# Paquete para el repositorio MarketIA

Todo está en las mismas rutas que usa el repositorio. Descomprime el ZIP en la
raíz del proyecto (o copia cada archivo a su carpeta). **Nada viene rellenado
con datos inventados:** los campos en blanco los completa el equipo con hechos
reales, como pide `.clinerules`.

| Archivo | Qué hacer | ¿Reemplaza o es nuevo? |
|---|---|---|
| `docs/06-auditoria/checklist-cierre-24-oct.md` | Seguir día por día hasta la presentación | Nuevo |
| `docs/actas/acta-01-ratificacion.md` | Completar en la reunión de ratificación | Reemplaza el actual |
| `docs/01-proyecto/verificacion-referencias.md` | Verificar las fuentes y cifras del problema | Nuevo |
| `docs/07-evidencias/registro-prueba-viabilidad.md` | Registrar la prueba de OmniRoute (solo con autorización) | Nuevo |
| `docs/07-evidencias/evidencia-organizacion.md` | Enlace de Trello, protección de `main`, pull requests | Nuevo |
| `docs/08-presentacion/hecho-vs-planificado.md` | Base de la diapositiva "qué está hecho y qué no" | Nuevo |

Ya existen en el repositorio y **no hace falta reescribirlos**:
`solicitud-autorizacion-docente.md` (enviarla tal cual),
`protocolo-entrevistas.md`, `consentimiento-informado.md`,
`ficha-registro-entrevista.md`, `plantilla-tabulacion.csv`,
`registro-entrevistas.md` y `guion-cotizaciones.md`.

## Texto para el README (reemplazar la sección "Estado actual")

Copia este bloque y deja solo lo que sea verdad el día que lo pegues. Cambia
`[ ]` por `[x]` únicamente si el archivo de evidencia ya está en el repositorio.

```markdown
## Estado actual
Actualizado el __ de octubre de 2026. Documentación redactada. Avance de las
acciones que dependen del equipo y de terceros:

- [ ] Acta 01 completada (`docs/actas/acta-01-ratificacion.md`)
- [ ] Solicitud enviada al docente y respuesta guardada (`docs/07-evidencias/`)
- [ ] Referencias verificadas (`docs/01-proyecto/verificacion-referencias.md`)
- [ ] Entrevistas aplicadas: __ de 8 (`docs/07-evidencias/registro-entrevistas.md`)
- [ ] Cotizaciones obtenidas: __ de 2
- [ ] 10 casos de fórmulas revisados por una segunda persona
- [ ] Prueba de viabilidad de OmniRoute (`docs/07-evidencias/registro-prueba-viabilidad.md`)
- [ ] Tablero de Trello y protección de `main` (`docs/07-evidencias/evidencia-organizacion.md`)

Lo que no tiene casilla marcada **no está validado**. El desarrollo en `src/`
empieza solo con autorización del docente.
```

También reemplaza en el README `**agregar aquí**` por el enlace real del
tablero de Trello cuando exista.
