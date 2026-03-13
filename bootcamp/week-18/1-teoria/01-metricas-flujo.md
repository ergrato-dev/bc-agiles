# 01 — Métricas de flujo: Cycle Time, Lead Time, Throughput y CFD

## Objetivos

- Calcular Cycle Time y Lead Time con datos reales
- Interpretar un Cumulative Flow Diagram (CFD)
- Detectar cuellos de botella a partir del CFD

---

## 1. Las tres métricas de flujo

El objetivo del Kanban avanzado es gestionar el **flujo de trabajo**, no las personas.
Las tres métricas principales miden distintas dimensiones de ese flujo.

| Métrica | Definición | Fórmula |
| ------- | ---------- | ------- |
| **Lead Time** | Tiempo desde que el ítem entra al sistema hasta que se entrega | `Fecha entrega − Fecha solicitud` |
| **Cycle Time** | Tiempo desde que el equipo empieza a trabajarlo hasta que termina | `Fecha entrega − Fecha inicio real` |
| **Throughput** | Cantidad de ítems entregados por unidad de tiempo | `Ítems / semana` (o días) |

> **Ejemplo**: El cliente solicita una historia el lunes (Lead Time empieza).
> El equipo la toma el jueves (Cycle Time empieza). Se entrega el siguiente miércoles.
> Lead Time = 9 días. Cycle Time = 6 días.

### Ley de Little

$\text{Lead Time} = \frac{\text{WIP}}{\text{Throughput}}$

**Implicación práctica**: para reducir Lead Time, reducir WIP o aumentar Throughput.
Añadir personas sin reducir WIP no siempre mejora el flujo.

---

## 2. Cumulative Flow Diagram (CFD)

El CFD muestra la acumulación de ítems en cada columna a lo largo del tiempo.
Es la herramienta más potente para detectar cuellos de botella visualmente.

### Cómo leer un CFD

- **Eje X**: tiempo (días o semanas)
- **Eje Y**: número de ítems acumulados
- **Cada banda**: una columna del tablero (To Do / In Progress / Done)

### Señales de alerta en un CFD

| Señal | Qué indica |
| ------ | ---------- |
| Banda que se ensancha en el tiempo | Acumulación — cuello de botella en esa fase |
| Banda plana (sin crecimiento en Done) | El equipo no entrega |
| Bandas paralelas y uniformes | Flujo saludable |

---

## 3. Antipatrones de flujo

- ❌ Medir velocity en un tablero Kanban (es una métrica Scrum, no de flujo)
- ❌ Ignorar el WIP limit cuando "hay urgencias"
- ❌ Usar Cycle Time para evaluar el desempeño individual
- ❌ No revisar el CFD hasta que el problema ya es evidente

---

## Checklist

- [ ] ¿Puedes explicar la diferencia entre Lead Time y Cycle Time con un ejemplo?
- [ ] ¿Qué le dice al equipo un CFD con una banda de "In Progress" muy ancha?
- [ ] ¿Cómo afecta el WIP al Lead Time según la Ley de Little?
- [ ] ¿Por qué el Throughput es más útil que la Velocity en equipos Kanban?

---

## Referencias

- Kanban Guide: <https://kanban.university/kanban-guide/>
- Metrics & CFD: <https://kanban.university/kanban-guide/metrics/>
