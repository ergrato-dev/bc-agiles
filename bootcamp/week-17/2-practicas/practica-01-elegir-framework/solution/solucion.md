<!-- Semana 17: Práctica 01 — SOLUCIÓN -->
<!-- GovTrack: plataforma tributaria municipal  -->

<!-- ============================================ -->
<!-- PASO 1: Elección de framework — SOLUCIÓN   -->
<!-- ============================================ -->

**¿Cuál framework eliges para GovTrack?**

**LeSS** (o Nexus como segunda opción válida).

**Justificación:**

1. Solo 3 equipos (22 personas) — SAFe está diseñado para 5–125+ equipos.
   Implementar SAFe aquí es exceso de proceso.

2. El equipo actual ya domina Scrum (Sprint Reviews y Retros efectivas).
   LeSS requiere que los equipos dominen Scrum antes de escalar — condición cumplida.

3. Un único Product Backlog gestionado por Sofía encaja perfectamente con el
   modelo de LeSS (1 PO, 1 Product Backlog compartido, mismo Sprint).

4. No hay restricciones regulatorias que justifiquen el overhead de PI Planning
   o el Program Backlog complejo de SAFe.

> Nexus también es válido. La diferencia es que LeSS impone menos capas y es
> más puramente "Scrum escalado". Nexus añade el NIT, útil si hay muchas
> dependencias técnicas entre equipos.

---

<!-- ============================================ -->
<!-- PASO 2: Antipatrones — SOLUCIÓN            -->
<!-- ============================================ -->

**Error 1: Dividir el backlog en 3 Program Backlogs**

En LeSS (y en Scrum en general), un único Product Backlog es fundamental.
Dividirlo crea silos: cada equipo optimiza su parte sin visión del producto completo.
Sofía perdería autoridad y visibilidad sobre el producto total.

**Error 2: Contratar un RTE externo sin madurez en SAFe**

El RTE requiere que todos los equipos entiendan SAFe y los PI Objectives.
Si los equipos no tienen esta base, el RTE se convierte en un Project Manager
clásico que asigna tareas — antipatrón explícito en SAFe.

**Error 3: PI Planning "el próximo mes" sin preparación**

Un PI Planning efectivo requiere semanas de preparación: Program Backlog refinado,
Features definidas, System Demos establecidas, herramientas configuradas.
Saltarse esta preparación convierte el PI Planning en una reunión decorativa.

---

<!-- ============================================ -->
<!-- PASO 3: Propuesta alternativa — SOLUCIÓN   -->
<!-- ============================================ -->

**Andrea responde:**

"Mauricio, entiendo que quieres escalar rápido. Mi recomendación es usar **LeSS**
porque GovTrack tiene 3 equipos y Sofía ya gestiona el backlog eficientemente.

Las diferencias clave con SAFe son:
1. LeSS no requiere PI Planning de 2 días ni rol de RTE — reducimos overhead desde el día 1
2. Los 3 equipos comparten el mismo Sprint y misma Sprint Review, lo que
   mantiene la visión unificada del producto que Sofía ya tiene

El primer paso concreto es: hacer un Sprint conjunto de adaptación donde los
3 equipos acuerdan cómo dividir el trabajo en el Refinement compartido,
manteniendo 1 solo Sprint Goal orientado al producto completo."
