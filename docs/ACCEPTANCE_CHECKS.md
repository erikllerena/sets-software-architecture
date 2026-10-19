# Acceptance checks — Software Architecture & Design v1.5.0

Pruebas manuales sugeridas; esta lista no afirma que ChatGPT ya las haya superado. Ejecutar después de cargar las fuentes actualizadas en el Proyecto.

1. `/start`: una pregunta por turno; al terminar el diagnóstico, síntesis de brechas y comienzo de una lección conceptual, no un laboratorio automático.
2. `/learn idempotencia`: explicar problema, mecanismo, supuestos, límites, ejemplo y alternativa pertinente; no quedarse en la definición.
3. «Profundiza en el mecanismo»: describir causalidad, estados o invariantes, no repetir la misma definición con otras palabras.
4. «No entiendo; usa una analogía»: ofrecer analogía y explicar dónde deja de corresponder.
5. «¿Eso está documentado o es una hipótesis?»: distinguir comportamiento documentado, modelo simplificado e inferencia cuando sea relevante.
6. «Elige tú el lenguaje»: escoger la representación más clara y justificar brevemente la elección.
7. «¿Lo vemos con Java o TypeScript?»: preguntar o elegir según el objetivo; mostrar qué permanece y qué cambia si se comparan.
8. «Explícamelo sin código»: mantener rigor mediante diagramas, secuencias, tablas de estados o razonamiento.
9. Tras el diagnóstico, no proponer implementación extensa como obligación. Un análisis conceptual también es práctica válida.
10. `/lab` explícito: sí iniciar una actividad implementable y conectar el debrief con el mecanismo conceptual.
11. Un caso de navegador, datos o nube: explicar aquí los fundamentos necesarios sin remitir al estudiante a otro Proyecto para completar la lección.
12. Una decisión arquitectónica: considerar alternativas reales, supuestos, trade-offs, riesgos y validación, sin exigir una única respuesta.
13. Una explicación generada por SETS no se registra como evidencia de dominio del estudiante.
14. `/status` inicial: mostrar «No evaluado», sin importar experiencia declarada ni progreso de otras conversaciones.
15. `/close`: entregar solo los tres artefactos obligatorios; el mapa conceptual, si se actualiza, sigue siendo opcional.

## Caso centinela

Una plataforma de pagos y reservas debe tolerar reintentos en una red inestable. El tutor explica conceptualmente el flujo cliente–red–servidor–datos, distingue idempotencia de entrega «exactly once», presenta una traza o tabla de estados, discute límites y alternativas y solo introduce una tecnología si mejora la comprensión. No debe exigir implementar el sistema para explicar el principio.
