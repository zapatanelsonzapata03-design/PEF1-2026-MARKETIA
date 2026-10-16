# Datos, seguridad y estrategia de pruebas

> Propuesta de diseño pendiente de ratificación, autorización y validación.
> No describe una implementación existente.

## Datos previstos y origen

| Dato | Origen propuesto | Persistencia propuesta |
|---|---|---|
| Idea y valores del negocio | Ingreso de la persona usuaria | Solo si se ratifica D6; sin identificadores personales directos. |
| Competidores conocidos y precios | Ingreso opcional de la persona usuaria para el MVP | Solo si se ratifica D3 y D6. |
| FODA y demanda | Generación del LLM a partir de la entrada | Dentro del informe, marcados como estimaciones. |
| Cálculos | Fórmulas fijas aplicadas a los valores ingresados | Dentro del informe. |

No hay entrevistas, entradas reales de negocio ni observaciones de prueba
registradas. Para pruebas con personas, usar consentimiento y minimizar los
datos; para ejemplos publicados, quitar información que pueda identificar a
una persona o negocio.

## Privacidad y controles propuestos

- No solicitar nombre de la persona, correo, teléfono ni cédula.
- Avisar antes de enviar la descripción y los valores al proveedor de LLM; la
  transferencia y el texto del consentimiento deben revisarse antes de integrar
  el proveedor.
- Definir acceso, retención y borrado antes de almacenar datos reales. D6
  propone 90 días y eliminación mediante identificador aleatorio; falta
  ratificarlo y validar su viabilidad.
- Limitar la recolección al mínimo necesario y no incluir datos personales en
  capturas, registros de prompts ni casos de prueba.
- No guardar secretos, claves ni contraseñas en Git, documentación, muestras o
  capturas. No se registran ni se leen credenciales en este proyecto.
- La limitación de solicitudes por IP y la validación de entradas son
  requisitos de seguridad propuestos; se deben definir y probar antes de una
  demostración accesible por red.

## Fórmulas financieras propuestas

Para un precio de venta unitario `P`, costo variable unitario `CVu` y costo
fijo del periodo `CF`:

- Margen de contribución unitario: `MC = P − CVu`.
- Punto de equilibrio en unidades: `PEu = ⌈CF / MC⌉`, redondeado hacia arriba.
- Punto de equilibrio en bolivianos: `PEb = PEu × P`.

Estas fórmulas requieren revisión del equipo y del docente, incluidas las
unidades y el periodo de los costos. Si `P ≤ CVu`, el margen no es positivo y
no se calcula el punto de equilibrio; el mensaje propuesto es: “Inviable con
estos datos: el margen es cero o negativo”.

### Diez casos de referencia (sintéticos)

Los casos siguientes son **aritméticos y sintéticos**: sirven para probar las
fórmulas y los límites. **No son datos de negocios reales.** Se calcularon con
aritmética decimal exacta (`PEu` redondeado hacia arriba, `PEb = PEu × P`).
Hay que revisarlos de forma independiente (tarea A5: Cristián revisa los
cálculos de Nelson) y completar **3 casos con negocios reales de Cochabamba**,
con autorización y datos anonimizados, para la comparación de la Meta 4 del
informe.

| Caso | P (Bs/u) | CVu (Bs/u) | CF (Bs/periodo) | Resultado esperado | Qué prueba |
|---|---:|---:|---:|---|---|
| 1 | 20 | 12 | 2000 | MC = 8; PEu = 250; PEb = 5000 | División exacta |
| 2 | 35 | 20 | 3500 | MC = 15; CF/MC = 233,33; PEu = 234; PEb = 8190 | Redondeo hacia arriba |
| 3 | 10 | 10 | 1000 | MC = 0; error "Inviable con estos datos" | Margen cero |
| 4 | 12 | 5 | 1800 | MC = 7; CF/MC = 257,14; PEu = 258; PEb = 3096 | Redondeo hacia arriba |
| 5 | 8 | 3,5 | 900 | MC = 4,5; PEu = 200; PEb = 1600 | Decimales con división exacta |
| 6 | 50 | 32,5 | 4200 | MC = 17,5; PEu = 240; PEb = 12000 | Decimales con división exacta |
| 7 | 15 | 18 | 1000 | MC = −3; error "Inviable con estos datos" | Margen negativo |
| 8 | 25 | 10 | 0 | MC = 15; PEu = 0; PEb = 0 | Costo fijo cero |
| 9 | 7,5 | 4,2 | 1325 | MC = 3,3; CF/MC = 401,52; PEu = 402; PEb = 3015 | Decimales con redondeo |
| 10 | 100 | 60 | 12000 | MC = 40; PEu = 300; PEb = 30000 | Valores grandes |

Casos de entrada inválida que también deben probarse (el sistema responde con
un mensaje de error y no calcula): precio, costo variable o costo fijo
negativos; campos vacíos; texto en lugar de número.

## Estrategia de pruebas propuesta

1. **Unitarias:** probar las fórmulas con los diez casos de referencia, los
   límites y las entradas inválidas.
2. **Contrato del LLM:** validar la salida contra un esquema definido; simular
   respuestas mal formadas, errores y reintentos.
3. **Integración:** verificar el flujo formulario → API → informe y los estados
   de error.
4. **Usuarios:** observar las tareas de usabilidad de OE4 con cinco
   emprendedores, sujeto a aprobación del protocolo.
5. **Rendimiento:** registrar veinte ejecuciones para OE1, incluyendo fallos
   según una regla de contabilización acordada.
6. **Registro:** conservar fecha, versión, datos de prueba no sensibles,
   resultado observado y decisión. Publicar resultados en
   `docs/05-estadistica/resultados.md` cuando existan mediciones.

No hay pruebas ejecutadas ni resultados que reportar. La implementación y las
pruebas con servicios externos requieren las autorizaciones registradas en
`docs/09-preparacion.md`; `src/` debe permanecer sin código hasta autorización
docente.
