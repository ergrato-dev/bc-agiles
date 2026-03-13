# 02 — Cumulative Flow Diagram (CFD) y Métricas de Flujo

## Objetivo

Interpretar un CFD para identificar cuellos de botella y entender Lead Time y Cycle Time.

---

## 1. ¿Qué es el CFD?

El CFD muestra cómo las Stories se acumulan en cada columna del tablero a
lo largo del tiempo. Cada banda de color representa una columna (ej: To Do,
In Progress, Review, Done).

**Cómo leerlo:**
- Eje X: tiempo
- Eje Y: cantidad de ítems
- Bandas angostas = columnas saludables (poco WIP)
- Bandas anchas = columnas con acumulación (posible cuello de botella)

---

## 2. Lead Time vs Cycle Time en el CFD

| Métrica | Definición | Cómo se ve en el CFD |
| ------- | ---------- | -------------------- |
| **Lead Time** | Desde que se crea el ítem (entra al backlog) hasta que se entrega | Distancia horizontal entre la banda "To Do" y "Done" |
| **Cycle Time** | Desde que el equipo empieza a trabajar en él hasta que se entrega | Distancia horizontal en la banda "In Progress" hacia "Done" |

> Lead Time incluye el tiempo de espera. Cycle Time solo el trabajo activo.

---

## 3. Señales de alerta en el CFD

- **Banda "In Progress" crece** → el equipo está empezando más de lo que termina (WIP excesivo)
- **Banda "Review" se ensancha** → bottleneck en revisión o QA
- **Banda "Done" no crece** → nada llega a Done (problema sistémico)
- **Curvas paralelas** → flujo estable y predecible (saludable)

---

## 4. ¿Qué hace el equipo cuando detecta un bottleneck?

1. Hacer visible el bottleneck al equipo (Daily Scrum)
2. Analizar causa raíz: ¿falta de revisores? ¿criterios de DoD muy exigentes?
3. Mover capacidad: alguien del equipo ayuda en la columna congestionada
4. Revisar si el WIP limit es correcto para esa columna

---

## Checklist

- [ ] ¿Puedes identificar qué columna tiene la banda más ancha en un CFD dado?
- [ ] ¿Sabes calcular el Lead Time aproximado mirando el eje horizontal del CFD?
- [ ] ¿Diferencias Lead Time de Cycle Time?
- [ ] ¿Sabes qué significa que dos bandas del CFD divergen?
