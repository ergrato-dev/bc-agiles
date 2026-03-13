<!-- Semana 02: Los 12 Principios Ágiles -->
<!-- Práctica 02 — Solución de referencia -->

# Práctica 02 — Solución

---

<!-- ============================================ -->
<!-- PASO 1: Nombres de antipatrones — SOLUCIÓN  -->
<!-- ============================================ -->

| Situación | Nombre del antipatrón |
| --------- | --------------------- |
| 1 | **Micromanagement / Command & Control Scrum** |
| 2 | **Big Bang Deployment / Mini-cascada** |
| 3 | **Scrum Zombie / Ceremonias vacías** |
| 4 | **Crunch culture / Ritmo insostenible** |
| 5 | **Deuda técnica intencional / Ágil sin ingeniería** |

---

<!-- ============================================ -->
<!-- PASO 2: Principios violados — SOLUCIÓN      -->
<!-- ============================================ -->

| Situación | Principio violado | Explicación |
| --------- | ----------------- | ----------- |
| 1 | **P11** | Los equipos ágiles son autoorganizados; quién hace qué lo decide el equipo, no el jefe |
| 2 | **P3 + P7** | Las entregas frecuentes de software funcionando (no batch al final) son la medida de progreso |
| 3 | **P12** | Las retrospectivas deben producir ajustes reales. Sin cambio, no hay mejora continua |
| 4 | **P8** | Los procesos ágiles promueven el desarrollo sostenible a ritmo constante indefinidamente |
| 5 | **P9** | La atención continua a la excelencia técnica y al buen diseño es lo que mantiene la agilidad |

---

<!-- ============================================ -->
<!-- PASO 3: Acciones de mejora — SOLUCIÓN       -->
<!-- ============================================ -->

**Situación 1:**
En el próximo Sprint Planning, el Scrum Master facilita que el equipo proponga
cómo dividir las User Stories en tareas. El Jefe de Proyecto escucha pero no
asigna. Después del Sprint se comparan resultados con el Sprint anterior.

**Situación 2:**
Introducir el concepto de "Pipeline de despliegue continuo": cada historia
completada se despliega en un entorno de staging visible para el PO.
Para el Sprint 2, al menos 1 funcionalidad estará disponible a mitad del Sprint.

**Situación 3:**
Cambiar el formato de la Retrospectiva: al cierre de cada retro se escribe
UN solo compromiso de mejora en el tablero con nombre del responsable y
fecha de revisión. Al inicio del siguiente Sprint se verifica si se cumplió.

**Situación 4:**
El Scrum Master expone el costo real del crunch: calidad de código, bugs
introducidos por fatiga, rotación de talento. Propone que el velocity
se mida sobre trabajo sostenible. Introduce la capacidad real del equipo
en el Sprint Planning (40h/persona, no 60h).

**Situación 5:**
Agregar como ítem de Definition of Done: "mínimo 1 test unitario por caso
de negocio crítico". No es opcional. Si el Sprint termina sin ese test,
la historia no está Done.

---

<!-- ============================================ -->
<!-- PASO 4: Priorización — SOLUCIÓN             -->
<!-- ============================================ -->

**Situación elegida:** **3 (Retrospectivas sin acciones)**

**Justificación:**
La Retrospectiva es el mecanismo de mejora continua del equipo. Si no produce
cambios, el equipo no tiene capacidad de autocorrección. Corregir esto primero
crea el hábito de mejora que permitirá resolver las otras 4 situaciones en
retrospectivas futuras. Es la "palanca" que mueve todas las demás.

*Nota: También es válido elegir la Situación 1 si se argumenta que el
micromanagement bloquea estructuralmente el resto de mejoras.*
