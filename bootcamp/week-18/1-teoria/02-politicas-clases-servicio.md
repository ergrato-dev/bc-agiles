# 02 — Políticas Explícitas, Clases de Servicio y #NoEstimates

## Objetivos

- Definir políticas explícitas útiles para un tablero Kanban
- Clasificar el trabajo por clases de servicio con SLA distinto
- Evaluar cuándo #NoEstimates es más apropiado que la estimación en puntos

---

## 1. Políticas Explícitas

Una política explícita es una **regla visible** que define cuándo un ítem puede
moverse de una columna a la siguiente. Sin políticas, cada persona interpreta
el tablero de forma diferente.

### Ejemplo de políticas por columna

| Columna | Política de entrada | Política de salida |
| ------- | ------------------- | ------------------ |
| **In Progress** | El ítem tiene criterios de aceptación claros y está en la DoR | Todos los criterios de aceptación están verificados |
| **In Review** | El código fue revisado por el autor y hay pull request abierto | Al menos 1 reviewer aprobó y los tests pasan |
| **Done** | El ítem cumple la DoD y fue demostrado al Product Owner | — |

> ⚠️ Las políticas deben estar **escritas y visibles** en el tablero, no en la memoria del equipo.

---

## 2. Clases de Servicio

No todos los ítems tienen la misma urgencia. Las clases de servicio definen
niveles de prioridad con **SLA (Service Level Agreement)** distintos.

| Clase | Descripción | SLA típico |
| ----- | ----------- | ---------- |
| **Urgente** | Bug crítico en producción, riesgo legal | ≤ 24 horas |
| **Fecha fija** | Demo para cliente, lanzamiento planificado | Fecha inamovible |
| **Estándar** | Trabajo normal del equipo | 7–14 días |
| **Intangible** | Deuda técnica, mejoras internas | Sin SLA — cuando hay capacidad |

**Color en el tablero**: cada clase de servicio se representa con un color diferente en las tarjetas.

---

## 3. #NoEstimates

El movimiento #NoEstimates argumenta que **el tiempo dedicado a estimar sería mejor
usado en entregar**. En lugar de Story Points usa métricas de flujo.

### Cuándo considerar #NoEstimates

- El equipo lleva 6+ meses con Throughput estable
- Los ítems de trabajo tienen tamaño similar (slice uniforme)
- Las forecasts de entrega se pueden hacer con datos de flujo histórico

### Cuándo mantener estimaciones

- El equipo es nuevo y necesita calibrar cuánto cabe en el Sprint
- Los ítems varían mucho en tamaño
- Los stakeholders requieren commitments con fechas

> **Posición pragmática**: no es una elección binaria. Muchos equipos maduros
> usan t-shirt sizing rápido (S/M/L) en lugar de Planning Poker para reducir el tiempo de estimación.

---

## Checklist

- [ ] ¿Cuál es la diferencia entre WIP limit y política de salida de una columna?
- [ ] ¿Qué clase de servicio usarías para un bug que bloquea 200 usuarios en producción?
- [ ] ¿En qué condición #NoEstimates tiene más sentido para tu equipo actual?
- [ ] ¿Cómo afectan las clases de servicio al Cycle Time promedio del equipo?

---

## Referencias

- Kanban Classes of Service: <https://kanban.university/kanban-guide/#service-classes>
- #NoEstimates: <https://noestimatesbook.com/> (Vasco Duarte — intro gratuita)
