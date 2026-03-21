# ADR-001 — Nomenclatura de Carpetas de Semanas

**Estado**: Aceptado  
**Fecha**: 2026-03-21  
**Autores**: Equipo ergrato-dev

---

## Contexto

Las carpetas de semanas del bootcamp se nombraban con el esquema `week-XX`
(ej: `week-05`, `week-12`). Este esquema no transmitía ninguna información
semántica sobre el contenido de cada semana.

## Decisión

Cambiar el esquema de nombres a `week-XX-tema_principal`, donde:

- `XX` es el número de semana con cero a la izquierda (01–24)
- `tema_principal` se extrae del título del `README.md` de cada semana
- El tema se escribe en **snake_case** (minúsculas, sin tildes, separado por `_`)

## Mapeo completo

| Antiguo          | Nuevo                                      | Tema (del README)                              |
|------------------|--------------------------------------------|------------------------------------------------|
| `week-01`        | `week-01-del_cascada_al_agil`              | Del Cascada al Ágil                            |
| `week-02`        | `week-02-principios_agiles`                | Los 12 Principios Ágiles                       |
| `week-03`        | `week-03-panorama_frameworks_agiles`       | Panorama de Frameworks Ágiles                  |
| `week-04`        | `week-04-roles_scrum`                      | Roles de Scrum                                 |
| `week-05`        | `week-05-eventos_scrum`                    | Eventos de Scrum                               |
| `week-06`        | `week-06-artefactos_scrum`                 | Artefactos de Scrum                            |
| `week-07`        | `week-07-introduccion_kanban`              | Introducción a Kanban                          |
| `week-08`        | `week-08-proyecto_integrador_etapa_0`      | Proyecto Integrador Etapa 0                    |
| `week-09`        | `week-09-user_stories`                     | User Stories: Del Problema al Backlog          |
| `week-10`        | `week-10-estimacion_agil`                  | Estimación Ágil: Puntos, Tallas y Planning Poker |
| `week-11`        | `week-11-sprint_planning_avanzado`         | Sprint Planning Avanzado                       |
| `week-12`        | `week-12-metricas_agiles`                  | Métricas Ágiles: Velocity, Burndown y CFD      |
| `week-13`        | `week-13-gestion_impedimentos`             | Gestión de Impedimentos y Deuda Técnica        |
| `week-14`        | `week-14-sprint_review_stakeholders`       | Sprint Review con Stakeholders                 |
| `week-15`        | `week-15-retrospectivas_avanzadas`         | Retrospectivas Avanzadas                       |
| `week-16`        | `week-16-proyecto_integrador_etapa_1`      | Proyecto Integrador — Etapa 1                  |
| `week-17`        | `week-17-scaled_agile`                     | Scaled Agile — SAFe, LeSS y Nexus              |
| `week-18`        | `week-18-kanban_avanzado`                  | Kanban Avanzado y #NoEstimates                 |
| `week-19`        | `week-19-devops_cicd`                      | DevOps y CI/CD en Contexto Ágil                |
| `week-20`        | `week-20-okrs_metricas_valor`              | OKRs y Métricas de Valor de Producto           |
| `week-21`        | `week-21-agile_coaching`                   | Agile Coaching: Niveles, Stances y Conversaciones |
| `week-22`        | `week-22-facilitacion_avanzada`            | Facilitación Avanzada: Liberating Structures y Design Thinking |
| `week-23`        | `week-23-transformacion_organizacional`    | Transformación Organizacional Ágil             |
| `week-24`        | `week-24-capstone_certificaciones`         | Capstone y Preparación para Certificaciones    |

## Reglas de nomenclatura

1. **Fuente del tema**: el título del `README.md` principal de cada semana (primer `#`)
2. **Formato**: snake_case (minúsculas, sin tildes ni caracteres especiales, `_` como separador)
3. **Abreviación permitida** cuando el título es muy largo (ej: `estimacion_agil` en lugar
   de `estimacion_agil_puntos_tallas_y_planning_poker`)
4. **Caracteres eliminados**: tildes (á→a, é→e, í→i, ó→o, ú→u), `#`, `:`, `.`, `-`, `,`

## Archivos actualizados

Se actualizaron todos los enlaces internos en:

- `bootcamp/week-XX-*/README.md` (navegación entre semanas, todas las 24 semanas)
- `README.md` (tabla de semanas + comando de ejemplo `cd`)
- `README_EN.md` (tabla de semanas + comando de ejemplo `cd`)
- `CONTRIBUTING.md` (referencias a archivos en ejemplos de commit)
- `.github/copilot-instructions.md` (enlace a la primera semana)

## Consecuencias

**Positivas:**
- Los nombres de carpeta son autodescriptivos: `ls bootcamp/` muestra el tema de cada semana
- Facilita la navegación sin abrir los READMEs
- Alineado con la convención del bootcamp hermano `bc-sql`

**A tener en cuenta:**
- Los commits futuros deben usar el nuevo nombre en sus referencias a rutas
- Los ejemplos de mensajes de commit con `feat(week-05)` son convenciones de formato,
  no rutas de sistema de archivos; se mantienen sin cambio
- Si el título de un README principal cambia, el nombre de la carpeta **no** se
  actualiza automáticamente — debe hacerse manualmente siguiendo este proceso
