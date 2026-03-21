<!-- Semana 07: Introducción a Kanban -->
<!-- Práctica 02: Cuello de Botella — SOLUCIÓN -->

# Solución — Cuello de Botella DataSync

---

## Sección 1: Diagnóstico

**Columna cuello de botella**: **Code Review** (WIP limit: 2, ítems actuales: 2 con edad elevada)

**Síntomas:**
1. Los ítems US-007 (2 días) y US-008 (3 días) llevan más tiempo del normal en Code Review; ninguno avanzó a Staging esta semana.
2. Staging tiene solo 2 ítems pero hay 4 en Desarrollo y 2 bloqueados en Code Review. La entrada a Staging está frenada porque Code Review no libera ítems.

**Por qué Desarrollo con 4/5 ítems no es el cuello:**
Desarrollo tiene WIP limit de 5 y solo 4 ítems → hay un slot libre. El trabajo está avanzando (los developers pueden jalar más o terminar uno). En contraste, Code Review tiene 2/2 con ítems envejecidos: no está liberando trabajo hacia Staging.

---

## Sección 2: Impacto

**Ítems bloqueados esperando Code Review:**
Visiblemente: 2 ítems en Code Review con 2–3 días de espera. De Desarrollo, 4 ítems potencialmente listos para pasar a Code Review pero no pueden (WIP lleno). Total bloqueado: ~4–6 ítems.

**Upstream del cuello:**
- Desarrollo: 4 ítems que no pueden avanzar
- Análisis: 3 ítems
- Backlog: 6 ítems
- Total acumulado upstream: 13 ítems "esperando" que el cuello se libere

**Impacto en Lead Time:**
Si Code Review tarda 4 días por ítem y debe procesar aprox. 6 ítems, el próximo ítem espera ~8–12 días solo en esa etapa. Lead Time total estimado: 15–18 días por ítem (vs. los 5 días iniciales de la semana 1).

---

## Sección 3: Acciones propuestas

**Acción 1 — Distribuir Code Review:**
Capacitar a un developer senior para hacer Code Reviews de cambios de bajo riesgo, dejando al tech lead solo para cambios críticos o de arquitectura. Esto dobla la capacidad de la columna sin agregar headcount.

**Acción 2 (estructural) — Reducir el tamaño de los PRs:**
El tech lead hace 1 Code Review/día porque los PRs son grandes. Acordar una política de "PRs ≤ 200 líneas de cambio". PRs pequeños se revisan en minutos, no horas. Esto es un cambio de proceso que acelera el flujo sin agregar personas.

**Por qué aumentar el WIP limit no ayuda:**
El WIP limit refleja la capacidad real de la columna. Si el tech lead solo puede hacer 1 review/día, aumentar el límite a 4 no duplica su capacidad: solo acumula más trabajo sin terminar, aumenta el Lead Time y genera frustración. El WIP limit debe reflejar la capacidad real, no enmascarar el cuello.
