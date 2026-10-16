# Alcance, MVP y requisitos

> Borrador de trabajo derivado de las funcionalidades del README. Los criterios
> marcados como propuesta requieren revisión del equipo y del docente antes de
> convertirse en compromisos de desarrollo.

## Usuarios y necesidades iniciales

El README identifica emprendedores y microempresarios, estudiantes, y asesores
o incubadoras como grupos de usuarios previstos. A partir de las funcionalidades
listadas, se infieren estas necesidades; aún no han sido confirmadas mediante
entrevistas:

- Describir una idea de negocio.
- Consultar información de competencia, precios y tendencias.
- Obtener una orientación FODA y de demanda.
- Comprender costos y punto de equilibrio.
- Consultar y compartir un informe.

Se debe priorizar un grupo de usuarios para el MVP y validar estas necesidades
con personas de ese grupo.

## Funcionalidades previstas y criterios de aceptación propuestos

| ID | Funcionalidad prevista | Criterio observable propuesto | Pendiente antes de desarrollar |
|---|---|---|---|
| RF-01 | Registrar la idea de negocio en un formulario. | La persona puede completar y enviar una idea; el sistema confirma si fue recibida o indica qué dato debe corregirse. | Definir campos, obligatoriedad, límites, validaciones y manejo de datos personales. |
| RF-02 | Investigar competencia, precios y tendencias. | El informe presenta resultados para el contexto de Cochabamba e identifica la fuente y fecha de cada dato usado. | Definir fuentes permitidas, cobertura, actualización, permisos y qué hacer cuando no haya datos. |
| RF-03 | Generar análisis FODA y estimación de demanda con IA. | El informe muestra los cuatro componentes FODA y una sección de demanda que distingue datos, supuestos y contenido generado. | Definir método de estimación, evidencias, límites de confianza, revisión humana y comportamiento ante datos insuficientes. |
| RF-04 | Calcular costos y punto de equilibrio con fórmulas fijas. | Para un conjunto de entradas acordado, el sistema muestra los costos y el punto de equilibrio; los resultados coinciden con un cálculo de referencia revisado. | Definir variables, fórmulas, unidades, moneda, redondeo, entradas inválidas y casos de prueba de referencia. |
| RF-05 | Presentar el informe en pantalla y PDF. | El informe puede consultarse en pantalla y exportarse a PDF; ambos formatos muestran la misma información esencial. | Definir estructura, accesibilidad, idioma, edición, almacenamiento y datos que se incluirán en el PDF. |

Los criterios son propuestas para convertir la lista general en requisitos
comprobables; no afirman que esos comportamientos estén implementados.

## Requisitos de calidad iniciales

| ID | Requisito o pregunta de calidad | Estado |
|---|---|---|
| RNF-01 | Generar el informe en menos de cinco minutos, de acuerdo con el objetivo general del README. | Umbral existente; falta acordar las condiciones y el método de medición. |
| RNF-02 | Proteger la información ingresada por las personas usuarias. | Necesidad pendiente de requisitos de privacidad, permisos, retención y eliminación. |
| RNF-03 | Presentar cálculos reproducibles y distinguibles de las estimaciones generadas por IA. | Propuesta; faltan reglas de trazabilidad y casos de validación. |
| RNF-04 | Definir facilidad de uso, compatibilidad, disponibilidad y demás atributos relevantes. | Pendiente de priorización y criterios verificables. |

## MVP propuesto

Como punto de partida para discusión, se propone que el MVP permita registrar
una idea, generar un informe en pantalla con análisis FODA/demanda y cálculos
de costos/punto de equilibrio, y cumplir el objetivo de tiempo ya establecido.
El PDF y la investigación de mercado automatizada podrían evaluarse como
entregas posteriores si el equipo confirma que son prescindibles en la primera
versión.

Esta priorización no está aprobada por el equipo. En particular, deben confirmar
si un informe sin investigación automatizada de competencia, precios y
tendencias entrega valor suficiente.

## Alcance

### Incluido en la propuesta actual del README

- Formulario de la idea de negocio.
- Investigación de competencia, precios y tendencias.
- Análisis FODA y estimación de demanda con IA.
- Cálculo de costos y punto de equilibrio mediante fórmulas fijas.
- Informe en pantalla y PDF.

### Exclusiones por definir

El repositorio no define si se desarrollarán cuentas de usuario, pagos,
despliegue público, aplicación móvil, cobertura fuera de Cochabamba ni
integraciones distintas de las tecnologías enumeradas. No se deben tratar como
incluidos ni como excluidos definitivos hasta que el equipo los decida.

### Reducción de alcance del 40 %: propuesta para discusión

Si fuera necesario reducir el trabajo, se propone conservar el formulario, el
análisis FODA/demanda, los cálculos verificables y un informe básico en pantalla.
Se propone posponer la investigación automatizada de mercado y la exportación
PDF. Esta opción conserva una ruta para evaluar viabilidad, pero reduce la
cobertura de mercado; requiere aprobación del equipo y del docente.

## Decisiones que bloquean requisitos finales

- Grupo de usuarios prioritario y necesidades validadas.
- Campos y datos personales que recibirá el formulario.
- Fuentes de datos de mercado y permisos para utilizarlas.
- Método de demanda, fórmulas financieras y casos de referencia.
- Contenido mínimo del informe y alcance exacto del MVP.
- Umbrales de calidad adicionales al tiempo de respuesta.
- Reglas de privacidad, retención, seguridad y revisión humana.
