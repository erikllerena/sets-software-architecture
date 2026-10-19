# Instalación — SETS | Software Architecture & Design v1.5.0

## 1. Crea el Proyecto
Nombre sugerido: **SETS | Software Architecture & Design**. Si la opción está disponible, selecciona memoria solo del Proyecto para mantener su contexto académico aislado. Este programa no requiere sesiones, progreso ni fuentes de otras especializaciones.

## 2. Instrucciones activas
Pega **solo** el contenido de `CHATGPT_PROJECT_INSTRUCTIONS.md` de este repositorio en las instrucciones del Proyecto. Ya incorpora la identidad y las reglas esenciales de esta disciplina. Si el Proyecto existía de antes, reemplaza las instrucciones anteriores para evitar directrices contradictorias.

## 3. Fuentes del framework común
Desde `sets-framework` v1.4.0, sube estos archivos como fuentes del Proyecto:

**Esenciales**
- `core/PROJECT_INSTRUCTIONS.md`
- `core/CONCEPTUAL_ENGINE.md` — nuevo motor conceptual, imprescindible para esta versión.
- `core/INTERACTION_ENGINE.md`
- `core/DECISION_ENGINE.md`
- `core/PRACTICE_ENGINE.md`
- `core/ASSESSMENT_ENGINE.md`
- `core/SESSION_HANDOFF.md`
- `templates/LAST_HANDOFF.template.md`

**Recomendadas**
- `templates/CONCEPT_MAP.template.md`
- `templates/ADR_TEMPLATE.md`
- `docs/REFERENCE_POLICY.md`
- `docs/LEARNING_SCIENCE.md`
- `docs/QUALITY_CHECKS.md`
- `docs/COMMAND_REFERENCE.md`

No basta con actualizar GitHub: las fuentes antiguas del Proyecto deben reemplazarse manualmente para que ChatGPT use los motores nuevos.

## 4. Fuentes de este repositorio
Sube:
- `PROJECT_CONFIG.yaml`
- `PROJECT_RULES.md`
- `learning/CURRICULUM.md`
- `learning/CASEBOOK.md`
- `learning/REFERENCES.md`
- `learning/INTERVIEW_SPRINT.md` (aunque el modo entrevista sea opcional)
- `state/LEARNING_STATE.md`
- `state/EVIDENCE_LOG.md`
- `state/CONCEPT_MAP.md` (opcional; puede mantenerse como archivo de trabajo)

`state/LAST_HANDOFF.md` no se adjunta antes del primer `/close` real.

## 5. Primer uso
- `/start`: diagnóstico breve y después enseñanza conceptual.
- `/learn <tema>`: empieza directamente una lección conceptual profunda.
- `/deep <tema>`: mecanismos, invariantes, límites y fallos.
- `/explain`: explicación directa, sin intento previo obligatorio.
- `/lab <tema>`: práctica implementable cuando la solicites.
- `/interview` o `/sprint`: activa preparación de entrevista; no se activa por defecto.
- `/close`: genera los tres artefactos obligatorios; revisa antes de guardar.

## 6. Verificación rápida
Pregunta: «¿Cómo decides qué lenguaje utilizar para explicar un concepto, qué haces después del diagnóstico y qué evidencia demostraría comprensión profunda?». La respuesta debe indicar que no existe stack fijo, que el tutor elige o pregunta solo si importa, que después del diagnóstico empieza a enseñar y que el dominio requiere evidencia observable, no exposición pasiva.

## 7. Continuidad
Guarda resultados en GitHub de este repositorio y actualiza manualmente las fuentes del Proyecto. Para continuar en un chat nuevo, permanece en el mismo Proyecto y usa `/resume`. No afirmes que existe sincronización automática entre GitHub y ChatGPT.
