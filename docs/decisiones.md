# Registro de decisiones del proyecto

Este registro separa propuestas documentadas de acuerdos confirmados. Una
propuesta no se considera aprobada hasta que el equipo la ratifique y anote
quién la aprobó y cuándo. No se han registrado actas ni aprobaciones en el
repositorio.

| ID | Tema | Propuesta para ratificar | Estado / criterio relacionado |
|---|---|---|---|
| D1 | Usuario prioritario | Emprendedores o microempresarios de Cochabamba que planifican un negocio sencillo de comercio o servicios. Estudiantes, asesores e incubadoras quedarían para una versión posterior. | Pendiente de aprobación y validación con usuarios (P2, P11). |
| D2 | Contenido del MVP | Formulario → cálculos fijos de costos y punto de equilibrio → FODA y estimación de demanda con IA, claramente etiquetados → informe en pantalla. | Pendiente de aprobación (P21–P22). |
| D3 | Investigación de mercado | En el MVP, la persona usuaria ingresaría los competidores que conoce y sus precios; la búsqueda automática se pospondría. | Pendiente de aprobación. Requiere definir datos y privacidad (P26, P29, P47). |
| D4 | PDF | Para el MVP se usaría la impresión del navegador; la exportación PDF propia se pospondría a v1.1. | Pendiente de aprobación (P19–P20). |
| D5 | Exclusiones de producto | Cuentas, inicio de sesión, pagos, aplicación móvil nativa, cobertura fuera de Cochabamba, panel administrativo e idiomas distintos del español quedarían fuera. | Pendiente de aprobación (P17–P18). |
| D6 | Persistencia y privacidad | Como alternativa de diseño, PostgreSQL guardaría solo la entrada necesaria y el informe, asociados a un identificador aleatorio, sin nombre, correo, teléfono ni cédula; retención propuesta de 90 días y borrado por identificador. | Pendiente de aprobación y revisión de privacidad. No es una garantía de cumplimiento ni está implementado (P31–P32). |
| D7 | Proveedor de LLM | OmniRoute sería la opción principal solo si supera una prueba de viabilidad; otro proveedor compatible sería el plan B. | Pendiente de aprobación y prueba. No registrar credenciales en este repositorio (P27–P29). |
| D8 | Idioma y moneda | Interfaz y reporte en español; cantidades monetarias en bolivianos (Bs). | Pendiente de aprobación (P15). |
| D9 | Flujo de trabajo Git | Ramas por tarea, cambios mediante pull request, revisión de otra persona y documentación/pruebas para cerrar una tarea. | Propuesta pendiente de acuerdo del equipo y de configurar las protecciones correspondientes (P42). |
| D10 | Autorización docente | Solicitar autorización para una prueba de viabilidad técnica y, por separado, para iniciar el desarrollo. | No hay respuesta ni autorización registrada; confirmar el procedimiento con el docente (P46, P48). |

## Registro de ratificación

| Fecha | Decisión o IDs ratificados | Quiénes participaron | Evidencia (acta o enlace) |
|---|---|---|---|
| Pendiente | Pendiente | Pendiente | Pendiente |

## Condiciones antes de cerrar decisiones

- Confirmar las propuestas con el equipo y registrar la ratificación.
- Acordar las decisiones que requieren autorización docente antes de actuar.
- Completar los datos reales indicados como pendientes en la auditoría y en
  `docs/09-preparacion.md`.
- No registrar claves, contraseñas, tokens ni valores de archivos de entorno en
  este documento ni en el repositorio.
