<!-- ============================================ -->
<!-- Semana 20: OKRs y Métricas de Valor        -->
<!-- Práctica 02 — Alineación Backlog ↔ OKRs   -->
<!-- solution/solucion.md                        -->
<!-- ============================================ -->

# Solución — Alineación Backlog ↔ OKRs: MediLink

---

<!-- ============================================ -->
<!-- PASO 1: Clasificación                       -->
<!-- ============================================ -->

| ID | User Story (resumen) | Alineación | KR relacionado | Justificación |
|----|----------------------|------------|----------------|---------------|
| US-031 | Confirmación automática de cita | **ALTA** | KR 1 | La confirmación automática elimina el tiempo de espera manual (4h → potencialmente minutos). Es la historia con mayor impacto directo en el KR 1. |
| US-032 | Cancelación 1 clic desde email | **ALTA** | KR 3 | Reducir la fricción para cancelar hace que el paciente cancele en vez de simplemente no asistir, lo que mejora la tasa de cancelaciones gestionadas y puede reducir el 22%. |
| US-033 | Exportar listado CSV para clínica | **BAJA** | Ninguno | Feature de administración interna de la clínica. Tiene valor de negocio para retener clínicas, pero no mueve ninguno de los 3 KRs orientados a la experiencia del paciente. |
| US-034 | Historial últimas 10 citas | **MEDIA** | KR 2 (NPS) | Mejora la percepción general del paciente y puede contribuir al NPS, pero no hay evidencia directa de que el historial sea un driver del NPS bajo. El impacto es indirecto. |
| US-035 | Búsqueda de médicos por especialidad y zona | **BAJA** | Ninguno activo | Feature de adquisición (nuevos pacientes), no de retención o reducción de fricciones en citas existentes. Puede ser prioridad en el próximo OKR, pero no en este Q3. |
| US-036 | Alerta a clínica si paciente no confirma en 30 min | **ALTA** | KR 1 + KR 3 | Permite a la clínica actuar en la ventana de 30 min, reduciendo el tiempo de confirmación (KR 1) y la tasa de cancelación tardía o no-show (contribuye a KR 3). |

---

<!-- ============================================ -->
<!-- PASO 2: Diagnóstico                         -->
<!-- ============================================ -->

**¿Qué patrón detectas en el Sprint 1–4 que explica la falta de mejora en el KR 1?**

El equipo ha entregado features que agregan información o conveniencia (historial, búsqueda,
exportación), pero ninguna ataca la causa raíz del tiempo de confirmación: el proceso manual
donde la clínica llama al paciente. El KR 1 requiere automatización del flujo de confirmación,
no más funcionalidades secundarias. El equipo mejoró el producto sin mover el outcome objetivo.

**¿Qué le diría Esteban al equipo en la Retrospectiva sobre la relación entre sus entregas y los KRs?**

Esteban plantearía: *"Hemos entregado con buena calidad cada sprint. Pero en 4 sprints el KR 1
bajó solo 10 minutos. Eso nos dice que nuestras elecciones de qué hacer no están conectadas con
lo que el OKR nos pide mover. En el Sprint Planning debemos preguntarnos: '¿este item, si lo
completamos, tiene probabilidad de mover KR 1, KR 2 o KR 3?'. Si la respuesta es no, hay que
evaluarlo."* La Retrospectiva debe generar como acción concreta un criterio de entrada al Sprint
Backlog alineado con los KRs activos.

**¿Cuál es la US del Sprint 5 con mayor potencial de mover el KR 1?**

**US-031** (confirmación automática). Elimina el paso humano que genera las 4 horas de espera.
Si el sistema confirma automáticamente cuando la clínica tiene disponibilidad, el tiempo colapsa
a minutos. US-036 es complementaria: actúa cuando la automación no es posible (paciente no
confirma), reduciendo la ventana de reacción a 30 minutos.

---

<!-- ============================================ -->
<!-- PASO 3: Sprint Goal reescrito               -->
<!-- ============================================ -->

**Sprint Goal del Sprint 5 — reescrito:**

> Para que los pacientes reciban confirmación de su cita en menos de 1 hora —en lugar de 4—,
> el equipo automatizará el flujo de confirmación y activará alertas de seguimiento para clínicas,
> avanzando el KR 1 de 3h 50min a menos de 2 horas al cierre del Sprint.

**Por qué funciona:**
- Dice el **beneficio para el usuario** (confirmación en < 1h)
- Nombra **qué hace el equipo** (automatizar flujo + alertas)
- Conecta con el **KR 1 específico** con un sub-target intermedio medible (< 2h)
- El equipo puede evaluar al final del sprint si lo logró o no

---

**US que deberían depriorizarse:**

| US | Razón para depriorizar |
|----|------------------------|
| US-033 — Exportar CSV para clínica | No mueve ningún KR del Q3 orientado al paciente. Puede hacerse en Q4 si la retención de clínicas se convierte en OKR. |
| US-035 — Búsqueda por especialidad y zona | Feature de adquisición (nada malo en sí), pero el equipo tiene capacidad limitada y los KRs activos son de retención y reducción de fricción, no de atracción de nuevos usuarios. |
| US-034 — Historial de citas | Contribución al NPS es indirecta y el NPS bajó 3 puntos. El equipo necesita atacar la causa raíz (time-to-confirm), no agregar features de conveniencia. Depriorizar hasta tener evidencia de que impacta el NPS. |
