# CASEBOOK — Arquitectura integral y razonamiento causal (v1.5.0)

Los escenarios son ficticios; las cifras introducidas durante una sesión son supuestos educativos, no datos medidos. El tutor puede elegir diagramas, contratos, pseudocódigo o cualquier lenguaje que ayude a comprender. No es necesario programar cada caso.

## Caso conductor: Plataforma Horizonte

Plataforma con aplicación web, clientes móviles potenciales, servicios de negocio, pagos, inventario, analítica y operación. Comienza como un MVP pequeño y cambia a medida que aparecen nuevos requisitos.

| Iteración | Cambio de contexto | Núcleo conceptual a comprender | Evidencia posible |
|---|---|---|---|
| H0 — Primer MVP | Equipo pequeño, una región, presupuesto limitado | Requisitos, límites, acoplamiento y simplicidad proporcional | Context diagram, supuestos y dos alternativas razonables |
| H1 — Checkout lento | Usuarios móviles experimentan latencia alta | Presupuesto de latencia, llamadas en cadena, caché y percepción de espera | Secuencia causal y opciones con costes |
| H2 — Pago duplicado | Un usuario reintenta después de perder la respuesta | Entrega/reintentos, idempotencia, estados y responsabilidades por capa | Tabla de estados, contrato y recorrido del fallo |
| H3 — Equipos autónomos | Tres equipos solicitan desplegar de forma independiente | Límites de dominio, ownership, coordinación y coste de distribución | Mapa de responsabilidades y análisis de alternativas |
| H4 — Conectividad inestable | Una operación se interrumpe a mitad de camino | Fallos parciales, consistencia, recuperación y experiencia de usuario | Traza de fallo y criterios de recuperación |
| H5 — Auditoría de seguridad | Se detectan riesgos de permisos y exposición de datos | Activos, fronteras de confianza, amenazas y defensa en profundidad | Modelo de amenazas proporcional y controles verificables |
| H6 — Pico de demanda | La carga sube diez veces durante una campaña | Cuellos de botella, capacidad, backpressure, degradación y coste | Hipótesis de cuello de botella y plan de medición |
| H7 — Modernización | La plataforma debe evolucionar con presupuesto fijo | Deuda, reversibilidad, migración incremental y señales de abandono | ADR, ruta por etapas y condiciones de revisión |

## Cómo abordar un caso sin convertirlo en examen permanente

El tutor debe comprobar primero si faltan fundamentos y enseñarlos cuando sea necesario. Según el caso, puede recorrer algunas de estas preguntas; no es obligatorio formularlas todas ni hacerlas en turnos separados:

1. ¿Qué problema estamos intentando resolver y para quién?
2. ¿Qué mecanismo causa el comportamiento observado?
3. ¿Qué supuestos y garantías estamos dando por hechos?
4. ¿Qué alternativas son realmente viables y qué coste trae cada una?
5. ¿Qué resultado o fallo podemos predecir?
6. ¿Qué dato, prueba o señal nos permitiría validar la hipótesis?
7. ¿Qué principio se transfiere a otro contexto y qué tendría que cambiar?

Si el estudiante no conoce un concepto necesario, no lo penalices por no adivinarlo: explícalo con un ejemplo trabajado y después, si resulta útil, comprueba la comprensión. Solo activa un laboratorio extenso cuando el estudiante lo solicite o acepte la propuesta.

## Escenarios de transferencia

- Plataforma educativa con vídeo, exámenes y conectividad variable.
- Fintech con transacciones sensibles y requisitos de auditoría.
- SaaS B2B multi-tenant con permisos y aislamiento de datos.
- Portal público con accesibilidad estricta y picos de tráfico.
- Sistema interno que debe modernizarse sin interrumpir la operación.

El propósito no es memorizar la solución de Horizonte, sino reconocer invariantes, detectar diferencias relevantes y adaptar el razonamiento al nuevo contexto.
