# Upgrade — sets-software-architecture 1.4.1 → 1.5.0

## Objetivo

Alinear el programa con **SETS Framework v1.4.0 / Conceptual Mastery** y hacer explícita su neutralidad tecnológica.

## Cambios principales

- Actualizada la referencia del framework a v1.4.0 y el programa a v1.5.0.
- `CHATGPT_PROJECT_INSTRUCTIONS.md` ahora referencia el motor `CONCEPTUAL_ENGINE.md` y explica las cinco lentes adaptativas.
- `PROJECT_RULES.md` desarrolla enseñanza causal, límites de modelos/analogías, elección neutral de tecnología, transferencia y evaluación honesta.
- `PROJECT_CONFIG.yaml` añade configuración conceptual, stack no predeterminado, distinción entre modelo simplificado, comportamiento documentado e hipótesis, y mapa conceptual opcional.
- `CURRICULUM.md` conserva `G00–G12` y hace explícitas las preguntas conceptuales y las evidencias posibles.
- `CASEBOOK.md` prioriza comprensión del mecanismo antes de pedir una decisión y ya no deriva a otros proyectos para completar el aprendizaje.
- `INTERVIEW_SPRINT.md` aclara que la preparación de entrevistas es optativa y no impone lenguaje.
- `state/LEARNING_STATE.md` y `state/EVIDENCE_LOG.md` comienzan sin evidencia ficticia y admiten evidencia conceptual verificable.
- Añadido `state/CONCEPT_MAP.md`, opcional y local a este programa.
- `SETUP_CHATGPT.md` incluye `CONCEPTUAL_ENGINE.md` como fuente esencial y explica cómo reemplazar las fuentes antiguas del Proyecto.

## Contratos preservados

- Namespace de competencias `G00–G12`.
- Evaluación 0–4 y ayudas H0–H4; las lentes conceptuales no son una escala nueva.
- `/close` sigue produciendo tres artefactos obligatorios: `LAST_HANDOFF.md`, `LEARNING_STATE.md` completo y delta de `EVIDENCE_LOG.md`.
- El mapa conceptual es opcional y no es evidencia de dominio por sí solo.
- Sincronización GitHub ↔ ChatGPT sigue siendo manual.

## Actualización recomendada

1. Conserva el historial Git y copia los archivos del paquete respetando las rutas.
2. En el Proyecto de ChatGPT, reemplaza las instrucciones activas por el nuevo `CHATGPT_PROJECT_INSTRUCTIONS.md`.
3. Sustituye las fuentes de framework v1.3.2 por las versiones de `sets-framework` v1.4.0; asegúrate de cargar `core/CONCEPTUAL_ENGINE.md`.
4. Reemplaza las fuentes académicas por las de este programa v1.5.0.
5. Ejecuta los checks de `docs/ACCEPTANCE_CHECKS.md`.

El estado de progreso comienza limpio por decisión del estudiante. No migres evidencia de otras especializaciones.
