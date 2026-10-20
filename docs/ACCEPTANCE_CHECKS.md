# Acceptance checks — Software Architecture & Design v1.5.2

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

## Checks de apertura y foco

- **OL1:** Pedir un ejemplo con una tecnología que no figure en la lista familiar: el tutor puede usarla si aclara el mecanismo y no regresa automáticamente a la tecnología familiar.
- **OL2:** Preguntar por un concepto arquitectónico pertinente sin módulo dedicado: se enseña en contexto sin bloquear por el orden del currículo.
- **OL3:** Solicitar un caso nuevo (por ejemplo, plataforma científica o logística): el tutor crea/adapta un escenario y separa hechos, hipótesis y supuestos didácticos.
- **OL4:** Pedir un tema avanzado sin completar el currículo: el tutor cubre los prerrequisitos mínimos y responde al alcance solicitado, sin imponer una ruta completa.
- **OL5:** Preguntar por internals frontend o backend desde una decisión end-to-end: explica lo necesario y conserva el foco arquitectónico, salvo ampliación explícita del estudiante.

## Checks de apertura y foco

- **OL1:** Pedir un ejemplo con una tecnología que no figure en la lista familiar: el tutor puede usarla si aclara el mecanismo y no regresa automáticamente a la tecnología familiar.
- **OL2:** Preguntar por un concepto arquitectónico pertinente sin módulo dedicado: se enseña en contexto sin bloquear por el orden del currículo.
- **OL3:** Solicitar un caso nuevo (por ejemplo, plataforma científica o logística): el tutor crea/adapta un escenario y separa hechos, hipótesis y supuestos didácticos.
- **OL4:** Pedir un tema avanzado sin completar el currículo: el tutor cubre los prerrequisitos mínimos y responde al alcance solicitado, sin imponer una ruta completa.
- **OL5:** Preguntar por internals frontend o backend desde una decisión end-to-end: explica lo necesario y conserva el foco arquitectónico, salvo ampliación explícita del estudiante.

## Caso centinela

Una plataforma de pagos y reservas debe tolerar reintentos en una red inestable. El tutor explica conceptualmente el flujo cliente–red–servidor–datos, distingue idempotencia de entrega «exactly once», presenta una traza o tabla de estados, discute límites y alternativas y solo introduce una tecnología si mejora la comprensión. No debe exigir implementar el sistema para explicar el principio.


## Checks de configuración de Fuentes (v1.5.2, manuales)

- **SRC-01:** Las fuentes cargadas se reconocen por nombre individual; no se espera que ChatGPT conozca la carpeta original. No se cargan tres guías distintas como `README.md`.
- **SRC-02:** `INTERACTION_ENGINE.md`, `DECISION_ENGINE.md` y `PRACTICE_ENGINE.md` están como Fuentes, no como Instrucciones activas concatenadas; el framework conserva v1.4.1.
- **SRC-03:** Sin `LAB_GUIDE.md`, `/learn` y `/lab` siguen funcionando; sin `CONCEPT_MAP.md`, no se inventa su contenido. Se evita usar `ACCEPTANCE_CHECKS.md` como examen del estudiante.
- **SRC-04:** `ARCHITECTURE_DECISIONS_GUIDE.md` describe ADRs técnicos, mientras que `DECISION_ENGINE.md` desarrolla criterio; en el setup se distinguen ambas funciones.

Estas pruebas están definidas pero **no se consideran ejecutadas ni aprobadas** hasta verificar el tutor en un Proyecto real.
