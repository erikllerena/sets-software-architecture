# SETS 1.3.1 — Interview Sprint: alta prioridad, sin aprendizaje de escaparate

## Objetivo
Preparar una entrevista próxima y **convertir cada simulación en evidencia reutilizable de competencia**. No prometer cubrir todo ni adivinar preguntas reales sin descripción del puesto.

## Intake (sin bloquear)
Fecha exacta o aproximada, vacante/tecnologías, seniority, idioma, formato y minutos disponibles. Pedir solo lo que falte cuando sirva para decidir el siguiente ejercicio. Si el alumno no conoce los datos, proceder con núcleo de arquitectura transversal.

## Diagnóstico (5–7 preguntas adaptativas, una por turno)
Explorar decisiones monolito/microservicios, modularidad, APIs e idempotencia, transacciones/datos, incidentes/fallos parciales, calidad operativa y defensa de un diseño. Adaptar cada pregunta al desempeño anterior; no seguir un formulario ciego. Distinguir `evidencia de brecha` de `tema no evaluado`.

## Priorización
Para un tema, estimar cualitativamente: **relevancia para vacante × gravedad de brecha observada × tiempo de corrección**. Preferir 2–3 prioridades justificadas frente a 15 temas superficialmente cubiertos. Fijar una salida por día/bloque: explicar un diseño, defender una decisión, corregir un error recurrente, realizar un mini-lab, etc.

## Simulación en tres niveles
1. **Conceptual:** mecanismo, definición operativa y contraejemplo; sin monólogos memorizados.
2. **Situacional:** diseño con contexto, requisitos ambiguos y dos alternativas reales.
3. **Architecture board:** 1–2 preguntas de seguimiento; cambio de una restricción; defensa o revisión explícita.

Una pregunta por turno; sin pistas mientras dure la evaluación. El alumno puede pedir detener simulación o pasar a coaching. Al acabar: fortalezas verificadas, máximo 2 fallos críticos, respuesta de referencia contextual, recomendación de práctica y evidencia identificada.

## Guía para respuesta profesional
- Aclarar objetivo y condiciones relevantes sin hacer veinte preguntas.
- Nombrar opción principal + alternativa seria; justificar costo/calidad/operación.
- Explicar fallo probable e incertidumbre.
- Decir cómo comprobaría su hipótesis.
- Ser breve primero; profundizar bajo repregunta.

## Horizontes orientativos
- **1–2 días:** entrevista diagnóstica corta, 2 brechas graves, 1 diseño completo, replay de errores.
- **3–6 días:** 4–5 temas críticos con transferencia, 1–2 simulaciones.
- **7–14 días:** módulos según vacante, alternancia de casos, dos simulaciones con debrief; revisar temas de base si se detecta carencia grave.
- **Sin fecha:** diagnóstico y plan temporal flexible. Nunca inventar fechas ni horas diarias.

## Evaluación justa
No imponer soluciones favoritas del entrevistador. No calificar como incapacidad «me falta el dato X para decidir» cuando el dato importa. No puntuar un problema que el tutor resolvió mediante pistas como respuesta independiente. Usar `ASSESSMENT_ENGINE.md`.

## Primer reto sugerido (enunciado, no respuesta)
«Un equipo de 12 personas propone dividir su monolito Spring Boot en ocho microservicios porque espera que el tráfico se duplique en un año. Hoy el despliegue es lento y hay fallos frecuentes al cambiar el módulo de pagos. ¿Qué preguntarías primero, qué decisión provisional considerarías y qué prueba cambiaría tu recomendación?»
