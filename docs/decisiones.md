# Registro de decisiones del proyecto

Este registro distingue las **propuestas listas para ratificar** de los
**acuerdos confirmados**. Una decisión pasa a estar aprobada solo cuando se
completa el [acta de ratificación](actas/acta-01-ratificacion.md) con fecha,
participantes y evidencia (por ejemplo, captura de la reunión o del chat).

**Reunión de ratificación propuesta:** viernes 16 de octubre de 2026,
20:00, por videollamada (confirmar con el equipo). Duración prevista: 60 minutos.

| ID | Tema | Propuesta lista para ratificar | Criterios |
|---|---|---|---|
| D1 | Usuario prioritario | Emprendedores y microempresarios de Cochabamba que planifican o inician un negocio sencillo de comercio o servicios. Estudiantes y asesores/incubadoras son usuarios secundarios (versión posterior), aunque se incluyan en la muestra de prueba del informe. | P2, P11 |
| D2 | Contenido del MVP | Formulario → cálculos fijos de costos y punto de equilibrio → FODA y estimación de demanda con IA, etiquetados y con supuestos visibles → informe en pantalla. | P21-P22 |
| D3 | Investigación de mercado | En el MVP, la persona ingresa los competidores que conoce y sus precios. El equipo reúne datos reales con visitas de campo (informe, tarea 10) para probar el sistema. La búsqueda automática se pospone a la versión 2. **Esto exige corregir la Meta 1 del informe** (ver D12). | P26, P29, P47 |
| D4 | PDF | MVP: impresión del navegador. Exportación PDF propia: v1.1. | P19-P20 |
| D5 | Exclusiones del MVP | Cuentas e inicio de sesión, pagos, aplicación móvil nativa, cobertura fuera de Cochabamba, panel administrativo, historial, versión para asesores e idiomas distintos del español. Los planes de pago del informe (Básico, Individual, Institucional) son proyección para 2027, **fuera del alcance académico**. | P17-P18 |
| D6 | Persistencia y privacidad | PostgreSQL guarda solo la entrada y el informe, con identificador aleatorio, sin nombre, correo, teléfono ni cédula. Retención de 90 días y borrado por identificador. Aviso y casilla de aceptación antes de enviar la idea al proveedor de IA. | P31-P32 |
| D7 | Proveedor de LLM | OmniRoute como opción principal para el piloto, condicionada a una prueba de viabilidad. Plan B: otro proveedor compatible. Sin credenciales en el repositorio. | P27-P29 |
| D8 | Idioma y moneda | Español y bolivianos (Bs). | P15 |
| D9 | Flujo de trabajo Git | Ramas por tarea, cambios por pull request con aprobación de otra persona, `main` protegida. Ver [`equipo/roles-y-acuerdos.md`](../equipo/roles-y-acuerdos.md). | P42 |
| D10 | Autorización docente | Solicitar por escrito autorización para la prueba de viabilidad, el desarrollo en `src/` y el protocolo de entrevistas. El registro del 15/10/2026 documenta el envío del enlace del repositorio, pero no una respuesta escrita ni autorización. Se requiere registrar una autorización expresa antes de actuar. Ver [`solicitud-autorizacion-docente.md`](07-evidencias/solicitud-autorizacion-docente.md). | P46, P48 |
| D11 | Reparto de responsabilidades | Unificar con los roles del README: Nelson (motor e IA), Cristián (pantalla y calidad), Alex (coordinación, informe y costos del proyecto). **Corregir el informe**: en el Gantt de la Etapa 1, las tareas 2, 3 y 4; en las Etapas 2 y 3, las tareas 11, 12, 13 y 14; en la tabla de pruebas, las filas "De fórmulas" y "De facilidad de uso". Detalle en [`equipo/roles-y-acuerdos.md`](../equipo/roles-y-acuerdos.md). | P36, P41 |
| D12 | Meta 1 del informe | Reformular: "Reducir al menos 70 % el tiempo para obtener el análisis completo frente a hacerlo a mano, usando datos de competencia ingresados o recolectados". Línea base: cronometrar el trabajo manual en 3 casos antes del 13 de noviembre. | P7, P10 |
| D13 | Muestras | Entrevistas exploratorias: 8 a 10 emprendedores (Fase A). Pruebas tempranas de usabilidad: 5 personas. Prueba piloto: 30 personas (diciembre). Si el tiempo lo permite, ampliar a 43. | P34 |
| D14 | Herramientas de seguimiento | Trello para tareas (columnas: pendiente, en curso, en revisión, terminada), GitHub para código y pull requests, Drive y WhatsApp para documentos y avisos. Exportar capturas de Trello a `docs/07-evidencias/`. | P36, P42 |
| D15 | Materia | Confirmar con el docente si el proyecto corresponde a Probabilidad y Estadística o a Programación II - P2. Hasta recibir respuesta, el README menciona ambas. | P46 |

## Registro de ratificación

| Fecha | IDs ratificados | Quiénes participaron | Evidencia |
|---|---|---|---|
| Completar tras la reunión | Completar | Completar | Enlace al acta y captura |

## Condiciones

- No se marca ninguna decisión como aprobada sin acta.
- Las decisiones que requieren autorización docente (D10, D15) se registran
  junto con su respuesta.
- No registrar claves, contraseñas, tokens ni archivos de entorno.
