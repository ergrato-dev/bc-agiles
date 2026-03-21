<!-- ============================================ -->
<!-- PASO 1: Qué demostrar — SOLUCIÓN           -->
<!-- ============================================ -->

## Decisión de Daniela: ¿qué se demuestra?

| US | ¿Se demuestra? | Justificación |
| -- | -------------- | ------------- |
| US-45 | ✅ Sí | DoD cumplida. Es parte del Sprint Goal (panel de seguimiento en tiempo real). |
| US-46 | ✅ Sí | DoD cumplida. Los estados son el núcleo del value prometido a los ciudadanos. |
| US-47 | ❌ No | No tiene DoD cumplida. Mostrarla engaña a los stakeholders sobre el estado real. |
| US-48 | ✅ Sí | DoD cumplida. Aporta contexto al panel de seguimiento. |

**Cómo explica Daniela que US-47 no se demuestra:**

> "El mapa por zona era parte del plan original, pero encontramos una dependencia
> con el proveedor de cartografía que nos tomó más tiempo del esperado.
> Los 3 ítems que sí vamos a mostrar cubren el Sprint Goal principal: el ciudadano
> ya puede ver el estado de su reporte sin llamar al municipio. US-47 entra
> como prioridad 1 en el próximo Sprint."

---

<!-- ============================================ -->
<!-- PASO 2: Feedback clasificado — SOLUCIÓN    -->
<!-- ============================================ -->

## Clasificación del feedback

| Stakeholder | Comentario (resumen) | Tipo | Acción en backlog |
| ----------- | -------------------- | ---- | ----------------- |
| Marcos | Panel de operarios por sector | **Nuevo requerimiento** | Crear US-N1 con estimación y prioridad |
| Claudia | Notificación WhatsApp al cerrar | **Nuevo requerimiento** | Crear US-N2; prioridad alta por impacto en retención |
| Pablo | Traducir estados a lenguaje ciudadano | **Ajuste a existente** | Refinar US-46: cambiar textos "In Progress" → "En camino" |
| Claudia | Versión mobile | **Fuera de scope** | Registrar en backlog como iniciativa futura; no comprometerse en Sprint 6 |

---

<!-- ============================================ -->
<!-- PASO 3: Backlog actualizado — SOLUCIÓN     -->
<!-- ============================================ -->

## Backlog actualizado después de la Review

| ID    | Título                                    | Prioridad | Pts  | Origen |
| ----- | ----------------------------------------- | --------- | ---- | ------ |
| US-47 | Mapa interactivo de reportes por zona    | **1**     | 8    | Plan anterior |
| US-N1 | Panel de operarios con filtro por sector | **2**     | 8    | Feedback Marcos |
| US-N2 | Notificación WhatsApp al cerrar reporte  | **3**     | 5    | Feedback Claudia |
| US-46* | *(Ajuste)* Textos de estado en lenguaje ciudadano | **4** | 1 | Feedback Pablo |
| US-49 | Panel de administrador municipal         | **5**     | 13   | Plan anterior (baja prioridad) |
| US-50 | Exportación de reportes a CSV            | **6**     | 5    | Plan anterior |
| US-EPIC | Versión mobile (iniciativa futura)    | —         | TBD  | Feedback Claudia |

**Cambio más relevante que generó la Review:**

El panel de operarios por sector (US-N1) no existía en el backlog y se convirtió
en prioridad 2 inmediata, por encima de features ya planificadas como US-49.
Esto demuestra que el Sprint Review no es una formalidad: cambió el orden
de trabajo del equipo para los próximos 2 Sprints con un solo input de Marcos.
