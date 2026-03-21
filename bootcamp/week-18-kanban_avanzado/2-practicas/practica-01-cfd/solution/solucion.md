<!-- Semana 18: Práctica 01 — CFD — SOLUCIÓN -->

<!-- ============================================ -->
<!-- PASO 1 — SOLUCIÓN                          -->
<!-- ============================================ -->

**1. ¿En qué columna está el cuello de botella?**

**"En Revisión Legal"** es el cuello de botella.

Del día 1 al día 13, esa columna acumuló 21 ítems nuevos (de 5 a 26), mientras que
"Entregado" solo creció 13 ítems (de 2 a 15). Hay un diferencial de 8 ítems atrapados
en Revisión Legal que no pasan a Entregado.

En un CFD, esto se visualiza como una banda que se **ensancha progresivamente**:
señal inequívoca de acumulación y cuello de botella.

**2. ¿Qué pasará con el Lead Time si continúa?**

Según la Ley de Little: `Lead Time = WIP ÷ Throughput`.
Si el WIP sigue creciendo (más ítems se acumulan en Revisión Legal) sin que aumente
el Throughput, el Lead Time aumentará proportionalmente.
El cliente espera más tiempo entre que hace la solicitud y recibe el informe.

---

<!-- ============================================ -->
<!-- PASO 2 — SOLUCIÓN                          -->
<!-- ============================================ -->

**Throughput:**
Ítems entregados en 13 días: 15 − 2 = **13 ítems**
Throughput diario promedio: 13 ÷ 13 = **1 ítem/día**

**Lead Time estimado:**
WIP = 14 ítems
Throughput = 1 ítem/día
Lead Time = 14 ÷ 1 = **14 días**

> Interpretación: en promedio, un ítem de inspección tarda 14 días desde que
> entra al sistema hasta que se entrega al cliente.

---

<!-- ============================================ -->
<!-- PASO 3 — SOLUCIÓN                          -->
<!-- ============================================ -->

**Acción 1: Reducir el WIP limit de "En Revisión Legal"**

Natalia establece un WIP limit de 6 para "En Revisión Legal".
Esto fuerza al equipo a **terminar revisiones antes de iniciar nuevas**,
en lugar de acumular trabajo sin resolver.

**Acción 2: Asignar un revisor legal dedicado al proceso**

El cuello en Revisión Legal probablemente indica un solo revisor saturado.
Natalia escala el impedimento al gerente de operaciones para asignar
un segundo revisor legal durante las próximas 2 semanas.
Criterio de éxito: Throughput de Revisión Legal ≥ 3 ítems/día en sprint siguiente.
