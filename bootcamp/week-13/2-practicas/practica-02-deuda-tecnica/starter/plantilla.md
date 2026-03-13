<!-- ============================================ -->
<!-- PASO 1: Clasificar cada ítem de deuda      -->
<!-- Semana 13 — Deuda Técnica                   -->
<!-- ============================================ -->

## Clasificación de deuda técnica

Tipos disponibles: Deliberada / Involuntaria / Acumulada / Diseño

| ID   | Descripción breve                             | Tipo de deuda | Justificación |
| ---- | --------------------------------------------- | ------------- | ------------- |
| DT-01 | Auth sin tests, sin actualizar 6 meses       | <!-- -->      | <!-- -->      |
| DT-02 | PDF solo para tipo A (hardcodeado)            | <!-- -->      | <!-- -->      |
| DT-03 | Queries sin índices, 3–5 seg                  | <!-- -->      | <!-- -->      |
| DT-04 | Monolito que impide separar flujos            | <!-- -->      | <!-- -->      |

---

<!-- ============================================ -->
<!-- PASO 2: Cuantificar el impacto              -->
<!-- ============================================ -->

## Cuantificación del impacto

Traduce cada ítem a lenguaje de negocio. Usa: usuarios afectados, velocidad
perdida, riesgo de seguridad, costo de corregir hoy vs. en 6 meses, etc.

**DT-01 — Auth sin tests:**

<!-- ¿Qué riesgo representa para los usuarios y el producto? -->
<!-- Tu respuesta aquí -->

**DT-02 — PDF solo tipo A:**

<!-- ¿Cuántos usuarios están bloqueados? ¿Por qué no puede esperar? -->
<!-- Tu respuesta aquí -->

**DT-03 — Queries lentas:**

<!-- ¿Qué impacto tiene en la experiencia? ¿Qué ocurre si crece el número de usuarios? -->
<!-- Tu respuesta aquí -->

**DT-04 — Monolito:**

<!-- ¿En qué punto bloquea el desarrollo? ¿Qué features futura dependen de esto? -->
<!-- Tu respuesta aquí -->

---

<!-- ============================================ -->
<!-- PASO 3: Propuesta de negociación            -->
<!-- ============================================ -->

## Propuesta de Beatriz a Catalina

**Capacidad estimada del Sprint 7**: ~38 puntos

**Aplicando la regla del 20%:**

<!-- ¿Cuántos puntos se reservan para deuda técnica? -->
Puntos para nuevas features: <!-- -->
Puntos para deuda técnica: <!-- -->

**¿Qué ítems incluir en el Sprint con esa capacidad?**

<!-- Ordena los ítems de mayor a menor prioridad (impacto × urgencia) -->
<!-- y selecciona cuáles entran en el 20% -->

| Prioridad | ID   | Estimación (pts) | ¿Entra en Sprint 7? |
| --------- | ---- | ---------------- | ------------------- |
| 1         | <!-- --> | <!-- -->      | <!-- -->            |
| 2         | <!-- --> | <!-- -->      | <!-- -->            |
| 3         | <!-- --> | <!-- -->      | <!-- -->            |
| 4         | <!-- --> | <!-- -->      | <!-- -->            |

**Argumento clave para Catalina (máx. 3 oraciones):**

<!-- ¿Cómo presenta Beatriz la decisión en términos de valor y riesgo para el producto? -->
<!-- Tu respuesta aquí -->

---

<!-- ============================================ -->
<!-- PASO 4: Enabler Stories en el Backlog      -->
<!-- ============================================ -->

## Backlog de Enabler Stories

Escribe mínimo 2 Enabler Stories para los ítems de mayor prioridad.
Formato: `Como equipo de desarrollo, quiero [acción] para [beneficio técnico/negocio]`

**Enabler 1 (para DT-__):**

Como equipo de desarrollo, quiero <!-- -->
para <!-- -->

**Criterio de aceptación:**
- Dado <!-- -->
  Cuando <!-- -->
  Entonces <!-- -->

---

**Enabler 2 (para DT-__):**

Como equipo de desarrollo, quiero <!-- -->
para <!-- -->

**Criterio de aceptación:**
- Dado <!-- -->
  Cuando <!-- -->
  Entonces <!-- -->
