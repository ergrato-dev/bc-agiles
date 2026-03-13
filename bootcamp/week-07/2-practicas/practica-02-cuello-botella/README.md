# Práctica 02 — Cuello de Botella

**Semana 07 — Introducción a Kanban**
**Tiempo estimado**: 1.5 horas

---

## Contexto

> **Escenario**: El equipo de desarrollo de **DataSync**, una startup de
> integración de datos, lleva 3 semanas con su tablero Kanban. El manager
> comparte la foto del tablero al final de la semana:

```
BACKLOG     | ANÁLISIS  | DESARROLLO  | CODE REVIEW  | STAGING  | DONE
(sin límite)| WIP: 3    | WIP: 5      | WIP: 2       | WIP: 2   |
------------|-----------|-------------|--------------|----------|------
US-020      | US-017    | US-011      | US-007  [2d] |          | US-001
US-021      | US-018    | US-012      | US-008  [3d] | US-009   | US-002
US-022      | US-019    | US-013      |              | US-010   | US-003
US-023      |           | US-014      |              |          | US-004
US-024      |           | US-015      |              |          | US-005
US-025      |           |             |              |          | US-006
```

*[2d] = lleva 2 días en esa columna*

---

## Paso 1: Identificar el cuello de botella

Analiza el tablero. Identifica qué columna es el cuello de botella y
explica los síntomas que lo evidencian.

**Abre `starter/plantilla.md`** y completa la Sección 1.

---

## Paso 2: Medir el impacto

Con los datos disponibles, calcula o estima:
- ¿Cuántos ítems están bloqueados esperando pasar a Code Review?
- ¿Qué parte del tablero está "bloqueada upstream" por el cuello?

**Abre `starter/plantilla.md`** y completa la Sección 2.

---

## Paso 3: Proponer solución

Propón 2 acciones concretas que podría implementar el equipo para
resolver el cuello de botella de Code Review. Una de las acciones debe
ser una mejora estructural (no solo "agregar personas").

**Abre `starter/plantilla.md`** y completa la Sección 3.
