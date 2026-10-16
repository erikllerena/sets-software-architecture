# SETS · Software Architecture & Design

Este repositorio contiene **el programa de aprendizaje de Arquitectura y Diseño de Software**, configurado para desarrollar competencias profesionales de **Software Architect**. Es una disciplina que usa **SETS Framework v1.3.1**, no el framework mismo.

**Objetivos complementarios:** entrevista técnica próxima (track inmediato) y formación profunda a largo plazo (track permanente).

```text
sets-software-architecture/
├── PROJECT_CONFIG.yaml
├── learning/
│   ├── CURRICULUM.md
│   ├── INTERVIEW_SPRINT.md
│   ├── CASEBOOK.md
│   └── REFERENCES.md
├── state/
│   ├── LEARNING_STATE.md
│   ├── EVIDENCE_LOG.md
│   └── LAST_HANDOFF.md
├── decisions/
├── labs/
└── SETUP_CHATGPT.md
```

## Uso

1. Mantén también el repositorio **`sets-framework`**. GitHub no comparte los archivos automáticamente entre repositorios.
2. Sigue [`SETUP_CHATGPT.md`](SETUP_CHATGPT.md) para combinar ambos repositorios en **un Proyecto de ChatGPT** llamado `SETS | Software Architecture`.
3. Ajusta `PROJECT_CONFIG.yaml` con los datos de tu entrevista cuando los conozcas. `assessed_level: null` significa **aún sin evaluar**.
4. Empieza con `/start` (diagnóstico) o `/sprint` (entrevista).
5. Al terminar con `/close`, guarda `state/LAST_HANDOFF.md`, reemplaza `state/LEARNING_STATE.md` y añade únicamente las nuevas entradas observadas a `state/EVIDENCE_LOG.md`; compara IDs para evitar duplicación.
6. Confirma cambios en GitHub y actualiza los adjuntos correspondientes en ChatGPT. **Guardar en GitHub no actualiza por sí solo los archivos del Proyecto.**

La bibliografía específica de arquitectura vive en `learning/REFERENCES.md`; la política general para evaluar fuentes está en `sets-framework/docs/REFERENCE_POLICY.md`.

Es preferible que este repositorio sea **privado** si contendrá evaluaciones personales o notas privadas; no subas credenciales ni datos propietarios.
