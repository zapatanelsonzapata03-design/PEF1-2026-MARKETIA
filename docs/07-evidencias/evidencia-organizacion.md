# Evidencia de organización del equipo

> Respalda la pregunta 42 (mecanismo para revisar e integrar el trabajo). Guardar
> las capturas en esta carpeta y anotar aquí su nombre. Mientras no existan,
> estos acuerdos siguen siendo propuestas.

## 1. Tablero de Trello

| Campo | Dato |
|---|---|
| Enlace del tablero (copiar también al README) | |
| Fecha de creación | |
| Columnas: pendiente, en curso, en revisión, terminada | ( ) creadas |
| Tarjetas creadas desde el plan (tareas A1 a A9 y B1 a B12) | ( ) sí |
| Cada tarjeta tiene responsable y fecha | ( ) sí |
| Captura | |

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
| Captura | |

## 3. Pull requests y ramas

| Campo | Dato |
|---|---|
| Pull request abierto al revisar el repositorio | Número ___ · Estado: ( ) fusionado ( ) cerrado ( ) sigue abierto |
| Convención de ramas acordada | `feat/<área>-<descripción>` y `docs/<descripción>` |
| Revisor de cada pull request | Una persona distinta a la autora |
| Revisión semanal de pull requests abiertos | Viernes, reunión de las 20:00 |

## 4. Reuniones

| Campo | Dato |
|---|---|
| Reuniones acordadas en el acta 01 | |
| Notas de 3 líneas al cierre de cada reunión (avance, bloqueo, siguiente paso) | ( ) se están guardando en el grupo |


# Registro de la prueba de viabilidad de OmniRoute

> Hacer esta prueba **solo con autorización escrita del docente** y fuera de
> `src/` (por ejemplo, en `spikes/omniroute/`). Usar ideas de ejemplo, sin datos
> personales ni de negocios reales, y sin subir claves ni archivos `.env`.
> Completar con mediciones reales; no estimar.

## 1. Datos generales

| Campo | Dato |
|---|---|
| Autorización del docente (fecha y medio) | |
| Fecha de la prueba | |
| Responsable | |
| Proveedor y modelo usados vía OmniRoute | |
| Versión de OmniRoute | |
| Condiciones (red, hora, plan gratuito o de pago) | |

## 2. Diez ideas de ejemplo

Criterios propuestos: al menos 9 de 10 respuestas con el formato JSON acordado
y mediana de latencia de 60 segundos o menos.

| N.º | Idea de ejemplo (resumen, sin datos reales) | ¿JSON válido? | Latencia (s) | ¿Reintento? | Costo (Bs o USD) | Observaciones |
|---:|---|:-:|---:|:-:|---:|---|
| 1 | | | | | | |
| 2 | | | | | | |
| 3 | | | | | | |
| 4 | | | | | | |
| 5 | | | | | | |
| 6 | | | | | | |
| 7 | | | | | | |
| 8 | | | | | | |
| 9 | | | | | | |
| 10 | | | | | | |

## 3. Resumen

| Indicador | Resultado | Criterio | ¿Cumple? |
|---|---|---|:-:|
| Respuestas con formato válido | ___ de 10 | 9 de 10 | |
| Mediana de latencia | ___ s | 60 s o menos | |
| Costo medio por informe | ___ | Comparar con OE5 | |
| Solicitudes fallidas y cómo se manejaron | | Documentar | |
| Términos y privacidad del proveedor revisados | Sí / No, fecha ___ | Antes de enviar datos reales | |

## 4. Repetición del caso de la cafetería (Anexo B del informe)

El ejemplo del informe (cafetería pequeña, inversión de Bs 20 000) no descontaba
costos variables ni personal. Repetirlo con costos completos y calcular el
punto de equilibrio con las **fórmulas fijas**, no con la IA.

| Dato | Valor |
|---|---|
| Precio de venta por unidad (Bs) | |
| Costo variable por unidad (Bs) | |
| Costos fijos mensuales (Bs) | |
| Punto de equilibrio en unidades (fórmula fija) | |
| Punto de equilibrio en Bs (fórmula fija) | |
| ¿La estimación de la IA es coherente con el cálculo? | |

 Decisión

- [ ] OmniRoute es viable para el piloto
- [ ] Activar el plan B de proveedor (indicar cuál: ____________)
- [ ] La prueba queda pendiente (motivo: ____________)

Pasar los resultados agregados a `docs/05-estadistica/resultados.md` y guardar
las capturas en esta carpeta, sin credenciales.

## 5. Cierre
Verificado por: __________ · Fecha: ____/10/2026
