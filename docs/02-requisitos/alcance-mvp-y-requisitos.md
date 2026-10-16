# Alcance, MVP y requisitos

> Especificación propuesta a partir del paquete de mejoras. Los acuerdos D1–D9
> requieren ratificación del equipo en `docs/decisiones.md`; estos requisitos
> no describen funciones implementadas.

## Usuarios y necesidades

El usuario prioritario propuesto es el emprendedor o microempresario de
Cochabamba que está planificando un negocio de comercio o servicios simples.
Estudiantes, asesores e incubadoras se proponen como usuarios posteriores.
Esta prioridad aún debe aprobarse y validarse con usuarios.

| Usuario propuesto | Necesidad | Funcionalidad relacionada |
|---|---|---|
| Emprendedor | Saber cuánto debe vender para no perder. | RF-04 |
| Emprendedor | Entender riesgos y oportunidades de la idea. | RF-03 |
| Emprendedor | Describir la idea sin conocimientos técnicos. | RF-01 |
| Emprendedor | Consultar un informe para evaluar la idea o conversar sobre financiamiento. | RF-05 |

## MVP propuesto

**MVP v1.0:** formulario → cálculos fijos → FODA y estimación de demanda con IA
etiquetados y con supuestos visibles → informe en pantalla.

El propósito es ayudar a responder cuánto habría que vender para cubrir los
costos y qué riesgos merece revisar. Los cálculos serían verificables; el FODA
y la demanda serían orientativos, no datos verificados. El usuario ingresaría
competidores y precios que conoce; no habría búsqueda automatizada en el MVP.

La exportación PDF propia queda propuesta para v1.1. Para v1.0, la persona
podría imprimir o guardar la página como PDF desde el navegador. El MVP y su
valor deben ser ratificados por el equipo y el docente.

## Requisitos funcionales y criterios propuestos

### RF-01 — Formulario de idea de negocio

**Campos propuestos:** nombre del negocio; rubro; descripción de 50 a 1000
caracteres; zona de Cochabamba; precio de venta por unidad en Bs; costo
variable por unidad en Bs; costos fijos mensuales en Bs; inversión inicial
opcional; competidores conocidos opcionales, con nombre comercial y precio.

El formulario no solicitaría nombre de la persona, correo, teléfono ni cédula.
El equipo debe revisar si el nombre comercial y la descripción pueden contener
datos identificables y añadir advertencias y controles apropiados antes de
enviar información a un proveedor.

- Dado un formulario válido, al enviarlo el sistema confirma la recepción e
  inicia la generación del informe.
- Dado un campo numérico vacío, negativo o no numérico, el sistema indica qué
  campo corregir y no genera el análisis.
- Si el texto contiene datos personales directos, el sistema advierte que no
  se deben ingresar y evita o minimiza su envío según una regla por definir.
- La zona debe corresponder al alcance de Cochabamba acordado por el equipo.

### RF-02 — Competencia conocida por la persona usuaria

En el MVP no se propone búsqueda automática de competencia, precios o
tendencias; la persona usuaria ingresaría los competidores y precios que
conoce. La búsqueda automática queda para una versión posterior.

- Si se ingresan competidores, el informe los lista con sus precios y muestra
  promedio y rango.
- Si no se ingresa ninguno, el informe indica “sin datos” en esa sección.
- No se presentan precios ingresados por el usuario como si fueran una
  investigación independiente o una fuente verificada.

### RF-03 — FODA y estimación de demanda con IA

- Para una entrada válida, el informe muestra Fortalezas, Oportunidades,
  Debilidades y Amenazas, con al menos dos elementos por cuadrante.
- La demanda se presenta como estimación de nivel bajo, medio o alto, con sus
  supuestos listados. El método y las definiciones de esos niveles deben
  ratificarse antes de desarrollar.
- El contenido generado se etiqueta: “Estimación generada por IA, no es un
  dato verificado”.
- Si el proveedor falla o la respuesta no cumple el formato, se propone un
  reintento; si vuelve a fallar, el sistema conserva los cálculos fijos y avisa
  que FODA y demanda no están disponibles.

### RF-04 — Costos y punto de equilibrio

El cálculo propuesto usa las fórmulas y casos documentados en
`docs/03-arquitectura/datos-seguridad-pruebas.md`.

- Para un caso de referencia aprobado, los resultados coinciden con el cálculo
  revisado, con tolerancia monetaria de ±0,01 Bs.
- Si el precio es menor o igual al costo variable unitario, se muestra:
  “Inviable con estos datos: el margen es cero o negativo”, y no se calcula el
  punto de equilibrio.
- Las unidades, el periodo y el tratamiento de entradas inválidas deben
  validarse con casos antes de implementar.

### RF-05 — Informe

- La pantalla muestra los datos de negocio ingresados, cálculos, competidores
  ingresados (o “sin datos”), FODA, demanda y avisos.
- Los resultados de fórmulas y las estimaciones de IA aparecen separados y
  etiquetados.
- El informe se puede imprimir o guardar como PDF mediante el navegador. La
  generación PDF propia se pospone a v1.1, sujeta a ratificación.

## Requisitos de calidad propuestos

Los umbrales deben ratificarse. Las mediciones y pruebas no están ejecutadas.

| ID | Requisito | Verificación propuesta |
|---|---|---|
| RNF-01 | Rendimiento: al menos 90 % de 20 ejecuciones terminan en 5 minutos o menos. | Medir desde envío hasta informe visible; registrar las 20 ejecuciones. |
| RNF-02 | Privacidad: no solicitar nombre, correo, teléfono ni cédula; aplicar una política de retención y borrado aprobada. | Revisar esquema y flujo de datos; retención de 90 días y borrado por ID son propuestas D6, todavía no aprobadas. |
| RNF-03 | Transparencia: separar visualmente los cálculos de las estimaciones y etiquetar el contenido de IA. | Prueba de pantalla y revisión de los informes generados. |
| RNF-04 | Usabilidad: al menos 4 de 5 participantes completan el flujo sin ayuda; satisfacción media ≥ 4/5. Interfaz usable desde 360 px de ancho. | Prueba moderada con protocolo y participantes aprobados. |
| RNF-05 | Seguridad: validar entradas, proteger el acceso al proveedor y limitar solicitudes por IP si corresponde. | Revisión y pruebas de seguridad. Si se usan secretos, no se guardan en Git ni en documentación. |
| RNF-06 | Compatibilidad: probar versiones recientes de Chrome y Firefox en escritorio y móvil. | Pruebas manuales documentadas. |
| RNF-07 | Disponibilidad: sin compromiso de operación 24/7; se plantea una demostración. | Acordar entorno y disponibilidad antes de desplegar. |

## Alcance

### Incluido en el MVP propuesto

- Formulario con los campos acordados.
- Datos de competidores ingresados por el usuario, sin búsqueda automática.
- Cálculos fijos de costos y punto de equilibrio.
- FODA y estimación de demanda con IA, supuestos y etiquetas.
- Informe consultable e imprimible desde navegador.
- Pruebas y documentación del MVP.
- Persistencia mínima solo si se ratifica D6; una reducción de alcance podría
  eliminarla.

### Fuera del MVP propuesto

- Cuentas e inicio de sesión.
- Pagos.
- Aplicación móvil nativa.
- Cobertura fuera de Cochabamba.
- Exportación PDF propia (propuesta para v1.1).
- Búsqueda automática de competencia y precios (propuesta para v2).
- Versión para asesores e historial (propuesta para v2).
- Panel administrativo e idiomas distintos del español.

### Funciones atractivas pero no necesarias

Chat con asesor IA, comparación de varias ideas, gráficos animados, proyección
financiera a cinco años, integración con redes sociales y ranking de negocios.
Estas exclusiones son propuestas a ratificar.

### Reducción de alcance del 40 % propuesta

**Conservar:** formulario, cálculos fijos y su validación, informe en pantalla,
y FODA/demanda con IA en versión simple.

**Eliminar o posponer:** almacenamiento en PostgreSQL (informe solo en
pantalla), competidores ingresados, impresión como PDF y pruebas de usabilidad
ampliadas, reducidas a tres usuarios.

Este recorte puede afectar la evaluación de experiencia de usuario; el equipo
debe ratificarlo y acordar qué criterios de éxito seguirían aplicando.

## Realismo y esfuerzo

Las horas indicadas en el plan son estimaciones propuestas, no disponibilidad
confirmada. Las tareas de desarrollo de la fase B suman 86 horas según la
tabla; el paquete las describe aproximadamente como 90 horas. Para afirmar que
el plan cabe en cuatro semanas, el equipo debe confirmar sus horas semanales,
fechas límite y trabajo académico concurrente.

## Decisiones que deben ratificarse

Consultar `docs/decisiones.md`: usuario prioritario, contenido del MVP,
competencia manual, alcance PDF, exclusiones, persistencia/retención, LLM,
moneda/idioma, flujo de Git y autorizaciones docentes.
