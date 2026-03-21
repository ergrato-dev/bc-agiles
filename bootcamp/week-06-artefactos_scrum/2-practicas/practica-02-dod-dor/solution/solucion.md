<!-- Semana 06: Artefactos de Scrum -->
<!-- Práctica 02: DoD y DoR — SOLUCIÓN -->

# Solución — Definition of Done y Definition of Ready

---

## Sección 1: Diagnóstico

| # | Criterio | Estado | Por qué |
|---|----------|--------|---------|
| 1 | El código compila sin errores | **Mejorar** | Necesario pero insuficiente; reescribir: "Build de CI/CD exitoso sin warnings críticos" |
| 2 | El dev lo probó en su máquina | **Eliminar** | Solo funcionar en local no es suficiente; sustituir por "probado en staging" |
| 3 | El PO dice que está bien | **Eliminar** | La DoD es del equipo; la aprobación del PO es Acceptance Testing, no DoD |
| 4 | Tiene comentarios en el código | **Mejorar** | Vago; reescribir: "Funciones públicas documentadas con descripción y parámetros" |
| 5 | Fue a staging | **Válido** | Verificable y crítico para UrbanTrack |
| 6 | Se ve bonito | **Eliminar** | Completamente subjetivo e inverificable |
| 7 | El equipo está satisfecho | **Eliminar** | Subjetivo; no puede ser criterio de entrega |
| 8 | Subido al repositorio | **Mejorar** | Reescribir: "Código mergeado a rama principal vía Pull Request aprobado" |
| 9 | Tests de unidad escritos | **Mejorar** | Reescribir: "Cobertura de tests unitarios ≥75%" |
| 10 | No tiene bugs conocidos | **Mejorar** | Reescribir: "Ningún bug de severidad Alta o Crítica abierto" |

---

## Sección 2: DoD mejorada para UrbanTrack

| # | Criterio | ¿Cómo se verifica? |
|---|----------|--------------------|
| 1 | Build de CI/CD exitoso sin warnings críticos | Reporte automático del pipeline |
| 2 | Cobertura de tests unitarios ≥75% | Reporte de cobertura en el pipeline |
| 3 | Desplegado en staging sin errores de consola | QA ejecuta smoke test en staging |
| 4 | Pull Request aprobado por ≥1 peer review | GitHub/GitLab muestra aprobación |
| 5 | Acceptance criteria verificados por QA | Checklist firmado por QA antes del Sprint Review |

---

## Sección 3: Definition of Ready + evaluación

**5 criterios de DoR del equipo UrbanTrack:**

1. La User Story sigue formato: Como / Quiero / Para
2. Tiene al menos 2 criterios de aceptación en formato Gherkin
3. Está estimada en Story Points por el equipo
4. No tiene dependencias bloqueantes pendientes
5. El diseño de pantalla (si aplica) está disponible y aprobado

**Evaluación:**

| Ítem | ¿Cumple? | Faltante |
|------|----------|----------|
| US-A: "Mejorar pantalla de rutas" | **No** | Sin formato US, sin CA, sin estimación, sin diseño |
| US-B: Historia conductor (CA + estimación) | **Parcial** | Cumple formato y estimación; falta verificar dependencias y diseño aprobado |
| US-C: "Integración con GPS" | **No** | Sin CA, sin estimación, sin diseño, posible dependencia de proveedor GPS |
