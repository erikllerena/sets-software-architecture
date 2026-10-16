# SETS 1.3.1 — Biblioteca de casos, cambios de contexto y consecuencias

## Caso conductor: MercadoLocal (ficticio; los valores son **supuestos para practicar**)
Plataforma para navegar catálogo, reservar inventario, crear pedidos, cobrar y notificar. Se evita obligar a usar microservicios por moda. Cada iteración introduce un riesgo nuevo; el estudiante decide y defiende **sin conocer la respuesta de antemano**.

### Nivel 0: negocio naciente
**Supuestos:** 4 desarrolladores, 3 000 pedidos/día, un mercado, Spring Boot + PostgreSQL, presupuesto ajustado. **Reto:** límites de módulos e invariantes, diseño desplegable, seguridad esencial, operación mínima y alternativa de evolución. **Entregables:** 1 diagrama (C4 o equivalente), 1 ADR, 2 riesgos y una validación barata.

### Nivel 1: doble reserva de inventario
Pedidos concurrentes consumen el mismo último artículo. **Reto:** formular la invariante; proponer prueba que reproduzca fallo, opciones de sincronización/transacción y plan de evaluación bajo carga. **Entregable:** caso de prueba + decisión contextual.

### Nivel 2: proveedor de pagos ambiguo
Un timeout HTTP puede ocurrir **después del cobro**. **Reto:** idempotencia extremo a extremo, reconciliación, reintentos seguros y trazabilidad. **Entregable:** flujo bajo fallo + contrato + observabilidad.

### Nivel 3: escala asimétrica
**Supuesto:** tráfico de lectura del catálogo crece 30× y pedidos 2×. **Reto:** identificar las métricas que faltan, probar hipótesis de cuello de botella y comparar índice, caché, réplica, CDN, separación de carga y nueva arquitectura. **Entregable:** experimento + ADR condicional.

### Nivel 4: continuidad y operaciones
Negocio exige despliegues frecuentes con riesgos limitados. **Reto:** SLI/SLO tentativos, backup/restore probado, rollback, alertas accionables, manejo de incidentes y presupuesto. **Entregable:** plan operativo + señal de revisión.

### Nivel 5: cambio organizativo
Dos equipos operan catálogos y pedidos con calendarios independientes. **Reto:** autonomía vs costos de distribución, ownership de datos, contratos, seguridad, migración y compensaciones. **Entregable:** arquitectura evolucionada y estrategia incremental.

## Banco de transferencias (no equivalentes exactos)
- **Citas médicas:** doble reserva y cancelación; ponderar consistencia, auditoría y experiencia de usuario.
- **Notificaciones masivas:** deduplicación, retries, tasa, backpressure, costes y gestión de proveedores.
- **Fintech ledger:** trazabilidad, dinero como invariante, conciliación, seguridad y cambios auditables.
- **Biblioteca universitaria:** picos de inscripción, control de cupos, compatibilidad de contratos.
- **Legado empresarial:** despliegues acoplados, schema evolution, strangler incremental y ownership.

## Inyecciones para el reviewer (usar máximo una por ronda)
- El presupuesto operativo se reduce 40%.
- Falló una dependencia externa durante 30 minutos.
- Se detecta inconsistencia sin pérdida de datos pero con impacto económico.
- El equipo no puede operar un broker 24/7.
- Dos equipos disputan propiedad de la misma entidad.
- Un requisito regulatorio obliga a conservar evidencia de cambios.

El tutor **no debe revelar todas estas inyecciones al abrir una simulación**. La elección será contextual y no un castigo por no anticipar un dato invisible. Si surge un dato nuevo, se espera revisar la decisión, no adivinarlo.

## Contrato de caso
- Antes: objetivo de competencia, restricciones dadas, datos desconocidos y producto esperado.
- Durante: una pregunta por turno; no resolver antes de intento; variar rol cuando resulte útil.
- Después: puntos fuertes, 1–2 problemas prioritarios, alternativa fuerte, validación, evidencia (solo si hubo respuesta) y seguimiento.

## Evaluación
Priorizar comprensión de objetivos, invariante, alternativas, causalidad, modos de fallo, costos y capacidad de **cambiar razonadamente de postura**. No puntuar por cantidad de cajas del diagrama ni tecnologías citadas.
