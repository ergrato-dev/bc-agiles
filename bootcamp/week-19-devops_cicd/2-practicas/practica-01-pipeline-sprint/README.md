# Práctica 01 — Pipeline CI/CD en el Sprint

## Escenario: CityConnect — Plataforma de participación ciudadana

**CityConnect** permite a los ciudadanos reportar incidentes urbanos (baches, alumbrado, basura).
El equipo tiene 6 desarrolladores y lleva 4 Sprints.

El Scrum Master **Andrés** detectó un patrón preocupante en los últimos 2 Sprints:

> "Todos los Sprints terminan con integración caótica el último día.
> El pipeline falla, hay conflictos de merge y la Sprint Review se hace con
> código que no pasó los tests de integración."

---

### Paso 1: Diagnóstico del antipatrón

Lee el diálogo del equipo en el Daily del Día 9 del Sprint:

> **Ana (dev)**: "Mergé mi feature branch de pagos — había 3 días desde el último merge."  
> **Carlos (dev)**: "Yo tenía el módulo de reportes desconectado toda la semana para no conflictuar."  
> **Laura (dev)**: "El pipeline tarda 40 minutos. No lo corro seguido porque interrumpe el flujo."  
> **Andrés (SM)**: "Mañana es la Review y el build está roto…"

**Identifica los 3 antipatrones de CI/CD presentes en este diálogo.**

---

### Paso 2: Proponer el pipeline

Andrés quiere proponer al equipo un pipeline CI/CD básico que se ejecute en cada commit.
Las etapas disponibles son:

```
Build → Unit Tests → Integration Tests → Static Analysis → Deploy a Staging
```

**Para cada etapa:**
1. ¿En qué momento del Sprint ocurre?
2. ¿Cuánto tiempo máximo debería tomar?
3. ¿Qué pasa si falla?

---

### Paso 3: Actualizar la DoD

La DoD actual del equipo dice:
- La funcionalidad cumple los criterios de aceptación
- El código fue revisado en peer review
- No hay bugs conocidos

**Añade 3 criterios DevOps a esta DoD** para que refleje las prácticas CI/CD.

**Abre `starter/plantilla.md`** y completa los 3 pasos.
