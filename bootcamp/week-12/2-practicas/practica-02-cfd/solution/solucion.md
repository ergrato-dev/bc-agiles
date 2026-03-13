<!-- ============================================ -->
<!-- PASO 1: SOLUCIÓN — Bottleneck en Review    -->
<!-- Semana 12 — CFD y Métricas de Flujo        -->
<!-- ============================================ -->

## Bottleneck — SOLUCIÓN

**Patrón en Review:** Crece de 2 a 15 ítems en 6 semanas, con saltos en S3 (+5) y S4 (+5).
La banda se ensancha progresivamente — señal clásica de congestionamiento creciente.

**¿Qué significa?** Los ítems entran a Review más rápido de lo que salen.
Development completó más ítems (el nuevo integrante desde S3 aumentó su output),
pero Review no tiene más capacidad para procesar el aumento. El embudo se estrecha
justo antes de Done.

**Impacto en Lead Time:** Un ítem que termina Development en S4 espera en la cola
de Review con otros 14 ítems. Si Norma procesa ~2 ítems/semana (dado que Done creció
~2/semana), el Lead Time de espera solo en Review es 14/2 = 7 semanas.
Esto es un problema crítico de flujo.

---

<!-- ============================================ -->
<!-- PASO 2: SOLUCIÓN — Little's Law            -->
<!-- ============================================ -->

## Little's Law — SOLUCIÓN

**S2:**
- WIP: 4 + 6 + 4 = **14 ítems**
- Throughput S1→S2: Done pasó de 1 a 3 = **2 ítems/semana**
- Lead Time S2: 14 / 2 = **7 semanas**

**S4:**
- WIP: 5 + 11 + 14 = **30 ítems**
- Throughput S3→S4: Done pasó de 5 a 7 = **2 ítems/semana**
- Lead Time S4: 30 / 2 = **15 semanas**

**Conclusión:** El Lead Time empeoró de 7 a 15 semanas entre S2 y S4.
El throughput no creció (sigue siendo ~2/semana) pero el WIP se dobló.
Little's Law predice que si el equipo no actúa, el Lead Time seguirá creciendo.

---

<!-- ============================================ -->
<!-- PASO 3: SOLUCIÓN — Plan de acción          -->
<!-- ============================================ -->

## Plan de acción de Pilar — SOLUCIÓN

**Paso 1 — Acción inmediata:** Congelar el inicio de nuevos ítems en Development.
Nadie jala nuevo trabajo de Analysis hasta que Review baje a 6 ítems (≤ WIP limit propuesto).
Esto "destapa" el cuello: el equipo se enfoca en terminar, no en empezar.

**Paso 2 — Acción a mediano plazo:** Definir quién más puede hacer Review.
Los desarrolladores con mayor experiencia pueden hacer code review entre pares.
La PO define un protocolo de validación rápida (30 min síncronos) en lugar de
revisar todo de forma asíncrona. Esto distribuye la carga de Norma.

**Paso 3 — Acción estructural:** Implementar WIP limit en Review = 5 ítems.
Cualquier ítem que llega a Review cuando ya hay 5 en espera queda en Development
hasta que haya espacio. Esto hace el problema visible antes de que explote.
Además, se agenda un policy de Review responsability compartida en la retro.

**¿Reducir WIP en Development?** Sí — temporalmente. Si Development sigue
llenando a Review al mismo ritmo que antes, el WIP limit en Review será
violado constantemente. Reducir el WIP en Development a 3–4 ítems máximo
sincroniza el ritmo entre ambas columnas y estabiliza el flujo total.
