# Respuestas al cuestionario de aprobación

**Equipo MarketIA · corte: 23 de octubre de 2026**

> Cada respuesta resume lo que ya existe en este repositorio y enlaza su
> fuente. El campo **Estado** es honesto: "Documentado" significa que hay un
> documento que responde la pregunta; "Pendiente de evidencia" significa que
> falta un dato real (entrevistas, cotizaciones, pruebas, acta o respuesta del
> docente). **Ninguna pregunta se marca "Cumple" hasta que su evidencia esté
> subida.** La matriz con fechas está en
> [`cuestionario-aprobacion.md`](cuestionario-aprobacion.md).
>
> La coordinación reportó que los integrantes aprobaron el paquete documental
> recibido el 22/10/2026. El repositorio no incluye confirmaciones individuales,
> fechas o firmas de cada integrante; por ello el reporte se registra como
> declaración de coordinación, no como aprobaciones individuales de GitHub ni
> ratificación del acta. Ver
> [`reporte-aprobacion-documental.md`](../actas/reporte-aprobacion-documental.md).

Rutas relativas a `docs/06-auditoria/`.

---

## 1. Problema y valor

**1. ¿Pueden explicar el problema en menos de 30 segundos sin tecnología?**
Sí: "Mucha gente en Cochabamba abre un negocio sin saber si le va a dar ganancia. Un estudio de viabilidad profesional puede ser caro y demorar días, así que decide sin un análisis claro. Necesita saber cuánto debe vender para cubrir sus costos y qué riesgos revisar."
Fuente: [`resumen-del-problema.md`](../01-proyecto/resumen-del-problema.md). **Estado:** Documentado; falta ensayo con cronómetro.

**2. ¿Quién tiene el problema y quién usará la solución?**
Emprendedor o microempresario de Cochabamba que planifica un negocio de comercio o servicios simples (decisión D1). Usuarios secundarios para versiones futuras: asesores, incubadoras y estudiantes.
Fuente: [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md). **Estado:** Documentado; D1 falta ratificar en el acta.

**3. ¿Qué evidencia demuestra que el problema es real, relevante o necesario?**
El repositorio contiene ocho resúmenes de entrevistas reportados (E01–E08), con tres respuestas clave por entrevista, no fichas completas de las 24 preguntas. No constan fichas originales ni evidencia de consentimiento o autorización; no se presentan como una muestra completa verificada. Dos capturas del 22/10 muestran consultas enviadas, pero no respuestas, precios ni plazos, ni acreditan dos proveedores distintos. Nelson reportó que los nueve enlaces de referencia abren y que contrastó las afirmaciones; quedan correcciones o delimitaciones por aplicar y una revisión por otra persona sigue pendiente.
Fuente: [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md), [`guion-cotizaciones.md`](../07-evidencias/guion-cotizaciones.md), [`referencias.md`](../01-proyecto/referencias.md), [`verificacion-referencias.md`](verificacion-referencias.md). **Estado:** Entrevistas y referencias con evidencia preliminar; validación y correcciones pendientes.

**4. ¿Qué consecuencias tiene actualmente ese problema?**
Los ocho resúmenes aportados describen dificultades relacionadas con competencia, planificación, costos y herramientas básicas. Son evidencia cualitativa preliminar; faltan fichas completas y consentimiento para valorar el procedimiento y no permiten generalizar a toda la población.
Fuente: [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md), [`resumen-del-problema.md`](../01-proyecto/resumen-del-problema.md). **Estado:** Indicios preliminares; validación pendiente.

**5. ¿Qué valor concreto aportará la solución al usuario?**
Un informe en menos de 5 minutos con punto de equilibrio calculado, FODA y estimación de demanda con supuestos visibles, en español y bolivianos. El costo por informe y la disposición de pago se medirán (OE5).
Fuente: [`objetivos.md`](../02-requisitos/objetivos.md). **Estado:** Documentado; falta medir.

**6. ¿Por qué la solución es una respuesta adecuada y no solo una aplicación interesante?**
El diseño propone responder "¿cuánto debo vender para cubrir mis costos y qué riesgos revisar?" mediante fórmulas fijas y estimaciones de IA etiquetadas. Los ocho resúmenes expresan interés en claridad, rapidez o facilidad, pero la documentación es parcial y no demuestra todavía la adecuación de la solución. Las consultas de precio no tienen respuesta y las cifras de referencias no están verificadas.
Fuente: [`resumen-del-problema.md`](../01-proyecto/resumen-del-problema.md), [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md). **Estado:** Diseño documentado; validación pendiente.

## 2. Objetivos y éxito

**7. ¿El objetivo general describe un resultado concreto que puede comprobarse?**
Sí: generar para un negocio en Cochabamba un informe con FODA, demanda, costos y punto de equilibrio en menos de 5 minutos y a costo accesible.
Fuente: [`README`](../../README.md), [`objetivos.md`](../02-requisitos/objetivos.md). **Estado:** Documentado; falta ratificar D12.

**8. ¿Los objetivos específicos permiten dividir y comprobar el avance?**
Sí: OE1 (18 de 20 ejecuciones en ≤ 5 min), OE2 (10 casos, ±0,01 Bs), OE3 (rúbrica ≥ 3,5/5 con 3 evaluadores y 10 ideas), OE4 (4 de 5 usuarios sin ayuda, satisfacción ≥ 4/5), OE5 (costo por informe a medir) y OE6 (reducir 70 % el tiempo).
Fuente: [`objetivos.md`](../02-requisitos/objetivos.md). **Estado:** Documentado; falta ratificar umbrales.

**9. ¿Hay relación clara entre problema, objetivos, solución y resultados?**
Sí, en la tabla de trazabilidad de `objetivos.md`: decidir sin conocer el punto de equilibrio → OE2 y OE3 → cálculos y FODA con supuestos; costo y tiempo del análisis → OE1 y OE5; contexto local → OE3 y OE4.
Fuente: [`objetivos.md`](../02-requisitos/objetivos.md). **Estado:** Documentado.

**10. ¿Cómo sabrán al final que tuvieron éxito?**
Cuando OE1 a OE6 cumplan sus umbrales con evidencia registrada en `docs/05-estadistica/resultados.md` (hoy plantilla vacía), con tamaño de muestra, proporción e intervalo de confianza del 95 %.
Fuente: [`plan-validacion.md`](../05-estadistica/plan-validacion.md). **Estado:** Documentado; OE5 y demás pendientes de medir.

## 3. Usuarios y requisitos

**11. ¿Usuarios y necesidades suficientemente definidos?**
Cuatro necesidades propuestas: saber cuánto vender para cubrir costos, entender riesgos y oportunidades, describir la idea sin conocimientos técnicos y obtener un informe para evaluar el negocio. Ocho resúmenes aportados mencionan algunas necesidades afines; faltan fichas completas y consentimiento documentado.
Fuente: [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md), [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md). **Estado:** Documentado con indicios cualitativos preliminares; validación pendiente.

**12. ¿Funcionalidades ligadas a necesidades reales?**
Cada necesidad propuesta se vincula a un requisito RF-01 a RF-05; los ocho resúmenes aportados son indicios, no una validación suficiente de esa correspondencia.
Fuente: [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md), [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md). **Estado:** Documentado como hipótesis; validar con fichas completas.

**13. ¿Funcionalidades descritas para que otro integrante las desarrolle sin adivinar?**
RF-01 lista campos, rangos (descripción de 50 a 1000 caracteres) y reglas de error; RF-02 a RF-05 describen entradas, salidas y mensajes (por ejemplo "Inviable con estos datos: el margen es cero o negativo"). El [wireframe borrador](../03-arquitectura/wireframe-borrador.md) complementa la especificación y sigue pendiente de revisión por Cristián. **Estado:** Documentado como borrador.

**14. ¿Cada funcionalidad tiene criterios de aceptación verificables?**
Sí, en formato dado/cuando/entonces para RF-01 a RF-05 (por ejemplo, resultados dentro de ±0,01 Bs frente al caso de referencia revisado).
Fuente: ídem. **Estado:** Documentado; falta convertirlos en casos de prueba (A6).

**15. ¿Existen requisitos de calidad?**
Sí: RNF-01 rendimiento (90 % de 20 ejecuciones en ≤ 5 min), RNF-02 privacidad, RNF-03 transparencia, RNF-04 usabilidad (4 de 5; ≥ 4/5), RNF-05 seguridad, RNF-06 compatibilidad (Chrome y Firefox), RNF-07 disponibilidad (demostración, sin 24/7).
Fuente: ídem. **Estado:** Documentado; falta ratificar umbrales.

## 4. Alcance

**16. ¿Está definido qué desarrollará el equipo?**
Formulario, cálculos fijos de costos y punto de equilibrio, FODA y demanda con IA etiquetados, informe en pantalla imprimible desde el navegador, pruebas y documentación.
Fuente: [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md). **Estado:** Documentado; falta ratificar D2.

**17. ¿Está definido qué NO desarrollará?**
Cuentas e inicio de sesión, pagos, app móvil nativa, otras ciudades, PDF propio (v1.1), búsqueda automática de competencia (v2), versión para asesores e historial (v2), panel administrativo y otros idiomas.
Fuente: ídem y [`decisiones.md`](../decisiones.md) (D5). **Estado:** Documentado; falta ratificar D5.

**18. ¿Identificaron funcionalidades interesantes pero innecesarias?**
Sí: chat con asesor IA, comparación de varias ideas, gráficos animados, proyección a cinco años, integración con redes sociales y ranking de negocios.
Fuente: ídem. **Estado:** Documentado.

**19. ¿El alcance es realista según tiempo, conocimientos y recursos?**
Estimación: 112 h de trabajo en la fase B frente a 138 h disponibles si cada integrante da 8 h semanales (margen ≈ 23 %). Las horas son una propuesta; cada integrante debe confirmarlas en el acta. Cristián queda ajustado (44 h para 46 h de capacidad individual).
Fuente: [`plan-desarrollo-y-riesgos.md`](../04-planificacion/plan-desarrollo-y-riesgos.md), [`roles-y-acuerdos.md`](../../equipo/roles-y-acuerdos.md). **Estado:** Documentado; falta confirmar disponibilidad.

**20. Si redujeran el proyecto 40 %, ¿qué conservarían y qué eliminarían?**
Conservar: formulario, cálculos fijos con su validación, informe en pantalla y FODA/demanda con IA en versión simple. Eliminar o posponer: PostgreSQL (informe solo en pantalla), competidores ingresados, impresión como PDF y pruebas de usabilidad ampliadas (reducidas a 3 usuarios).
Fuente: [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md). **Estado:** Documentado; falta ratificar.

## 5. MVP

**21. ¿Existe una primera versión funcional claramente definida?**
MVP v1.0: formulario → cálculos fijos → FODA y demanda con IA etiquetados y con supuestos visibles → informe en pantalla.
Fuente: ídem. **Estado:** Documentado; falta ratificar D2.

**22. ¿El MVP resuelve una parte real del problema y entrega valor?**
El MVP se diseñó para responder cuánto vender para cubrir costos y qué riesgos revisar. Los resúmenes aportados expresan interés en algunas funciones, pero no se documenta que los participantes hayan visto o evaluado el wireframe; el valor sigue sin validarse.
Fuente: [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md), [`wireframe-borrador.md`](../03-arquitectura/wireframe-borrador.md), [`registro-entrevistas.md`](../07-evidencias/registro-entrevistas.md). **Estado:** Diseño documentado; validación con usuarios pendiente.

**23. ¿Puede estar terminado dentro del tiempo disponible?**
Plan en tres hitos: 40 % el 24/10, 80 % el 24/11 y 100 % el 19/12, con cuatro sprints de dos semanas. Depende de la autorización docente para iniciar el desarrollo.
Fuente: [`plan-desarrollo-y-riesgos.md`](../04-planificacion/plan-desarrollo-y-riesgos.md). **Estado:** Documentado; falta confirmar calendario y autorización.

**24. ¿Las funcionalidades posteriores están separadas del MVP?**
Sí: v1.1 (PDF propio) y v2 (búsqueda automática de competencia, asesores, historial).
Fuente: ídem. **Estado:** Documentado; falta ratificar.

## 6. Diseño y viabilidad técnica

**25. ¿La solución es técnicamente viable con las tecnologías y recursos del equipo?**
La arquitectura (Python + FastAPI, React, PostgreSQL, LLM vía OmniRoute) se propone como candidata. No hay evidencia de experiencia ni de pruebas del equipo con ellas; se confirmará con la prueba de viabilidad.
Fuente: [`arquitectura-inicial.md`](../03-arquitectura/arquitectura-inicial.md). **Estado:** Pendiente de evidencia.

**26. ¿Identificaron las partes más difíciles o inciertas?**
Sí: (1) calidad y formato de la salida del LLM, (2) cumplir 5 minutos y conocer el costo por informe, (3) estimar demanda sin datos independientes, (4) qué datos se guardan y cómo se informa al usuario, (5) cálculos reproducibles con unidades inequívocas.
Fuente: ídem. **Estado:** Documentado.

**27. ¿Validaron o prevén validar las tecnologías críticas antes de depender de ellas?**
Está previsto: prueba con 10 ideas (≥ 9 con JSON válido, mediana ≤ 60 s, costo por análisis), fuera de `src/` y sin datos reales. No se ha ejecutado: requiere autorización docente. El Anexo B del informe contiene un solo caso, que no reemplaza la prueba.
Fuente: [`registro-prueba-viabilidad.md`](../07-evidencias/registro-prueba-viabilidad.md). **Estado:** Pendiente de evidencia y autorización.

**28. ¿Las decisiones tecnológicas tienen justificación relacionada con el proyecto?**
Sí, cada tecnología tiene una necesidad y una alternativa en la tabla de arquitectura (por ejemplo, SQLite como alternativa a PostgreSQL). La justificación se confirmará con costos reales.
Fuente: ídem. **Estado:** Documentado.

**29. ¿Identificaron las dependencias externas?**
Se identificaron como dependencias candidatas el proveedor de LLM, hosting, base de datos (si se ratifica D6), librerías y acceso al repositorio. El registro de accesos y hosting está creado como plantilla sin completar; los servicios, cuentas y costos no constan como verificados.
Fuente: [`09-accesos-y-hosting.md`](../09-accesos-y-hosting.md), [`09-preparacion.md`](../09-preparacion.md). **Estado:** Dependencias documentadas; recursos por confirmar.

**30. ¿Hay estructura técnica inicial para comenzar?**
Sí: flujo formulario → API → validación → cálculos y LLM → informe, contrato inicial (`POST /analisis`, `GET /health`) y árbol propuesto `backend/` y `frontend/`. Hay dos contratos alternativos en la sección 6; el equipo debe elegir uno.
Fuente: [`arquitectura-inicial.md`](../03-arquitectura/arquitectura-inicial.md). **Estado:** Documentado; falta ratificar un único contrato.

## 7. Datos, seguridad y calidad

**31. ¿Qué información manejará el sistema y de dónde proviene?**
Descripción y valores del negocio ingresados por el usuario, competidores y precios opcionales, FODA y demanda generados por el LLM, y cálculos de fórmulas fijas. No se piden nombre, correo, teléfono ni cédula.
Fuente: [`datos-seguridad-pruebas.md`](../03-arquitectura/datos-seguridad-pruebas.md). **Estado:** Documentado.

**32. ¿Identificaron restricciones de datos, privacidad, seguridad y acceso?**
Sí: aviso antes de enviar datos al proveedor de IA, retención de 90 días con borrado por id aleatorio (D6), validación de entradas, límite de solicitudes por IP, sin secretos en Git (`.env` ignorado).
Fuente: ídem. **Estado:** Documentado; falta ratificar D6.

**33. ¿Cómo comprobarán que las funciones principales funcionan?**
Se documentaron diez casos sintéticos. Una reproducción aritmética decimal de sus entradas coincide con los diez resultados de la tabla; esto no es la revisión independiente de Cristián, no prueba software y no incluye negocios reales. La sección para su revisión está en blanco.
Fuente: [`datos-seguridad-pruebas.md`](../03-arquitectura/datos-seguridad-pruebas.md), [`revision-formulas-borrador.md`](../03-arquitectura/revision-formulas-borrador.md). **Estado:** Comprobación aritmética preliminar; revisión independiente y validación real pendientes.

**34. ¿Hay estrategia inicial de pruebas?**
Sí: unitarias (fórmulas), contrato del LLM (esquema y respuestas mal formadas), integración, usabilidad con 5 emprendedores, rendimiento con 20 ejecuciones y registro de resultados.
Fuente: ídem. **Estado:** Documentado; no hay pruebas ejecutadas.

## 8. Plan de desarrollo

**35. ¿El Gantt tiene tareas concretas?**
Sí: fase A (A1 a A9) y fase B (B1 a B12), con diagramas Gantt por fase.
Fuente: [`plan-desarrollo-y-riesgos.md`](../04-planificacion/plan-desarrollo-y-riesgos.md). **Estado:** Documentado; fechas de fase A vencidas, deben reprogramarse.

**36. ¿Cada tarea tiene responsable?**
El plan asigna responsables por tarea (por ejemplo B2 Nelson, B4 Cristián, B9 Alex). La captura de Trello muestra algunas tarjetas, pero no permite comprobar que todas las tareas del plan estén reflejadas ni que cada tarjeta tenga responsable y fecha.
Fuente: [`plan-desarrollo-y-riesgos.md`](../04-planificacion/plan-desarrollo-y-riesgos.md), [`evidencia-organizacion.md`](../07-evidencias/evidencia-organizacion.md). **Estado:** Asignaciones documentadas; verificación completa del tablero pendiente.

**37. ¿Las tareas tienen estimaciones razonables?**
Sí, en horas por tarea: 49 h en la fase A y 112 h en la fase B.
Fuente: ídem. **Estado:** Documentado; falta confirmar.

**38. ¿Las dependencias están identificadas?**
Sí, en la columna "Depende de" del plan (por ejemplo B3 depende de A4 y B1). La captura no muestra dependencias entre tarjetas de Trello.
Fuente: [`plan-desarrollo-y-riesgos.md`](../04-planificacion/plan-desarrollo-y-riesgos.md), [`evidencia-organizacion.md`](../07-evidencias/evidencia-organizacion.md). **Estado:** Documentado en el plan; reflejo en Trello pendiente de comprobar.

**39. ¿El Gantt contempla desarrollo, integración, pruebas, correcciones y documentación?**
Sí: B1 a B6 desarrollo, B7 integración, B8 y B10 pruebas y mediciones, B12 correcciones, B9 documentación e informe final.
Fuente: ídem. **Estado:** Documentado.

**40. ¿Identificaron las tareas que podrían bloquear al equipo?**
Sí: A1 y la autorización docente, A4 (prueba de OmniRoute), B1 (contrato de API), B7 (integración) y A3 (entrevistas), cada una con su respuesta.
Fuente: ídem, sección 4. **Estado:** Documentado.

## 9. Equipo y riesgos

**41. ¿Cada integrante tiene responsabilidad concreta y verificable?**
Alex: actas, calendario, referencias, informe y evidencias. Nelson: motor de cálculos, API e integración con IA. Cristián: formulario, pantalla de informe, pruebas de usabilidad y guías.
Fuente: [`roles-y-acuerdos.md`](../../equipo/roles-y-acuerdos.md). **Estado:** Documentado; falta ratificar en el acta.

**42. ¿Hay mecanismo acordado para revisar e integrar el trabajo?**
Se proponen ramas por tarea, pull request con aprobación de otra persona, `main` protegida y revisión semanal los viernes. Una captura de ajustes muestra el requisito de PR y una aprobación, pero no el patrón de rama ni que la regla se aplique a `main`; otra captura muestra un listado de PR fusionadas, no revisiones individuales. La captura de Trello muestra listas y tarjetas, no que el flujo se aplique.
La coordinación reporta que los integrantes aprobaron el paquete documental usando una cuenta; el repositorio no registra aprobaciones individuales de GitHub.
Fuente: [`roles-y-acuerdos.md`](../../equipo/roles-y-acuerdos.md), [`reporte-aprobacion-documental.md`](../actas/reporte-aprobacion-documental.md), [`evidencia-organizacion.md`](../07-evidencias/evidencia-organizacion.md). **Estado:** Capturas parciales; aplicación de la regla a `main` y revisiones individuales pendientes de comprobar.

**43. ¿Cuáles son los tres riesgos que más podrían hacer fracasar o retrasar el proyecto?**
R1: poco tiempo del equipo y alcance mayor al tiempo. R2: la IA se equivoca, inventa datos o responde con formato inválido. R3: poca gente quiere pagar o no se valida la necesidad.
Fuente: [`plan-desarrollo-y-riesgos.md`](../04-planificacion/plan-desarrollo-y-riesgos.md). **Estado:** Documentado.

**44. ¿Cada uno tiene estrategia de mitigación?**
R1: MVP acotado, revisión del Gantt los lunes, recorte del 40 %. R2: fórmulas fijas, validación de esquema, etiquetas de estimación, comparación con casos reales. R3: entrevistas, nivel gratuito, alianzas. Cada riesgo tiene señal, plan B y responsable.
Fuente: ídem. **Estado:** Documentado.

**45. ¿Qué harían si una persona clave deja de estar disponible?**
Falta Nelson: Cristián sigue con el contrato y las pruebas, y se aplica el recorte. Falta Cristián: Nelson hace una interfaz mínima y Alex asume las pruebas con usuarios. Falta Alex: Cristián asume actas y evidencias, y Nelson el calendario.
Fuente: [`roles-y-acuerdos.md`](../../equipo/roles-y-acuerdos.md). **Estado:** Documentado; falta ratificar.

## 10. Preparación para desarrollar

**46. ¿Hay alguna decisión fundamental sin tomar que bloquee el inicio?**
Sí: las decisiones D1 a D16 siguen como propuestas porque el acta 01 no está completada; D16 se añadió como propuesta y tampoco está ratificada. El registro docente muestra el envío del enlace, pero no una respuesta escrita que autorice desarrollo. También falta confirmar la materia (D15). El equipo reportó su aprobación del paquete documental; eso no completa el acta ni sustituye autorización docente.
Fuente: [`decisiones.md`](../decisiones.md), [`acta-01-ratificacion.md`](../actas/acta-01-ratificacion.md), [`solicitud-autorizacion-docente.md`](../07-evidencias/solicitud-autorizacion-docente.md), [`reporte-aprobacion-documental.md`](../actas/reporte-aprobacion-documental.md). **Estado:** Pendiente.

**47. ¿Hay algún requisito importante que todavía no comprendan?**
Sí: el método para estimar la demanda (niveles bajo, medio, alto) aún no tiene rúbrica ni supuestos ratificados. Se mitiga mostrando los supuestos y probándolo con 10 ideas en la tarea A4.
Fuente: [`alcance-mvp-y-requisitos.md`](../02-requisitos/alcance-mvp-y-requisitos.md). **Estado:** Documentado; pendiente de rúbrica.

**48. ¿Falta alguna dependencia, permiso, acceso o recurso necesario para comenzar?**
El repositorio no documenta autorización docente, hosting, cuentas ni acceso confirmado a OmniRoute; las capturas muestran un tablero y ajustes de rama con requisitos de PR/aprobación, pero no permiten confirmar que la regla esté activa para `main`.
Fuente: [`09-preparacion.md`](../09-preparacion.md), [`09-accesos-y-hosting.md`](../09-accesos-y-hosting.md), [`evidencia-organizacion.md`](../07-evidencias/evidencia-organizacion.md). **Estado:** Pendiente de verificar el alcance de la regla y los demás recursos.

**49. Si mañana tuvieran que programar, ¿cada integrante sabría qué construir primero?**
Sí, tras la autorización: Nelson, esqueleto de la API y motor de cálculos (B1, B2); Cristián, formulario (B4); Alex, coordinación, informe y evidencias.
Fuente: [`09-preparacion.md`](../09-preparacion.md). **Estado:** Documentado; falta ratificar.

**50. Si un nuevo integrante solo revisara el repositorio, ¿podría entender qué hacer?**
El README resume problema, MVP, equipo, hitos y orden de lectura. Falta comprobarlo con una persona ajena al equipo.
Fuente: [`README`](../../README.md). **Estado:** Pendiente de evidencia.

## 11. Prueba de fracaso

**51. ¿Qué tendría que ser cierto para que el proyecto fracase?**
Que la IA produzca contenido inválido o lento, que el alcance exceda el tiempo, que nadie valide la necesidad ni el precio, que los cálculos sean incorrectos, que se confundan estimaciones con hechos, que se agoten las cuotas gratuitas de IA, que el equipo se desorganice, que se exponga información o un secreto, que el docente no autorice a tiempo y que poca gente quiera pagar.
Fuente: [`prueba-de-fracaso.md`](prueba-de-fracaso.md). **Estado:** Documentado.

**52. ¿Tienen estrategia para evitar o controlar cada condición?**
Sí, las condiciones, controles propuestos, responsables y estados se detallan en [`prueba-de-fracaso-tabla.md`](prueba-de-fracaso-tabla.md). Los controles siguen siendo en gran medida propuestas y dependen de evidencias, permisos y validación.
Fuente: ídem. **Estado:** Documentado; controles sin comprobar.

---

## Resumen de estados

- **Documentado:** preguntas 1, 2, 4, 5, 7 a 10, 13 a 21, 23, 24, 26, 28 a 32, 34 a 41, 43 a 45, 47, 49, 51 y 52.
- **Pendiente de evidencia:** preguntas 3, 6, 11, 12, 22, 25, 27, 33, 42, 46, 48 y 50.
- **"Cumple":** ninguna hasta subir la evidencia correspondiente.
