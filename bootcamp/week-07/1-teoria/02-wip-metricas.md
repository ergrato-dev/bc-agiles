# 02 — WIP Limits y Métricas de Flujo

## Objetivos

- Calcular y justificar un WIP limit para una columna
- Distinguir Lead Time de Cycle Time
- Identificar cuellos de botella en un tablero Kanban

---

## 1. WIP Limits — La regla de oro

**WIP** = Work In Progress.  
Un **WIP limit** es el máximo de ítems que puede tener una columna al mismo
tiempo. Cuando se alcanza, el equipo no puede empezar trabajo nuevo:
debe terminar primero lo que está en curso.

**Regla de oro**: "Stop starting, start finishing."

**Por qué funciona**: Multitask reduce la calidad y aumenta el tiempo total
de entrega. Limitar el WIP fuerza al equipo a colaborar para
terminar lo que está en progreso antes de jalar más trabajo.

**Cómo definir un WIP limit inicial**: 2n–1 donde n = número de personas
que trabajan en esa columna (regla aproximada, se ajusta con datos reales).

---

## 2. Lead Time vs Cycle Time

| Métrica | Definición | Se mide desde |
| ------- | ---------- | ------------- |
| **Lead Time** | Tiempo total desde que se solicita hasta que se entrega | Entrada al backlog → Done |
| **Cycle Time** | Tiempo que el equipo activamente trabaja en el ítem | Inicio de trabajo activo → Done |

**Ejemplo**:
- Un bug se reporta el lunes (entra al backlog).
- El equipo lo empieza el miércoles y lo resuelve el viernes.
- **Lead Time**: 5 días (lunes → viernes)
- **Cycle Time**: 3 días (miércoles → viernes)

El **Lead Time** es lo que importa al cliente. El **Cycle Time** es lo
que el equipo puede controlar directamente.

---

## 3. Identificar cuellos de botella

Un **cuello de botella** es la columna donde el trabajo se acumula.
Se reconoce cuando:

- Una columna tiene más ítems que su WIP limit permite
- Los ítems "esperan" antes de entrar a esa columna
- El tiempo en esa etapa es desproporcionalmente largo

**Solución típica**: agregar capacidad a la columna cuello de botella
(más personas, automatización, o dividir la columna en dos etapas).

---

## Checklist de Comprensión

- ¿Puedo calcular un WIP limit inicial usando la fórmula 2n–1?
- ¿Sé cuándo el Lead Time de un ítem es mayor que su Cycle Time?
- ¿Puedo identificar el cuello de botella en un tablero con ítems acumulados?
- ¿Entiendo por qué reducir WIP puede acelerar la entrega general?

---

## Referencias

- Kanban Guide: https://kanban.university/kanban-guide/
- "Making Work Visible" — Dominica DeGrandis: https://itrevolution.com/making-work-visible/
