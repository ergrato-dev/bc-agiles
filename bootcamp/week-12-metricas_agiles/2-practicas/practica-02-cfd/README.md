# Práctica 02 — Lectura del CFD y Detección de Bottlenecks

**Semana 12 · Métricas Ágiles**
**Duración estimada**: 2 horas

---

## Contexto

El equipo de **SupplyPulse** (gestión de inventario para distribuidoras)
usa un tablero Kanban con 5 columnas: Backlog | Analysis | Development |
Review | Done.

El SM, **Pilar**, revisa el CFD de las últimas 3 semanas y nota algo
preocupante.

---

## Datos del CFD (ítems acumulados por columna por semana)

| Semana | Backlog | Analysis | Development | Review | Done |
| ------ | ------- | -------- | ----------- | ------ | ---- |
| S1     | 25      | 3        | 4           | 2      | 1    |
| S2     | 22      | 4        | 6           | 4      | 3    |
| S3     | 19      | 5        | 9           | 9      | 5    |
| S4     | 16      | 5        | 11          | 14     | 7    |
| S5     | 14      | 5        | 12          | 14     | 11   |
| S6     | 12      | 4        | 11          | 15     | 14   |

> *Los números son acumulados: un ítem que pasa por Analysis en S1 y
> S2 cuenta en S1 y S2. Done es siempre creciente.*

---

## Paso 1: Identificar el bottleneck

Mira la banda "Review": ¿qué ocurre entre S3 y S6? ¿Qué significa ese
ensanchamiento? ¿Cómo impacta al Lead Time?

---

## Paso 2: Calcular el Lead Time aproximado

En S4, el promedio de ítems en el sistema (columnas Analysis + Development +
Review) es: 5 + 11 + 14 = 30 ítems. El throughput (Done) creció de S3→S4 en
2 ítems. Usando Little's Law de forma aproximada: Lead Time ≈ WIP / Throughput.

Calcula el Lead Time aproximado en S4 y compáralo con el de S2.

---

## Paso 3: Plan de acción de Pilar

¿Qué haría Pilar para resolver el bottleneck en Review? Da un plan de 3 pasos
específicos (no solo "reducir WIP").
