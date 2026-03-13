<!-- ============================================ -->
<!-- PASO 1: Antipatrones — SOLUCIÓN            -->
<!-- ============================================ -->

## Antipatrones en el Sprint Review de TravelNow

| # | Antipatrón detectado | Evidencia en la transcripción | Por qué es un problema |
| - | -------------------- | ----------------------------- | ----------------------- |
| 1 | Review como lectura de tickets | Fede lee tickets cerrados en lugar de mostrar el Incremento funcionando | El Sprint Review inspecciona el **producto**, no la lista de tareas. Sin demo, los stakeholders no pueden evaluar el valor entregado. |
| 2 | Sin Sprint Goal como punto de partida | Andrés no menciona el Sprint Goal al inicio | Sin contexto del objetivo, los stakeholders no saben qué evaluar. El feedback pierde foco. |
| 3 | Feedback sin acción en backlog | Andrés anota el pedido de filtros "para después" informalmente | El feedback de stakeholders debe convertirse en User Stories priorizadas en el backlog. "Anotarlo" sin formalizarlo no genera ningún cambio. |
| 4 | Review demasiado corta (15 min) | El SM cierra en 15 min sin conversación real | Una Review de 2 semanas debería durar hasta 2 horas. 15 minutos indica que no hubo colaboración real con stakeholders. |

---

<!-- ============================================ -->
<!-- PASO 2: Agenda comparada — SOLUCIÓN        -->
<!-- ============================================ -->

## Comparación de agendas

| Momento estándar | ¿Estuvo en TravelNow? | ¿Qué faltó? |
| ---------------- | --------------------- | ------------ |
| Recordar Sprint Goal y capacidad | ❌ No | Andrés abrió directamente con la lista de tickets. No se mencionó el Sprint Goal. |
| Demostración del Incremento | ⚠️ Parcialmente | Fede mostró pantallas sin contexto. No se narró el flujo desde la perspectiva del usuario. |
| Feedback estructurado de stakeholders | ❌ No | Andrés preguntó "¿alguna pregunta?" sin guiar la conversación. No hubo preguntas abiertas ni espacio real. |
| Actualización del Product Backlog | ❌ No | El pedido de Laura quedó en una nota informal. El backlog no cambió. |

---

<!-- ============================================ -->
<!-- PASO 3: Review mejorada — SOLUCIÓN         -->
<!-- ============================================ -->

## Review mejorada — 4 pasos de Rosa

**Paso 1 (0–10 min): Contexto**

Rosa abre la Review recordando el Sprint Goal:
> "El objetivo de este Sprint era que los viajeros pudieran buscar y reservar
> vuelos sin asistencia. Tuvimos una capacidad de 28 puntos y completamos 18,
> cubriendo los tres pasos del flujo principal. Vamos a mostrar exactamente eso."

Esto permite a Laura evaluar con criterio en lugar de juzgar tickets individuales.

**Paso 2 (10–30 min): Demo del Incremento**

Fede narra la demo desde los ojos del usuario:
> "Imaginen que son María, 32 años, quiere volar a Buenos Aires este fin de semana.
> Ingresa al buscador, escribe origen y destino, selecciona fechas…"

Solo se muestran US-18, US-19 y US-21 — las que tienen DoD cumplida.
US-20 y US-22 no se muestran; Rosa lo explica brevemente al inicio.

**Paso 3 (30–50 min): Feedback guiado**

Rosa lanza la pregunta:
> "Laura, si tu equipo de ventas tuviera esta funcionalidad activa mañana,
> ¿qué cambiaría en el proceso de reserva actual? ¿Qué haría diferente un viajero?"

Esto genera feedback accionable. Laura responde con los filtros por aerolínea.

**Paso 4 (50–60 min): Actualización del backlog**

Andrés crea en tiempo real:
> **US-New-01**: Como viajero frecuente, quiero filtrar resultados por aerolínea
> para comparar solo las opciones que prefiero.
> Estimación provisional: 3 pts. Prioridad: Alta (validado por Laura).

Rosa cierra: "Entonces el siguiente Sprint Planning incluirá esta historia
en la discusión de prioridad. ¿Correcto, Laura?" — Laura confirma.
