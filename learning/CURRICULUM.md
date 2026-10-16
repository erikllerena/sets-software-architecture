# SETS 1.3.1 — Mapa de competencias del Software Architect

No es una lista de cursos que hay que consumir en orden. Es una **matriz de competencias observables**, reutilizable por disciplinas y guiada por problemas; la preparación para entrevistas prioriza mientras la formación profunda construye fundamentos sólidos.

| ID | Dominio | Capacidad que debe demostrar | Evidencia práctica |
|---|---|---|---|
| M00 | Diagnóstico | Identificar datos faltantes, justificar una postura, expresar incertidumbre | Decisión corta + 5–7 preguntas adaptativas |
| M01 | CS para arquitectos | Razonar sobre redes, OS, latencia, concurrencia, memoria, IO y complejidad | Interpretar cuello de botella y fallo probable |
| M02 | Diseño de software | Modularidad, cohesión, acoplamiento, SOLID/GRASP y patrones con criterio | Refactor con antes/después y justificación |
| M03 | Arquitecturas de aplicación | Comparar capas, monolito modular, hexagonal, clean y onion | Diagrama de dependencias + ADR |
| M04 | Domain design | Modelar invariantes, agregados, contextos y límites sin exceso de patrones | Dominio y eventos analizados |
| M05 | API & integration | Diseñar contratos, evolución, seguridad básica, errores e idempotencia | API con casos de timeout y duplicados |
| M06 | Datos y consistencia | SQL/NoSQL, aislamiento, locking, modelado, índices y trade-offs | Invariante + estrategia de transacción y pruebas |
| M07 | Distribución | Orden, retries, fallos parciales, colas, sagas y consistencia | Flujo bajo fallo + plan de recuperación |
| M08 | Atributos de calidad | Definir y medir rendimiento, disponibilidad, resiliencia, escala y DR | Escenarios de calidad medibles + riesgo |
| M09 | Seguridad | Threat modeling, identidad, autorización, secretos y trazabilidad | Riesgos + controles comprobables |
| M10 | Cloud & operations | CI/CD, despliegue, observabilidad, costos, capacidad y operación | Runbook/SLI/SLO/plan de recuperación |
| M11 | Comunicación técnica | C4, UML selectivo, ADR, RFC, negociación y presentación | Defensa para equipo y stakeholder no técnico |
| M12 | System design | Analizar, estimar, componer y defender sistemas end-to-end | Diseño con supuestos y trade-offs |
| M13 | Evolución y gobernanza | Migraciones, deuda, fitness functions, ownership y cambio organizacional | Plan incremental con triggers claros |
| M14 | Capstone | Integrar las competencias en un caso cambiante | Dossier + prototipo selectivo + review adversarial |

## Competencias transversales (se evalúan dentro de cada módulo)
- **Pensamiento crítico:** discriminar hechos de conjeturas, ofrecer alternativa fuerte, identificar datos que faltan.
- **Toma de decisiones:** seleccionar criterio dominante y justificar sacrificios, reversibilidad y costo.
- **Práctica profesional:** verificar con pruebas/telemetría y reconocer límites de lo no ejecutado.
- **Comunicación e influencia:** adaptar explicación a ingeniería, operaciones y negocio.
- **Metacognición:** explicar qué cambió en su modelo mental y cuándo revisaría su decisión.

## Rutas iniciales
**Entrevista:** diagnóstico M00 → M02/M03 → M05/M06/M07 → M08/M11/M12, en orden adaptado a vacíos y vacante. No omitir incidentes y seguridad cuando el puesto los exige.

**Roadmap duradero:** reforzar fundamentos M01–M02, luego M03–M04, integraciones/datos M05–M07, atributos/operación M08–M10 y defensa/evolución M11–M14; trabajar ciclos y dependencias, no cursos rígidos.

**Tecnología concreta:** aplicar motor técnico a Java, Kafka, PostgreSQL, Kubernetes u otra; justificar por qué es pertinente para la capacidad objetivo. Puede existir un Proyecto de ChatGPT por especialidad con su propio estado.

## Hitos de desarrollo (no rangos de empleo ni certificación)
1. **Interpretar:** explicar mecanismos con ejemplos correctos.
2. **Diagnosticar:** anticipar fallos y aislar hipótesis.
3. **Diseñar:** proponer alternativas condicionadas por requisitos.
4. **Validar:** verificar invariantes, calidad y riesgos con pruebas.
5. **Defender:** responder objeciones y adaptar decisiones con evidencia.
6. **Evolucionar:** revisar decisiones, mantener sistemas y trabajar con stakeholders.

## Capstone: criterio de completitud
Contexto realista, no objetivos y restricciones, 3 escenarios de calidad medibles, módulos/datos/contratos, dos ADR relevantes, threat model proporcional, riesgos operativos/costos, experimento comprobable, plan de migración y presentación a stakeholders. No hace falta codificar todo el sistema; construir solo lo necesario para probar hipótesis.
