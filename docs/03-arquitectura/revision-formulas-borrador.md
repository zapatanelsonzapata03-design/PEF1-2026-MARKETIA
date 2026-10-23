# Revisión de las fórmulas: borrador de comparación

**Corte: 22 de octubre de 2026** · Responde las preguntas 14 y 33 · Objetivo OE2

> **Este documento NO es la revisión independiente.** Es un recálculo previo,
> hecho con aritmética decimal exacta. Se volvió a calcular aquí cada ejemplo
> con las fórmulas descritas y los diez resultados coinciden con la tabla. Esto
> solo verifica la aritmética de los ejemplos: **no es la revisión
> independiente de Cristián, una prueba de software ni una validación con
> negocios reales**. Cristián debe recalcular los casos por su cuenta y
> completar la sección 4 si efectivamente los revisa. Mientras esa sección y
> la evidencia de revisión estén vacías, P33 sigue pendiente de evidencia.

## 1. Fórmulas

Para precio de venta unitario `P`, costo variable unitario `CVu` y costo fijo del periodo `CF`:

```latex
MC = P - CV_u \qquad PE_u = \left\lceil \frac{CF}{MC} \right\rceil \qquad PE_b = PE_u \times P
```

Si `MC ≤ 0` no se calcula el punto de equilibrio y se muestra: "Inviable con estos datos: el margen es cero o negativo".

## 2. Resultados del recálculo (borrador) frente a lo documentado

Origen de los datos de entrada y de la columna "Documentado": [`datos-seguridad-pruebas.md`](../03-arquitectura/datos-seguridad-pruebas.md). Los casos son sintéticos, no de negocios reales.

| Caso | P | CVu | CF | MC | CF/MC | PEu | PEb | Documentado (MC, PEu, PEb) | ¿Coincide? |
|---:|---:|---:|---:|---:|---:|---:|---:|---|:-:|
| 1 | 20 | 12 | 2000 | 8 | 250,00 | 250 | 5000 | 8, 250, 5000 | Sí |
| 2 | 35 | 20 | 3500 | 15 | 233,33 | 234 | 8190 | 15, 234, 8190 | Sí |
| 3 | 10 | 10 | 1000 | 0 | n/a | error | error | Error "Inviable" | Sí |
| 4 | 12 | 5 | 1800 | 7 | 257,14 | 258 | 3096 | 7, 258, 3096 | Sí |
| 5 | 8 | 3,5 | 900 | 4,5 | 200,00 | 200 | 1600 | 4,5, 200, 1600 | Sí |
| 6 | 50 | 32,5 | 4200 | 17,5 | 240,00 | 240 | 12000 | 17,5, 240, 12000 | Sí |
| 7 | 15 | 18 | 1000 | −3 | n/a | error | error | Error "Inviable" | Sí |
| 8 | 25 | 10 | 0 | 15 | 0,00 | 0 | 0 | 15, 0, 0 | Sí |
| 9 | 7,5 | 4,2 | 1325 | 3,3 | 401,52 | 402 | 3015 | 3,3, 402, 3015 | Sí |
| 10 | 100 | 60 | 12000 | 40 | 300,00 | 300 | 30000 | 40, 300, 30000 | Sí |

**Comprobación aritmética de los ejemplos:** 10 de 10 resultados coinciden con
las fórmulas y entradas indicadas; no se observan diferencias monetarias en
esta reproducción decimal. Este resultado no debe anotarse como revisión
independiente ni como prueba ejecutada del sistema.

Observaciones para tener en cuenta al revisar:
- Caso 2, 4 y 9: el cociente `CF/MC` no es entero y el resultado depende de redondear **hacia arriba**. Un redondeo normal daría 233, 257 y 402 (el 9 coincide por casualidad), así que estos casos sí prueban la regla.
- Caso 8: costo fijo cero devuelve punto de equilibrio 0; confirmar que el equipo acepta mostrarlo así o prefiere una advertencia.
- Los casos 3 y 7 prueban `MC ≤ 0` (cero y negativo).
- Los resultados dependen de que `CF` y las unidades sean del mismo periodo (mensual). El informe debe mostrar el periodo.

## 3. Cómo recalcular de forma independiente (para Cristián)

En una hoja de cálculo, columnas A a C = `P`, `CVu`, `CF`:

| Celda | Fórmula en Excel o Google Sheets |
|---|---|
| D (MC) | `=A2-B2` |
| E (PEu) | `=SI(D2<=0;"Inviable";REDONDEAR.MAS(C2/D2;0))` (en inglés: `=IF(D2<=0,"Inviable",ROUNDUP(C2/D2,0))`) |
| F (PEb) | `=SI(D2<=0;"Inviable";E2*A2)` |

Tomar los valores de entrada solo de la tabla de la sección 2, sin mirar mis resultados, y recién después compararlos.

**Entradas inválidas que también deben probarse** (el sistema muestra error y no calcula): precio, costo variable o costo fijo negativos; campos vacíos; texto en lugar de número.

## 4. Revisión independiente (pendiente; completar Cristián solo si la realiza)

| Campo | Dato |
|---|---|
| Revisor previsto | Cristián García Bustamante |
| Fecha de la revisión | |
| Herramienta usada | |
| Casos que coinciden | ___ de 10 |
| Discrepancias encontradas y cómo se resolvieron | |
| ¿Se acepta el redondeo hacia arriba y el caso 8? | |
| Archivo de la hoja de cálculo guardado en | |

Firma (nombre y fecha, si se realiza): ______________________

## 5. Casos con negocios reales (pendiente)

La Meta 4 del informe pide comparar con 3 negocios reales de Cochabamba, anonimizados y con permiso del dueño. Tolerancia propuesta: diferencia relativa ≤ 10 % entre el punto de equilibrio calculado y el que registra el dueño.

| Caso real | Rubro | P | CVu | CF mensual | PEu calculado | PEu del dueño | Diferencia relativa | ¿Cumple ≤ 10 %? |
|---|---|---:|---:|---:|---:|---:|---:|:-:|
| R1 | | | | | | | | |
| R2 | | | | | | | | |
| R3 | | | | | | | | |
