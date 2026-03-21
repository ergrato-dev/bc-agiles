<!-- ============================================ -->
<!-- PASO 1: Clasificar cada situación — SOLUCIÓN -->
<!-- ============================================ -->

## Clasificación de situaciones

| # | Descripción breve                          | Tipo                  | Justificación |
| - | ------------------------------------------ | --------------------- | ------------- |
| 1 | Sin acceso al entorno de pruebas (Infra)   | **Impedimento**       | El equipo no puede solucionarlo solo; depende de un área externa. Bloquea tareas del Sprint. |
| 2 | Bug en librería de mapas v3.2              | **Obstáculo**         | El equipo puede resolverlo aplicando un workaround o migrando a v3.3. No requiere intervención externa. |
| 3 | Estimaciones siempre optimistas            | **Problema de proceso** | No bloquea el Sprint actual; es un patrón recurrente. Se trabaja en retrospectiva. |
| 4 | PO aceptó scope externo sin avisar         | **Impedimento**       | Amenaza el Sprint Goal acordado. Carlos debe actuar para proteger el acuerdo del equipo. |
| 5 | Sin respuesta del área legal               | **Impedimento**       | Marco lleva 2 días esperando. No puede avanzar solo. El Sprint Goal está en riesgo. |

---

<!-- ============================================ -->
<!-- PASO 2: Acción de Carlos por situación — SOLUCIÓN -->
<!-- ============================================ -->

## Acción de Carlos como SM

**Situación 1 — Acceso denegado por Infra:**

**Nivel 2**. Carlos contacta directamente al líder de Infraestructura hoy mismo.
No espera: el acceso es una dependencia crítica para entregar el Sprint Goal.
Registra en ROAM como **Owned** con owner = Carlos.

**Situación 2 — Bug en librería:**

Carlos **no actúa** directamente. Es un obstáculo técnico que el equipo puede resolver.
Valida en el Daily que Tomás tiene un plan (workaround o upgrade a v3.3) y que no necesita
de Carlos para desbloquearse. Si el equipo tardara más de un día, entonces reevalúa.

**Situación 3 — Estimaciones optimistas:**

No es urgente para este Sprint. Carlos lo anota como tema de retrospectiva.
Si el patrón ya existe desde los últimos 3 Sprints, propone también una sesión de calibración
de estimaciones antes del próximo Sprint Planning.

**Situación 4 — Scope creep aceptado por PO:**

Carlos habla con Valeria (PO) después del Daily, sin el equipo presente.
Le recuerda que el Sprint Goal fue acordado y que agregar US-47 sin negociación
viola el acuerdo del Sprint. Propone tres opciones: (a) posponer US-47 al próximo
Sprint, (b) eliminar otra historia de igual o mayor tamaño, (c) renegociar el Sprint
Goal con el equipo de forma explícita. Registra en ROAM como **Owned** = Carlos.

**Situación 5 — Espera del área legal:**

Marco lleva 2 días bloqueado: ya es **Nivel 2** desde ayer.
Carlos usa datos en el escalamiento: "Marco lleva 2 días sin respuesta. Faltan 5 días
para el fin del Sprint. Sin la aprobación legal, no podemos activar el módulo de rutas
de emisiones, que es el Sprint Goal." Registra en ROAM como **Mitigated** o **Accepted**
según resolución; mientras tanto, reasigna a Marco a preparar tests de integración.

---

<!-- ============================================ -->
<!-- PASO 3: Registro ROAM del Sprint — SOLUCIÓN -->
<!-- ============================================ -->

## Registro ROAM — Sprint 6 · Día 5

| Impedimento                     | Owner  | Nivel | Estado ROAM | Acción concreta                        | Fecha resolución esperada |
| ------------------------------- | ------ | ----- | ----------- | -------------------------------------- | ------------------------- |
| Sin acceso entorno pruebas Infra | Carlos | 2     | Owned       | Contactar líder Infra hoy               | Día 6                     |
| Scope creep US-47 sin negociar  | Carlos | 1     | Owned       | Reunión con Valeria post-Daily          | Hoy                       |
| Espera aprobación legal (Marco) | Carlos | 2     | Mitigated   | Escalar a dirección; Marco en tests     | Día 7                     |
