# Wireframe borrador: formulario e informe de MarketIA

**Corte: 22 de octubre de 2026** · Apoya las preguntas 13, 14 y 22 · Funciones RF-01 a RF-05

> **Borrador para revisar.** Se armó a partir de los campos y reglas de
> [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md).
> Cristián debe revisarlo, corregirlo y, si está de acuerdo, firmarlo como
> suyo en la sección 6 (y reemplazarlo por un dibujo en Figma, Canva o papel si
> prefiere). Los campos y los textos de ejemplo son propuestas, no resultados.
> Diseño pensado para pantallas desde 360 px de ancho (RNF-04).
> El reporte de aprobación documental del equipo está en
> [`../actas/reporte-aprobacion-documental.md`](../actas/reporte-aprobacion-documental.md);
> no sustituye la revisión individual del diseño. Se ajusta este borrador para
> no solicitar nombres identificables de negocios o personas.

## 1. Flujo

```text
[Formulario] --enviar--> [Validación] --ok--> [Calculando...] --> [Informe]
                              |                                      |
                              +-- error: muestra qué campo corregir  +-- Imprimir / Guardar como PDF (navegador)
```

## 2. Pantalla 1: formulario de idea de negocio (RF-01)

```text
+--------------------------------------------------+
|  MarketIA                                         |
|  Analiza tu idea de negocio en Cochabamba         |
+--------------------------------------------------+
|  ⓘ No escribas tu nombre, correo, teléfono ni    |
|    cédula. Tu descripción se enviará a un        |
|    servicio de IA externo para generar el FODA.  |
|                                                   |
|  Alias de la idea (opcional; no usar nombre real) |
|  [______________________________]                 |
|                                                   |
|  Rubro *                                          |
|  [ Comercio v ]   (Comercio / Servicios)          |
|                                                   |
|  Describe tu idea * (50 a 1000 caracteres)        |
|  [                                         ]      |
|  [                                         ]      |
|  [__________________________________]  0 / 1000   |
|                                                   |
|  Zona de Cochabamba *                             |
|  [ Seleccionar zona v ]                           |
|                                                   |
|  Precio de venta por unidad (Bs) *                |
|  [________]                                       |
|  Costo variable por unidad (Bs) *                 |
|  [________]                                       |
|  Costos fijos mensuales (Bs) *                    |
|  [________]                                       |
|  Inversión inicial (Bs)   (opcional)              |
|  [________]                                       |
|                                                   |
|  Referencia de competidor (opcional, sin nombre)  |
|  Tipo / zona general       Precio (Bs)            |
|  [______________]        [______]    [+ agregar]  |
|                                                   |
|  [ ] Entiendo que mi descripción se envía a una   |
|      IA externa                                   |
|                                                   |
|           [   Generar informe   ]                 |
+--------------------------------------------------+
```

**Reglas de validación (de RF-01):**

| Campo | Regla | Mensaje de error propuesto |
|---|---|---|
| Rubro, zona | Obligatorios | "Completa este campo" |
| Alias de la idea | Opcional; usar un alias y no identificar personas o negocios | |
| Descripción | 50 a 1000 caracteres | "La descripción debe tener entre 50 y 1000 caracteres" |
| Precio, costo variable, costo fijo | Número mayor o igual a 0; no vacío; sin texto | "Escribe un número válido en Bs" |
| Zona | Debe ser de Cochabamba | "Por ahora solo analizamos negocios en Cochabamba" |
| Descripción con datos personales | Advertir y no enviar el dato | "Parece que escribiste un dato personal; quítalo para continuar" |
| Casilla de aviso | Obligatoria antes de enviar | "Debes aceptar el aviso para continuar" |

## 3. Pantalla 2: generando el informe

```text
+--------------------------------------------------+
|  Generando tu informe...                          |
|  [=========>               ]                      |
|  Calculando costos y punto de equilibrio  ✔       |
|  Preparando FODA y demanda con IA         ...     |
|  (Puede tardar hasta 5 minutos)                   |
+--------------------------------------------------+
```

## 4. Pantalla 3: informe (RF-02, RF-03, RF-04, RF-05)

Los cálculos y las estimaciones de IA aparecen en bloques separados y etiquetados (RNF-03).

```text
+--------------------------------------------------+
|  Informe: [Alias de la idea]                      |
|  Rubro · Zona · Fecha                             |
+--------------------------------------------------+
|  1. TUS DATOS                                     |
|  Precio: Bs __   Costo variable: Bs __            |
|  Costos fijos mensuales: Bs __  Inversión: Bs __  |
+--------------------------------------------------+
|  2. CÁLCULOS  [Resultado de fórmulas fijas]       |
|  Margen de contribución: Bs __ por unidad         |
|  Punto de equilibrio: __ unidades al mes          |
|  Punto de equilibrio: Bs __ al mes                |
|                                                   |
|  (si margen <= 0)                                 |
|  ⚠ Inviable con estos datos: el margen es cero    |
|    o negativo                                     |
+--------------------------------------------------+
|  3. COMPETENCIA QUE INGRESASTE                    |
| Referencia general         Precio (Bs)           |
|  ...            ...                               |
|  Promedio: Bs __   Rango: Bs __ a Bs __           |
|  (si no ingresó: "Sin datos")                     |
+--------------------------------------------------+
|  4. ESTIMACIÓN DE IA                              |
|  ⓘ Estimación generada por IA, no es un dato      |
|    verificado                                     |
|                                                   |
|  FODA                                             |
|  Fortalezas:   • __ • __   (mínimo 2)             |
|  Oportunidades:• __ • __                          |
|  Debilidades:  • __ • __                          |
|  Amenazas:     • __ • __                          |
|                                                   |
|  Demanda estimada: [ Baja | Media | Alta ]        |
|  Supuestos: • __ • __                             |
|                                                   |
|  (si la IA falla tras un reintento)               |
|  ⚠ FODA y demanda no están disponibles ahora.     |
|    Los cálculos de arriba siguen siendo válidos.  |
+--------------------------------------------------+
|  [ Imprimir / Guardar como PDF ]  [ Nuevo análisis ]|
+--------------------------------------------------+
```

## 5. Notas para el diseño

- Una sola columna en móvil (desde 360 px); botones de al menos 44 px de alto.
- Los avisos de privacidad y de "estimación de IA" no se pueden ocultar.
- No solicitar nombres de personas, nombres comerciales, ubicaciones exactas,
  teléfonos, correos ni otros identificadores; el alias es opcional.
- Si el formulario tiene errores, no se envía nada al servidor de IA.
- Probar en Chrome y Firefox, escritorio y móvil (RNF-06).
- Pregunta para los entrevistados al mostrar este flujo: "¿Esto te serviría? ¿Qué le falta?". Registrar la respuesta en la ficha de entrevista.

## 6. Revisión del autor (pendiente; completar Cristián solo si la realiza)

| Campo | Dato |
|---|---|
| Revisor previsto | Cristián García Bustamante |
| Fecha | |
| Cambios hechos al borrador | |
| ¿Se reemplaza por un dibujo propio (Figma, Canva, papel)? Enlace o archivo | |
| ¿Se confirma que representa la intención del equipo? | Sí ( ) No ( ) |

Firma (nombre y fecha, si se realiza): ______________________
