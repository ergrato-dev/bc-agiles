<!-- Semana 01: Del Cascada al Ágil -->
<!-- Práctica 01 — SOLUCIÓN -->

<!-- ============================================ -->
<!-- PASO 1: Resumen del fracaso — SOLUCIÓN      -->
<!-- ============================================ -->

**¿Por qué falló este proyecto?**

El sistema falló porque los requisitos se congelaron en el mes 3 con
información incompleta (solo 5 de 47 oficinas). El cliente no tuvo
visibilidad del producto hasta el mes 15, cuando ya era demasiado
tarde para cambios estructurales. El contrato incentivó "entregar"
sobre "entregar valor real".

---

<!-- ============================================ -->
<!-- PASO 2: Fases del cascada identificadas     -->
<!-- ============================================ -->

| Problema detectado                                      | Fase del cascada  |
| ------------------------------------------------------- | ----------------- |
| El cliente no participó en decisiones de arquitectura   | Diseño            |
| No se validó conectividad en oficinas regionales        | Requisitos        |
| El cliente vio el producto por primera vez en el mes 15 | Verificación      |
| Los reportes no eran compatibles con el entorno real    | Requisitos/Diseño |

---

<!-- ============================================ -->
<!-- PASO 3: Señales de alerta ignoradas         -->
<!-- ============================================ -->

**Señal 1:**
Solo se relevaron 5 de las 47 oficinas. La muestra era del 10% del
universo real. Los requisitos no representaban la realidad operativa.

**Señal 2:**
El cliente recibía avances en porcentajes abstractos ("80% completado")
sin ver funcionalidades reales. Un porcentaje no es una demo.

**Señal 3:**
La infraestructura de conectividad nunca se validó en campo. Asumir
Internet estable en oficinas regionales fue una decisión sin datos.

---

<!-- ============================================ -->
<!-- PASO 4: ¿Qué habría cambiado con ágil?     -->
<!-- ============================================ -->

**Entregas incrementales (Sprints):**
Con Sprints de 2 semanas, el cliente habría visto funcionalidades reales
desde el primer mes. Los problemas de interfaz y conectividad habrían
emergido en el Sprint 2 o 3, no en el mes 15.

**Participación continua del cliente:**
Un Product Owner del Ministerio en el equipo habría garantizado que las
decisiones de diseño reflejaran la realidad operativa de las 47 oficinas.

**Validación temprana con usuarios reales:**
Pilotear el sistema con 2 o 3 funcionarios reales en el Sprint 1 habría
expuesto el problema de las colas presenciales antes de construir todo
el sistema sobre un supuesto incorrecto.
