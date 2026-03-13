# 02 — DoD, DoR y Transparencia

## Objetivos

- Redactar una Definition of Done con criterios verificables
- Distinguir la DoD de la Definition of Ready
- Entender cómo los compromisos aumentan la transparencia

---

## 1. Definition of Done (DoD)

La DoD es el acuerdo del equipo sobre qué significa que un trabajo esté
**completamente terminado**. No es una lista de "pasos de QA" — es el
estándar de entrega que aplica a TODO ítem del Incremento.

**Ejemplo de DoD de un equipo de software:**

| Criterio | Verificable |
| -------- | ----------- |
| Código revisado por al menos 1 peer | ✅ |
| Tests unitarios con cobertura ≥80% | ✅ |
| Desplegado en staging sin errores | ✅ |
| Documentación de API actualizada | ✅ |
| Aprobado en Acceptance Testing | ✅ |

**Lo que NO es un criterio buen de DoD:**
- ❌ "El código funciona bien" (subjetivo)
- ❌ "El equipo está satisfecho" (no verificable)
- ❌ "El PO lo aprobó" (la DoD es del equipo, no del PO)

---

## 2. Definition of Ready (DoR)

La DoR define cuándo un ítem del Product Backlog está **listo para
entrar al Sprint Planning**. Es un criterio de entrada, no de salida.

**Ejemplo de DoR:**

- La User Story está en formato: Como / Quiero / Para
- Tiene criterios de aceptación verificables
- Está estimada (en puntos o T-shirt)
- No tiene dependencias bloqueantes con otros ítems
- El diseño de UX está disponible (si aplica)

**Trampa frecuente**: usar la DoR para "pre-aprobar" trabajo y saltarse
el refinamiento → el Backlog Refinement es el espacio para llegar a DoR.

---

## 3. Transparencia: el propósito real de los artefactos

Los artefactos de Scrum existen para crear **transparencia**. Sin
transparencia, la inspección es inútil y la adaptación imposible.

| Artefacto | Sin transparencia | Con transparencia |
| --------- | ----------------- | ----------------- |
| Product Backlog | Nadie sabe qué viene después | Prioridad visible para todos |
| Sprint Backlog | El equipo no sabe si va a lograr el Sprint Goal | Progreso visible diariamente |
| Incremento | No se sabe qué está "hecho" | La DoD define el estándar |

---

## Checklist de Comprensión

- ¿Puedo escribir una DoD con 5 criterios verificables para mi dominio?
- ¿Entiendo la diferencia entre DoD (salida) y DoR (entrada)?
- ¿Sé por qué "aprobado por el PO" NO es un criterio de la DoD?
- ¿Comprendo cómo la falta de DoD destruye la transparencia del Incremento?

---

## Referencias

- Scrum Guide 2020: https://scrumguides.org/ (sección "Commitments")
- Scrum.org — DoD: https://www.scrum.org/resources/blog/done-understanding-definition-done
