<!-- Semana 08: Proyecto Integrador Etapa 0 -->
<!-- Práctica 01 — SOLUCIÓN Sprint Planning -->

# Solución — Sprint Planning: ClearRoute Sprint 3

---

<!-- ============================================ -->
<!-- PASO 1: Sprint Goal — SOLUCIÓN              -->
<!-- ============================================ -->

**Sprint Goal:**

> "Para que los viajeros puedan descubrir y guardar las rutas que les
> interesan, el equipo habilitará la búsqueda, el filtrado por dificultad
> y el guardado de favoritas."

**¿Por qué este Sprint Goal y no el de Daniela?**

La PO listó 5 cosas distintas: búsqueda, filtros, favoritas, login social
y un bug. Eso no es un Sprint Goal — es un patch list. El SM facilitó
la conversación para identificar el **hilo de valor común**: la búsqueda
y guardado de rutas forman un flujo de usuario coherente. El login social
y el bug son importantes pero pueden ser Sprint Goals separados.

> Antipatrón detectado: "Sprint como bolsa de tareas" — el Sprint Goal
> debe responder a "¿por qué hacemos este Sprint?" no "¿qué metemos?".

---

<!-- ============================================ -->
<!-- PASO 2: Selección — SOLUCIÓN                -->
<!-- ============================================ -->

**Ítems seleccionados para el Sprint 3:**

| ID | User Story | Pts | Razón de inclusión |
| --- | --- | --- | --- |
| US-007 | Buscar rutas por nombre | 5 | Núcleo del Sprint Goal |
| US-008 | Filtrar rutas por dificultad | 3 | Núcleo del Sprint Goal |
| US-009 | Guardar rutas favoritas | 8 | Núcleo del Sprint Goal |
| US-011 | Bug: mapa en blanco | 2 | Must urgente, afecta UX crítica |

**Total de puntos seleccionados:** 18 pts (dentro de capacidad de 23)

Se dejan 5 puntos de margen para imprevistos y refinamiento mid-Sprint.

**¿Qué ítem NO incluyes y por qué?**

- **US-010 (Login Google, 5 pts)**: no contribuye al Sprint Goal actual.
  Sería un Sprint Goal separado. Si se incluye, fragmenta el foco.
- **US-012 y US-013**: Could — bajo valor en este momento dado el backlog.

---

<!-- ============================================ -->
<!-- PASO 3: Descomposición — SOLUCIÓN           -->
<!-- ============================================ -->

**US-007: Buscar rutas por nombre**

| Tarea | Horas | Responsable |
| ----- | ----- | ----------- |
| Diseñar componente de barra de búsqueda | 4h | Areli (Frontend) |
| Endpoint GET /routes?q=term con full-text search | 6h | Bruno (Backend) |
| Tests unitarios del endpoint | 3h | Carmen (QA) |

**US-008: Filtrar rutas por dificultad**

| Tarea | Horas | Responsable |
| ----- | ----- | ----------- |
| Agregar filtros al componente de búsqueda | 3h | Areli (Frontend) |
| Extender el endpoint con param ?difficulty= | 4h | Bruno (Backend) |

---

<!-- ============================================ -->
<!-- PASO 4: Verificación — SOLUCIÓN             -->
<!-- ============================================ -->

| Ítem del Checklist | Estado |
| ------------------ | ------ |
| Sprint Goal definido y claro para todos | ✓ |
| Capacidad del equipo calculada | ✓ (23 pts disponibles, 18 seleccionados) |
| Todos los ítems seleccionados cumplen DoR | ✓ (verificar US-011 antes de Lunes) |
| Tareas descompuestas y asignadas | ✓ |
| Sprint Planning cerrado en ≤4 horas | ✓ (estimado: 3h) |

**Riesgos identificados:**

1. US-009 (guardar favoritas, 8pts) depende de que el backend de autenticación
   esté estable. Bruno debe verificar el estado de la sesión antes del miércoles.
2. Carmen tiene un día de reuniones el jueves — coordinar con Diego para cubrir QA.
