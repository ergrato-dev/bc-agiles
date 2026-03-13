<!-- Semana 19: Práctica 01 — SOLUCIÓN -->
<!-- CityConnect: plataforma de participación ciudadana -->

<!-- ============================================ -->
<!-- PASO 1: Antipatrones — SOLUCIÓN            -->
<!-- ============================================ -->

**Antipatrón 1: Feature branches de larga duración**
Ana trabajó 3 días sin integrar. Los feature branches de larga duración son
la causa raíz del "integration hell". La solución es integrar al menos 1 vez al día
(práctica CI: "trunk-based development" o branches cortas de máximo 1 día).

**Antipatrón 2: Desconectar módulos para evitar conflictos**
Carlos desconectó el módulo de reportes para no conflictuar. Esta práctica aumenta
la deuda técnica: cuanto más se pospone la integración, peor es el conflicto.
Es el síntoma más directo del "integration hell".

**Antipatrón 3: Pipeline lento que se evita ejecutar**
Un pipeline de 40 minutos no cumple su propósito — el equipo lo evita porque
interrumpe el flujo. El standard DevOps es un pipeline de **máximo 10–15 minutos**
para que sea ejecutable en cada commit sin frustrar al equipo.

---

<!-- ============================================ -->
<!-- PASO 2: Pipeline — SOLUCIÓN                -->
<!-- ============================================ -->

| Etapa | Momento del Sprint | Tiempo máximo | Si falla... |
| ----- | ------------------ | ------------- | ----------- |
| Build | Cada commit (días 1–10) | 2 min | Bloquea el merge — nadie integra hasta que pase |
| Unit Tests | Cada commit | 5 min | Bloquea — el developer corrige antes de pushear |
| Integration Tests | Al menos 2x/día | 5 min | Se asigna a quien rompió el build para corregir en < 30 min |
| Static Analysis | Cada commit | 2 min | Falla informativa — no bloquea pero se registra en el backlog técnico |
| Deploy a Staging | Al finalizar el día (automático) | 5 min | El SM notifica al equipo para revisar el log antes del siguiente Daily |

> **Tiempo total pipeline ideal**: ~14 minutos. Ejecutable en cada commit.

---

<!-- ============================================ -->
<!-- PASO 3: DoD actualizada — SOLUCIÓN         -->
<!-- ============================================ -->

**DoD actualizada — criterios nuevos:**

1. **El pipeline CI está en verde**: build, unit tests e integration tests pasan
   sin errores en el branch integrado a main/trunk

2. **La historia está desplegada en staging**: el código está disponible en el
   entorno de staging para que Andrés y el PO puedan verlo antes de la Sprint Review

3. **Cobertura de tests ≥ 70%**: los criterios de aceptación tienen al menos
   1 test automatizado (unitario o de integración) que los verifica
