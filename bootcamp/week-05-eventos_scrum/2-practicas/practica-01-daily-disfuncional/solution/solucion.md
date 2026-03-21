<!-- Semana 05: Eventos de Scrum -->
<!-- Práctica 01: Daily Scrum Disfuncional — SOLUCIÓN -->

# Solución — Daily Scrum Disfuncional

---

<!-- ============================================================ -->
<!-- SECCIÓN 1: Diagnóstico — SOLUCIÓN                          -->
<!-- ============================================================ -->

## Sección 1: Diagnóstico del Daily actual

| # | Nombre del antipatrón | Cita de la transcripción que lo evidencia |
|---|----------------------|------------------------------------------|
| 1 | **Stand-up de reporte al SM** | "Rodrigo: Ana, ¿qué hiciste ayer?" — las preguntas las hace el SM, no el equipo |
| 2 | **Resolución de problemas en el Daily** | 11 minutos discutiendo el bug de Ana y la librería (09:03–09:08) |
| 3 | **Impedimento no escalado en 3 días** | El servidor de staging lleva 3 días caído y se menciona como dato |
| 4 | **Extensión del Daily con temas de Backlog** | "¿alguien tiene temas del backlog que quiera revisar? aprovechememos…" — 09:17–09:44 |

---

<!-- ============================================================ -->
<!-- SECCIÓN 2: Reformulado — SOLUCIÓN                          -->
<!-- ============================================================ -->

## Sección 2: Daily Scrum reformulado

**Las 3 preguntas correctas:**

1. ¿Qué hice ayer que contribuyó al Sprint Goal?
2. ¿Qué haré hoy para contribuir al Sprint Goal?
3. ¿Hay algún impedimento que bloquee mi progreso o el del equipo?

**Cómo manejar el bug técnico de Ana:**

Rodrigo interviene a los 2 minutos: "Ana, anotamos ese bloqueo. ¿Alguien
puede quedarse 10 minutos después del Daily para ayudarla?" — No se resuelve
en el Daily; se coordina quién lo resuelve y cuándo.

**Cómo manejar el servidor de staging:**

Rodrigo anota el impedimento y lo escala INMEDIATAMENTE después del Daily
con TI y/o management. Debe reportar al equipo la resolución antes del
Daily del día siguiente. Si lleva 3+ días sin resolverse, es un impedimento
organizacional que el SM debe escalar a un nivel superior.

---

<!-- ============================================================ -->
<!-- SECCIÓN 3: Impedimentos — SOLUCIÓN                         -->
<!-- ============================================================ -->

## Sección 3: Tipos de impedimentos detectados

| Impedimento | Tipo | ¿Quién lo gestiona? |
|-------------|------|---------------------|
| Bug en parser JSON (Ana) | Técnico (interno al equipo) | Los Developers entre sí |
| Servidor de staging caído | Organizacional (externo al equipo) | Scrum Master escala |

**¿Por qué no resolver impedimentos en el Daily?**

El Daily tiene timebox de 15 minutos. Su propósito es sincronizar y planear
las próximas 24 horas, no resolver problemas. Resolver en el Daily excluye
a quienes no necesitan ese contexto, consume el time-box y genera la ilusión
de que el equipo "ya trabajó en ello" cuando realmente solo habló. La regla:
**identificar** en el Daily, **resolver** después del Daily.
