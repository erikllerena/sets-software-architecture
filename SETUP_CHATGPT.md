# Instalar SETS | Software Architecture en ChatGPT Projects

**Proyecto sugerido:** `SETS | Software Architecture` — con memoria limitada al proyecto si la opción está disponible.

## A. Desde el repositorio `sets-framework`
- Pega `core/PROJECT_INSTRUCTIONS.md` como **instrucciones** del Proyecto de ChatGPT.
- Adjunta los archivos sueltos `core/INTERACTION_ENGINE.md`, `core/DECISION_ENGINE.md`, `core/PRACTICE_ENGINE.md`, `core/ASSESSMENT_ENGINE.md` y `core/SESSION_HANDOFF.md`.
- Adjunta `docs/REFERENCE_POLICY.md` (cómo seleccionar y comprobar fuentes) y `docs/LEARNING_SCIENCE.md` (técnicas de estudio). Si tienes límite de archivos, prioriza los motores y el estado; puedes conservar estas dos guías en GitHub y consultarlas cuando hagan falta.
- **Adjunta también `templates/LAST_HANDOFF.template.md` desde el framework**. Es el contrato obligatorio de formato para `/close`, incluso cuando todavía no existe una sesión real.
- `docs/EXAMPLE_SESSION.md`, `docs/QUALITY_CHECKS.md` y `templates/ADR_TEMPLATE.md` son recursos de apoyo, no imprescindibles para cada sesión.

## B. Desde ESTE repositorio de disciplina
- Adjunta `PROJECT_CONFIG.yaml`, `learning/CURRICULUM.md`, `learning/INTERVIEW_SPRINT.md`, `learning/CASEBOOK.md` y **`learning/REFERENCES.md` (bibliografía de arquitectura)**.
- Adjunta `state/LEARNING_STATE.md` y `state/EVIDENCE_LOG.md`. **No adjuntes `state/LAST_HANDOFF.md` antes de tener un cierre real**; cuando exista, adjunta su versión actualizada. **No confundas** el protocolo `sets-framework/core/SESSION_HANDOFF.md` con el resultado `state/LAST_HANDOFF.md`.

## C. Sesión de estudio
1. Inicia con `/start` (diagnóstico) o `/sprint` (preparación de entrevista).
2. Responde una decisión por turno; solicita `/hint` solo cuando haga falta.
3. Finaliza con `/close`: SETS consultará `LAST_HANDOFF.template.md` y generará **tres resultados propuestos**: `state/LAST_HANDOFF.md` íntegro, `state/LEARNING_STATE.md` íntegro y entradas nuevas para añadir a `state/EVIDENCE_LOG.md`.
4. Actualiza esos tres archivos **de manera manual o mediante una integración de escritura que hayas comprobado** y confirma el commit.
5. Reemplaza también los adjuntos del Proyecto de ChatGPT que quedaron obsoletos.

**Importante:** GitHub conserva el historial, ChatGPT facilita el entrenamiento. No se debe asumir que la IA ha guardado los cambios por redactarlos.
