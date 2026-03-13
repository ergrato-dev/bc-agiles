# Práctica 01 — Lectura de un CFD y Detección de Cuellos de Botella

## Escenario: BuildSafe — Empresa de inspecciones de seguridad laboral

**BuildSafe** gestiona solicitudes de inspección para obras de construcción.
Tienen un tablero Kanban con estas columnas:

`Backlog → Asignado → En Inspección → En Revisión Legal → Entregado`

Natalia, la Kanban Master del equipo, tiene los siguientes datos del mes de marzo:

### Datos del CFD — Semana 3 de marzo

| Día | Backlog (acumulado) | Asignado | En Inspección | En Revisión Legal | Entregado |
| --- | --- | --- | --- | --- | --- |
| 1  | 40 | 35 | 20 | 5  | 2  |
| 3  | 45 | 38 | 22 | 7  | 4  |
| 5  | 48 | 40 | 24 | 12 | 6  |
| 7  | 50 | 41 | 26 | 18 | 8  |
| 9  | 52 | 42 | 27 | 22 | 10 |
| 11 | 54 | 43 | 28 | 25 | 13 |
| 13 | 55 | 44 | 29 | 26 | 15 |

---

### Paso 1: Detectar el cuello de botella

> **Observa los datos de la columna "En Revisión Legal".**
> Del día 1 al día 13, esa columna creció de 5 a 26 ítems acumulados, mientras que
> "Entregado" solo creció de 2 a 15.

**Preguntas:**

1. ¿En qué columna está el cuello de botella? Justifica con los datos de la tabla.
2. ¿Qué pasará con el Lead Time si esta situación continúa la semana siguiente?

---

### Paso 2: Calcular métricas de flujo

Usa los datos del Día 1 y el Día 13:

- **Throughput**: ¿Cuántos ítems se entregaron en 13 días?
- **Cycle Time promedio**: En el día 13, hay 26 ítems en "En Revisión Legal".
  Si el WIP promedio del equipo completo es 14, usa la Ley de Little para estimar el Lead Time.

---

### Paso 3: Proponer acciones

Natalia necesita 2 acciones concretas para resolver el cuello de botella en "En Revisión Legal".

**Abre `starter/plantilla.md`** y completa los 3 pasos.
