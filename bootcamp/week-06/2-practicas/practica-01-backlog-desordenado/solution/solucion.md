<!-- Semana 06: Artefactos de Scrum -->
<!-- Práctica 01: Backlog Desordenado — SOLUCIÓN -->

# Solución — Product Backlog Desordenado

---

## Sección 1: Clasificación

| # | Ítem | Tipo | Justificación |
|---|------|------|---------------|
| 1 | Pagar multas online | **User Story** | Beneficio directo al ciudadano, acción verificable |
| 2 | Migrar a PostgreSQL | **Tarea técnica** | Trabajo interno, el ciudadano no lo percibe directamente |
| 3 | Sistema en la nube | **Restricción técnica** | Es un NFR (non-functional requirement), no una historia |
| 4 | Reportes para el alcalde | **Epic** | Demasiado amplio; requiere descomposición en múltiples stories |
| 5 | Agendar turnos registro civil | **User Story** | Acción específica, valor claro para el ciudadano |
| 6 | Autenticación 2FA | **Tarea técnica / NFR** | Seguridad requerida, habilita otras features pero no es feature per se |
| 7 | App más rápida | **Restricción de calidad** | Sin métricas concretas, es inestimable e inverificable |
| 8 | Historial de ciudadano | **User Story** | Actor (funcionario), acción (ver historial), valor (eficiencia) |
| 9 | Exportar a Excel | **User Story** | Feature concreta con valor para el alcalde / jefe de trámites |
| 10 | Cierre viernes 14:00 | **Restricción de negocio** | Regla del cliente, no una feature del software |
| 11 | Integración facturación | **Epic / Tarea técnica** | Puede generar múltiples User Stories, técnicamente complejo |
| 12 | Sistema sin caídas | **Restricción de calidad** (SLA) | NFR, debe traducirse a métricas como "99.5% uptime" |

---

## Sección 2: User Stories redactadas

### US-001: Pago de multas online

Como **ciudadano** quiero **pagar mis multas municipales desde la app**
para **evitar ir a la municipalidad y hacerlo en cualquier momento**.

**Criterios de Aceptación:**
- Dado que tengo una multa pendiente, Cuando ingreso al portal y selecciono "Pagar multa", Entonces veo el monto, la fecha límite y las opciones de pago disponibles.
- Dado que realizo el pago, Cuando la transacción es exitosa, Entonces recibo un comprobante en PDF por email y la multa desaparece de mis pendientes.
- Dado que mi tarjeta es rechazada, Cuando intento pagar, Entonces el sistema muestra el error del banco y permite intentar con otro método.

---

### US-002: Agendamiento de turnos para registro civil

Como **ciudadano** quiero **agendar un turno para trámites del registro civil online**
para **no tener que esperar en filas y planificar mi visita con anticipación**.

**Criterios de Aceptación:**
- Dado que quiero un turno, Cuando elijo el trámite, el día y la hora disponible, Entonces se confirma mi reserva y recibo un email de confirmación.
- Dado que ya hay un turno reservado, Cuando intento reservar otro para la misma franja, Entonces el sistema lo bloquea y sugiere el siguiente horario disponible.

---

### US-003: Historial de ciudadano para funcionarios

Como **funcionario del municipio** quiero **ver el historial de trámites de un ciudadano**
para **atenderlo más rápido sin pedirle documentos que ya presentó antes**.

**Criterios de Aceptación:**
- Dado que busco a un ciudadano por DNI, Cuando lo encuentro en el sistema, Entonces veo sus últimos 10 trámites con fecha, tipo y estado.
- Dado que un ciudadano no existe en el sistema, Cuando busco su DNI, Entonces el sistema muestra "Ciudadano no registrado" sin exponer datos de otros usuarios.

---

## Sección 3: Top 5 para Sprint 1

**Criterio**: Valor inmediato para el ciudadano + reducción de volumen
de atención presencial (objetivo del cliente).

| Posición | Ítem | Razón |
|----------|------|-------|
| 1 | Pago de multas online | Alta demanda ciudadana + retorno económico inmediato para la municipalidad |
| 2 | Login / registro de ciudadanos | Habilita TODAS las demás features; dependencia técnica crítica |
| 3 | Autenticación 2FA | Requisito legal del cliente; bloquea el lanzamiento sin esto |
| 4 | Agendamiento de turnos | Segundo trámite más frecuente + reduce fila física |
| 5 | Historial de ciudadano (funcionario) | Eficiencia del equipo interno + satisfacción del ciudadano |
