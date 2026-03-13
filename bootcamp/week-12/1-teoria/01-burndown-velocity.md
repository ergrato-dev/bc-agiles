# 01 — Burndown Chart y Velocity

## Objetivo

Leer e interpretar un Burndown Chart para detectar riesgos en el Sprint antes de que sea tarde.

---

## 1. ¿Qué es el Burndown Chart?

El Burndown Chart muestra **cuántos puntos quedan por completar** en el
Sprint a lo largo del tiempo. El eje X es los días del Sprint; el eje Y,
los puntos pendientes.

**Línea ideal**: parte del total comprometido (ej: 20 pts) y llega a 0
el último día, asumiendo progreso uniforme.

**Línea real**: refleja lo que ocurre en la práctica.

---

## 2. Patrones de Burndown y su interpretación

| Patrón | Qué ves | Diagnóstico |
| ------ | ------- | ----------- |
| Línea real sigue la ideal | Progreso uniforme diario | Sprint saludable |
| Escalones planos al inicio + caída al final | Trabajo en batch, pocas integraciones | Riesgo de entrega sin validación |
| Línea real por arriba de la ideal | Equipo más lento de lo esperado | Riesgo de no completar el Sprint Goal |
| Línea real cae de golpe a la mitad | Una User Story grande se completó de una vez | Normal si las stories son grandes |
| La línea sube | Se agregaron puntos al Sprint (scope creep) | Violación del Sprint — SM debe intervenir |

---

## 3. Velocity: qué es y qué NO es

| Velocity ES                                | Velocity NO ES                         |
| ------------------------------------------ | -------------------------------------- |
| Promedio histórico de puntos entregados     | Una meta a aumentar sprint a sprint    |
| Herramienta de planificación               | Medida de productividad individual     |
| Dato del equipo como unidad                | Comparable entre equipos distintos     |

> La Velocity varía sprint a sprint. Un Sprint con 15 pts puede ser más
> valioso que uno con 25 si los 15 resolvieron el problema crítico del usuario.

---

## 4. Burnup Chart: la alternativa

El Burnup Chart tiene dos líneas: el **trabajo completado** (sube) y el
**scope total** (puede subir si se agregan ítems). Es más honesto para
mostrar scope creep a stakeholders.

---

## Checklist

- [ ] ¿Sabes dónde está la línea real en relación con la ideal en el día de hoy?
- [ ] ¿Identificas cuándo el equipo completó sus últimas Stories?
- [ ] ¿Puedes nombrar el patrón de Burndown de tu Sprint actual?
- [ ] ¿Sabes si la Velocity del último Sprint fue representativa o atípica?
