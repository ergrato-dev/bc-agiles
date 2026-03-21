# 01 — Impedimentos: Identificación y Escalación

## Objetivo

Distinguir tipos de impedimentos y aplicar el proceso de escalación adecuado.

---

## 1. Impedimento vs. Obstáculo vs. Problema del equipo

| Tipo | Definición | Ejemplo | ¿Quién lo resuelve? |
| ---- | ---------- | ------- | -------------------- |
| **Impedimento** | Bloquea el progreso del equipo y está **fuera del control del equipo** | El servidor de staging lleva 2 días caído y depende de Infra (otro equipo) | SM escala externamente |
| **Obstáculo** | Dificulta pero **el equipo puede resolverlo solo** | La librería que usan tiene un bug conocido — hay que parchearla | Equipo lo gestiona internamente |
| **Problema de proceso** | El equipo trabaja de forma ineficiente | El Daily Scrum dura 45 minutos | SM facilita la mejora |

> La clave: si el equipo puede resolverlo en el mismo Sprint sin ayuda externa, no es un impedimento. El SM solo interviene en impedimentos.

---

## 2. El proceso de escalación en 3 niveles

**Nivel 1 — Equipo resuelve** (1–2 días):
El SM identifica el bloqueo en el Daily. El equipo intenta resolverlo.
Si en 1 día no hay avance → Nivel 2.

**Nivel 2 — SM escala internamente** (2–3 días):
El SM habla con el área responsable (Infra, Legal, HR, otro equipo).
Documenta el bloqueo y su impacto en el Sprint. Si no hay resolución → Nivel 3.

**Nivel 3 — SM escala a liderazgo** (inmediato si amenaza el Sprint Goal):
El SM escala al Product Owner, Gerencia o Director de Tecnología según el contexto.
Presenta el impacto en datos: "llevamos X días bloqueados, el Sprint Goal está en riesgo."

---

## 3. Registro ROAM

Técnica para registrar y dar follow-up a impedimentos en el Sprint:

| Estado | Significado |
| ------ | ----------- |
| **R**esuelto | El impedimento fue eliminado |
| **O**wned | Alguien es responsable de resolverlo (con fecha) |
| **A**ccepted | El equipo lo acepta como restricción temporal |
| **M**itigated | No se eliminó pero se redujo su impacto |

---

## Checklist

- [ ] ¿Tienes el registro de impedimentos visible para todo el equipo?
- [ ] ¿Cada impedimento tiene un Owner y una fecha de resolución esperada?
- [ ] ¿Escalaste antes del Día 3 los impedimentos del Sprint actual?
- [ ] ¿Diferencias los impedimentos de los obstáculos que el equipo resuelve solo?
