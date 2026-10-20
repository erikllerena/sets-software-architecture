# Mapa de competencias — Software Architecture & Design

**Programa v1.5.1 · SETS Framework v1.4.1 · Namespace `G00–G12`**

Este programa desarrolla criterio para comprender, diseñar, evaluar y evolucionar sistemas completos. Es autónomo y neutral respecto a lenguajes, frameworks, nubes y estilos arquitectónicos. La meta no es memorizar un catálogo de patrones: es explicar mecanismos, identificar condiciones, comparar alternativas y justificar decisiones.

Este mapa define competencias prioritarias, no agota todos los temas que pueden estudiarse. SETS puede enseñar una pregunta pertinente fuera de `G00–G12` y relacionarla con una competencia existente cuando ayude; solo se propone un módulo nuevo si el tema es recurrente o estratégicamente central. Fundamento, profundización y especialización son alcances adaptativos, no fases obligatorias. La apertura no cambia el foco de arquitectura integral.

## Competencias observables

| ID | Módulo | Capacidad observable | Pregunta conceptual central | Evidencia posible |
|---|---|---|---|---|
| G00 | Diagnóstico arquitectónico transversal | Reconocer contexto, objetivos, supuestos, incertidumbres y límites del propio conocimiento | ¿Qué necesitamos saber antes de decidir? | Diagnóstico razonado y brechas observadas |
| G01 | Pensamiento arquitectónico y requisitos | Traducir necesidades de negocio en drivers, restricciones y criterios de éxito | ¿Cómo influyen los requisitos en la forma del sistema? | Mapa de stakeholders, drivers priorizados y criterios verificables |
| G02 | Fundamentos del sistema completo | Explicar el recorrido entre cliente, red, servicios, datos e infraestructura y sus consecuencias | ¿Cómo se propaga una solicitud, una demora o un fallo entre componentes? | Diagrama de secuencia, presupuesto de latencia o traza causal |
| G03 | Límites, acoplamiento y diseño modular | Delimitar responsabilidades y justificar fronteras entre módulos, componentes y equipos | ¿Dónde conviene separar responsabilidades y qué coste tiene esa frontera? | Mapa de dependencias, contratos y ownership |
| G04 | Atributos de calidad y evaluación | Convertir calidad en escenarios medibles y razonar sobre tensiones entre atributos | ¿Qué significa «bueno» en este contexto y cómo lo comprobaríamos? | Escenarios de calidad, hipótesis y plan de validación |
| G05 | Estilos y patrones arquitectónicos | Comparar monolito modular, distribución, cliente-servidor, eventos y otros estilos según contexto | ¿Qué problema resuelve cada estilo y qué complejidad introduce? | Comparación equilibrada y ADR con alternativas defendibles |
| G06 | Contratos, integración y flujo de información | Razonar sobre APIs, eventos, BFF, caché, sincronización y límites de consistencia | ¿Qué garantías ofrece cada interacción y dónde pueden fallar? | Secuencia, contrato, tabla de estados y escenarios de fallo |
| G07 | Seguridad, privacidad y confianza end-to-end | Modelar activos, fronteras de confianza, amenazas, controles y responsabilidades | ¿Qué puede salir mal, quién puede provocarlo y qué control lo reduce? | Modelo de amenazas proporcional y controles verificables |
| G08 | System design integral | Componer una solución coherente a partir de requisitos, restricciones y estimaciones explícitas | ¿Cómo se relacionan las decisiones locales y qué límites dominan el sistema? | Diseño end-to-end, estimaciones, riesgos y defensa de alternativas |
| G09 | Operabilidad, confiabilidad y experiencia | Diseñar señales, SLI/SLO, recuperación, costes y observabilidad de extremo a extremo | ¿Cómo sabremos que funciona y cómo descubriremos o recuperaremos un fallo? | Plan de observabilidad, indicadores y estrategia de recuperación |
| G10 | Comunicación, documentación y gobernanza | Explicar decisiones a audiencias técnicas y de negocio y conservar su contexto | ¿Cómo hacemos que una decisión sea comprensible, revisable y gobernable? | ADR, vistas C4/arc42 apropiadas y explicación adaptada a audiencia |
| G11 | Evolución, modernización y reversibilidad | Planificar cambios incrementales y reconocer señales para revisar una decisión | ¿Qué cambiaría nuestra decisión y cómo reducimos el coste de cambiarla? | Ruta de evolución, triggers, riesgos y estrategia de reversión |
| G12 | Capstone end-to-end | Integrar conocimientos y defender una arquitectura ante cambios de contexto | ¿Qué propuesta equilibra mejor las necesidades actuales y la evolución probable? | Dossier arquitectónico, revisión adversarial y validación mínima |

## Cómo se aprende cada competencia

La progresión no es una receta rígida. SETS aplica las lentes de `CONCEPTUAL_ENGINE.md` según la dificultad y las necesidades observadas:

1. **Origen:** problema real y por qué aparece.
2. **Mecanismo:** cómo funciona, qué causa qué y qué invariantes importan.
3. **Límites:** supuestos, contraejemplos, fallos y condiciones donde deja de aplicar.
4. **Criterio:** alternativas, trade-offs, señales de éxito y consecuencias.
5. **Transferencia:** qué se conserva y qué cambia en un contexto nuevo.

Estas lentes no son cinco niveles, cinco exámenes ni una escala numérica. Una explicación puede usar solo las lentes necesarias; un concepto complejo puede explorarse en varias sesiones.

## Formas válidas de evidencia

La evidencia depende de la competencia: explicación con palabras propias, predicción de un resultado, traza causal, diagrama, tabla de estados, análisis de contraejemplo, comparación, ADR, cálculo, experimento o implementación. **No se exige código para cada competencia.** Una solución generada por el tutor o una explicación recibida no se registra como desempeño demostrado por el estudiante.

## Método pedagógico

- Diagnóstico breve, una pregunta por turno; al finalizar, síntesis y comienzo de enseñanza conceptual.
- Explicar directamente cuando el estudiante lo pide; no bloquear la explicación con preguntas socráticas.
- No iniciar laboratorios automáticamente después del diagnóstico o de una lección.
- Seleccionar lenguaje y representación por valor explicativo, no por fidelidad a un stack. Preguntar preferencias solo cuando la elección importe; si no, elegir y justificar brevemente.
- Separar principio general de detalles específicos de lenguaje, runtime, protocolo o proveedor.
- Para decisiones, comparar alternativas viables, supuestos, riesgos, trade-offs y señales de validación.
- Evaluar mediante evidencias, ayuda H0–H4 y transferencia; no inferir dominio por familiaridad o una única respuesta.
- Adaptar la ruta a brechas reales, entrevista solicitada o caso de interés; no es obligatorio cursar todos los módulos en orden.

## Rutas

- **Fundamentos:** G01–G05 según diagnóstico; no exigir completar toda la ruta antes de estudiar un concepto concreto.
- **Interacción y sistema end-to-end:** G02, G03, G06, G08 y G09, según necesidad.
- **Riesgo y evolución:** G04, G07, G09, G10 y G11.
- **Entrevista:** solo cuando se active; priorizar la vacante y las brechas observadas, sin asumir lenguaje obligatorio.
- **Capstone:** G12 integra requisitos, decisiones, evidencia y evolución; no exige implementar cada componente.

## Criterio de comprensión profunda

Se busca que el estudiante pueda explicar el problema y el mecanismo, declarar supuestos, anticipar al menos una consecuencia o modo de fallo, reconocer un límite y razonar sobre una alternativa. El dominio se decide con las reglas de `ASSESSMENT_ENGINE.md`, no por contar cuántas lentes se mencionaron.
