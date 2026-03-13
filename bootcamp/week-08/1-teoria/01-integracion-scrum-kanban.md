# 01 — Integración de Scrum y Kanban

## Objetivos

- Identificar cuándo combinar prácticas de Scrum y Kanban
- Reconocer cómo el tablero Kanban complementa el Sprint Backlog
- Aplicar el flujo de trabajo integrado en tu proyecto

---

## 1. Scrum y Kanban: herramientas complementarias

Scrum define el **ritmo** del trabajo (Sprints, eventos, roles).
Kanban define la **visualización del flujo** dentro del Sprint.

Un equipo Scrum puede usar un tablero Kanban **dentro** de cada Sprint:

```
Product Backlog ──► Sprint Backlog ──► Tablero Kanban del Sprint
                                        To Do │ In Progress │ Review │ Done
```

---

## 2. ¿Cuándo usar Scrum, Kanban o Scrumban?

| Situación | Recomendación |
| --------- | ------------- |
| Trabajo en producto con entregas iterativas | Scrum + tablero Kanban interno |
| Flujo continuo de soporte o mantenimiento | Kanban puro (sin Sprints) |
| Equipo en transición | Scrumban (Sprint + WIP limits) |
| Equipo con alta variabilidad en tamaño de ítems | Kanban avanzado |

> El error más común: usar el tablero como decoración sin respetar el WIP limit.

---

## 3. Flujo del Sprint Integrador

```
Sprint Planning ──► Tablero activo ──► Sprint Review ──► Retro
                    (visualización      (Incremento)      (mejora)
                     + WIP limits)
```

El tablero del Sprint debe mostrar **en todo momento** qué está Done,
qué está en progreso y dónde está el cuello de botella.

---

## 4. Antipatrones del Sprint Integrador

- **Ocultar impedimentos**: El tablero muestra los bloqueos; ignorarlos no los resuelve.
- **Sprint Goal vago**: Si el equipo no sabe cuál es el objetivo del Sprint, no puede priorizar.
- **Retro sin acciones**: La reunión sin una mejora concreta es tiempo perdido.
- **Review sin stakeholders**: El feedback del cliente es el insumo para el siguiente Sprint.

---

## Checklist

- [ ] ¿Tu tablero refleja el estado real del trabajo hoy?
- [ ] ¿El Sprint Goal es claro y mide algo concreto?
- [ ] ¿Los eventos del Sprint tienen un facilitador definido?
- [ ] ¿La Retrospectiva tiene al menos una acción con responsable?

---

## Referencias

- [Scrum Guide 2020 — The Sprint](https://scrumguides.org/scrum-guide.html#the-sprint)
- [Atlassian — Scrum vs. Kanban](https://www.atlassian.com/agile/kanban/kanban-vs-scrum)
