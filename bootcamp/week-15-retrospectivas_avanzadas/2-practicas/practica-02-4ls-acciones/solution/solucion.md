<!-- ============================================ -->
<!-- PASO 1: Tablero 4Ls — SOLUCIÓN             -->
<!-- ============================================ -->

## Tablero 4Ls — Sprint 7

**Liked (gustó):**

- El Daily Scrum se mantuvo en < 20 min durante todo el Sprint (acción del Sprint 5 cumplida).
- El flujo de aprobación básico quedó funcionando y Carmen lo probó desde el día 8.
- La comunicación dentro del equipo de devs fue fluida; no hubo bloqueos internos.

**Learned (aprendimos):**

- Las zonas horarias no estaban en los criterios de aceptación del scheduler → aprendimos que necesitamos criterios más exhaustivos para modules con lógica temporal.
- Las dependencias con equipos externos no se pueden descubrir durante el Sprint; deben identificarse en el Refinement.

**Lacked (faltó):**

- Cobertura de tests para el módulo de scheduling (bugs en producción lo evidencian).
- Un proceso de coordinación con el equipo de diseño antes del Sprint.
- Tiempo para completar la vista de calendario (subestimamos la complejidad).

**Longed for (quisiéramos):**

- Un ambiente de staging más parecido a producción para detectar bugs de concurrencia.
- Un checklist explícito en la DoD que incluya tests de integración para cada módulo nuevo.

---

<!-- ============================================ -->
<!-- PASO 2: 5 Whys — SOLUCIÓN                  -->
<!-- ============================================ -->

## Problema 1: 3 bugs en producción

| # | ¿Por qué? |
| - | --------- |
| Why 1 | Los bugs llegaron a producción sin ser detectados por QA |
| Why 2 | QA no tenía casos de prueba para zonas horarias ni concurrencia |
| Why 3 | Los criterios de aceptación de las historias no incluían esos escenarios |
| Why 4 | El Refinement no tiene un paso de revisión de edge cases técnicos |
| Why 5 (causa raíz) | **La DoD del equipo no exige tests de integración para módulos nuevos** |

---

## Problema 2: Historia bloqueada por Diseño

| # | ¿Por qué? |
| - | --------- |
| Why 1 | US-67 estuvo bloqueada 3 días porque el equipo de diseño no entregó a tiempo |
| Why 2 | El equipo de diseño no sabía que eran una dependencia del Sprint 7 |
| Why 3 | La dependencia se descubrió durante el Sprint, no antes |
| Why 4 | El Refinement no incluye identificación de dependencias externas |
| Why 5 (causa raíz) | **No existe un proceso para mapear dependencias externas antes del Sprint Planning** |

---

<!-- ============================================ -->
<!-- PASO 3: Acciones SMART — SOLUCIÓN          -->
<!-- ============================================ -->

## Acción SMART 1 (para Problema 1)

**Descripción**: Tomás revisa y actualiza la Definition of Done agregando:
"Todo módulo nuevo incluye al menos 3 tests de integración (happy path + 2 edge cases)
validados en staging antes de marcarse como Done."

| Campo | Detalle |
| ----- | ------- |
| Responsable | Tomás (con revisión del equipo en Daily del Día 2 del Sprint 8) |
| Fecha de cumplimiento | Día 2 del Sprint 8 |
| Métrica de éxito | 0 bugs en producción detectados por usuarios en Sprint 8 |
| ¿Cuándo se verifica? | Retrospectiva del Sprint 8 |

---

## Acción SMART 2 (para Problema 2)

**Descripción**: Elisa agrega un bloque de 10 min al Refinement
llamado "dependencias externas": el equipo identifica qué equipos fuera de Scrum
necesitan ser notificados antes del Sprint Planning. Carmen los contacta con 5 días
de anticipación.

| Campo | Detalle |
| ----- | ------- |
| Responsable | Elisa (estructura el bloque), Carmen (contacto externo) |
| Fecha de cumplimiento | Primer Refinement del Sprint 8 |
| Métrica de éxito | Cero historias bloqueadas por dependencias externas en Sprint 8 |
| ¿Cuándo se verifica? | Retrospectiva del Sprint 8 |

---

**Acción no cumplida del Sprint anterior:**

La acción "Revisar criterios de DoD" del Sprint 6 no se cumplió.
Elisa la trae al inicio de esta retrospectiva:
> "Antes de empezar el 4Ls, revisemos lo del Sprint anterior. La acción de
> revisar la DoD no se completó. ¿Fue porque no tuvimos tiempo, o porque
> dejó de ser relevante?"

Si el equipo confirma que sigue siendo relevante (y los 3 bugs en producción lo prueban),
se integra directamente a la Acción SMART 1 de esta retro.
Esto demuestra continuidad y que las acciones tienen consecuencias reales.
