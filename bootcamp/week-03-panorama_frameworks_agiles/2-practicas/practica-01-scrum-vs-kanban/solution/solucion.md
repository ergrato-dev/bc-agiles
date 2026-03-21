<!-- Semana 03: Panorama de Frameworks Ágiles -->
<!-- Práctica 01 — Solución de referencia -->

# Práctica 01 — Solución

---

<!-- ============================================ -->
<!-- PASO 1: Equipo A — SOLUCIÓN                -->
<!-- ============================================ -->

**Framework recomendado:** **Scrum**

**Razón #1:** El trabajo llega en lotes planificados con el equipo de producto.
Los Sprints de 2 semanas permiten compromisos claros y demos periódicas que
el gobierno-cliente valida.

**Razón #2:** Los stakeholders quieren visibilidad periódica. La Sprint Review
satisface exactamente esa necesidad sin requerir acceso constante al equipo.

**Evento más valioso:** La **Sprint Review**: permite que reguladores y el
equipo de producto vean el software funcionando y ajusten prioridades.

---

<!-- ============================================ -->
<!-- PASO 2: Equipo B — SOLUCIÓN                -->
<!-- ============================================ -->

**Framework recomendado:** **Kanban**

**¿Por qué Scrum NO es adecuado?**
1. Los tickets llegan de forma impredecible: los Sprints se romperían
   constantemente con interrupciones. No hay "Sprint Goal" posible.
2. El Sprint Planning no tiene sentido si no se puede predecir qué tickets
   llegarán esta semana.

**Elementos clave de Kanban para Equipo B:**
- Tablero con columnas: In Queue → In Progress → Blocked → Done
- WIP limit en "In Progress" (ej: max 2 tickets por persona)
- Métricas: tiempo de ciclo (cycle time) por tipo de ticket
- Política explícita de SLA: crítico < 2h, normal < 24h

---

<!-- ============================================ -->
<!-- PASO 3: Equipo A híbrido — SOLUCIÓN         -->
<!-- ============================================ -->

**Propuesta: Scrumban**
Mantener los Sprints para las funcionalidades planificadas pero agregar un
carril separado en el tablero para tickets reactivos del legado. Los límites
WIP en el carril reactivo impiden que consuman toda la capacidad del equipo.
La capacidad planificada se reduce (ej: 70% producto nuevo, 30% mantenimiento).

**Riesgo si no se gestiona:** El trabajo reactivo expande hasta consumir el
100% del Sprint, y nunca se entrega trabajo planificado. El producto nuevo
queda paralizado. Síntoma: el Sprint Goal se incumple sistemáticamente.

---

<!-- ============================================ -->
<!-- PASO 4: Antipatrón — SOLUCIÓN              -->
<!-- ============================================ -->

**Antipatrón:** "Cargo cult ágil" / "Scrum forzado"

**Consecuencia observada:** Los tickets reactivos se atienden fuera del
proceso Scrum, creando un proceso informal paralelo. El tablero de Scrum
no refleja el trabajo real del equipo. Las métricas de velocity son falsas.

**Cambio mínimo del Scrum Master:**
Proponer a la organización adoptar **Scrumban** para el Equipo B:
mantener la retrospectiva quincenal (útil para mejora), eliminar el Sprint
Planning predictivo, y añadir un tablero Kanban con WIP limits para los tickets.
La Retrospectiva como único evento de Scrum es más que suficiente para un
equipo de soporte.
