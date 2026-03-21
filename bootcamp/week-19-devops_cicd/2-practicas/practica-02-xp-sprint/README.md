# Práctica 02 — Prácticas XP para Mejorar la Calidad en el Sprint

## Escenario: GreenField — Sistema de gestión de áreas verdes urbanas

**GreenField** administra el mantenimiento de parques y plazas de una ciudad.
El equipo Scrum de 5 personas lleva 6 meses trabajando juntos.

La Product Owner **Valeria** se queja de que hay bugs en producción cada 2–3 Sprints.
El Scrum Master **Miguel** sospecha que falta disciplina técnica: no hay tests
y el código legacy del módulo de inspecciones es frágil.

---

### Paso 1: TDD en la User Story actual

El equipo está trabajando en esta historia:

> **US-047: Programar inspección periódica**  
> Como **coordinador de mantenimiento** quiero **programar inspecciones recurrentes**
> para que **nunca se nos pase revisar un parque por más de 30 días**.
>
> **Criterios de aceptación:**
> - CA-1: Si el parque no tuvo inspección en 30 días, el sistema genera alerta automática
> - CA-2: El coordinador puede configurar la frecuencia (7, 14 o 30 días) por parque
> - CA-3: Si el Inspector está de vacaciones, el sistema reasigna automáticamente

**Escribe 3 tests TDD** para esta historia — uno por cada criterio de aceptación.
Usa pseudocódigo o el lenguaje que prefieras.

---

### Paso 2: Pair Programming en el módulo legacy

Miguel quiere usar Pair Programming para el módulo de inspecciones legacy.
El equipo tiene 3 desarrolladores disponibles: **Jair** (senior, conoce el legacy),
**Priya** (junior, fuerte en tests) y **Tomás** (mid, no conoce el módulo).

**Propón el mejor par** para trabajar en el módulo legacy y justifica por qué.

---

### Paso 3: Refactoring como parte de la DoD

La DoD actual no incluye refactoring. Valeria objeta: "Si refactorizamos, tardamos más."

**Escribe la respuesta de Miguel** para convencer a Valeria de incluir refactoring
en la DoD, usando un argumento concreto de negocio (no técnico).

**Abre `starter/plantilla.md`** y completa los 3 pasos.
