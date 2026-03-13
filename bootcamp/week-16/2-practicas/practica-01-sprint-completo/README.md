# Práctica 01: Sprint Completo — CropLink

**Semana 16 — Proyecto Integrador Etapa 1**
**Empresa**: CropLink · **SM**: Diego Ferreira

---

## Contexto

CropLink es una plataforma que conecta agricultores pequeños con compradores
de mercados locales. Tiene 7 meses de desarrollo y un equipo de 5 personas.

Esta práctica muestra un **Sprint 2 completo documentado** como modelo de referencia.
Úsalo para guiar tu propio proyecto integrador.

---

## Artefacto 1: Sprint Planning

**Equipo**: Carla, Mateo, Lucía (devs), Sebastián (PO), Diego (SM)

**Capacidad Sprint 2:**

| Persona | Días disponibles | Factor foco | Días-foco |
| ------- | ---------------- | ----------- | --------- |
| Carla | 10 | 0.75 | 7.5 |
| Mateo | 9 (1 día festivo) | 0.75 | 6.75 |
| Lucía | 10 | 0.75 | 7.5 |
| **Total** | | | **21.75** → **~22 pts** |

**Sprint Goal:**
> "Para que los agricultores puedan publicar su oferta de productos sin asistencia,
> el equipo entrega el flujo completo de creación de perfil y listado de productos."

**Sprint Backlog:**

| US | Título | Pts | Responsable |
| -- | ------ | --- | ----------- |
| US-11 | Registro de agricultor | 3 | Carla |
| US-12 | Creación de perfil con foto | 5 | Carla |
| US-13 | Listado de productos con precio | 5 | Mateo |
| US-14 | Editar producto existente | 3 | Lucía |
| US-15 | Categorización de productos | 3 | Mateo |
| US-16 | Vista pública del perfil | 3 | Lucía |
| **Total** | | **22** | |

---

## Artefacto 2: Daily Scrum — muestra de 3 días

**Día 3:**
- Carla: "Terminé US-11. Hoy empiezo US-12. Sin bloqueos."
- Mateo: "US-13 al 60%. Necesito que Sebastián confirme el formato de precio: ¿con o sin IVA?"
- Lucía: "Empecé US-16. Bloqueo: no tengo acceso al servidor de imágenes para pruebas."

**Día 5:**
- Carla: "US-12 terminada. Empiezo a ayudar a Lucía con US-16."
- Mateo: "US-13 Done. US-15 al 40%. Sin bloqueos."
- Lucía: "US-16 bloqueada 2 días por acceso de imágenes. Diego escaló a Infra."

**Día 8:**
- Carla: "US-16 terminada con Lucía. Empezamos a ayudar a Mateo con US-15."
- Mateo: "US-15 Done. Sin bloqueos."
- Lucía: "US-14 al 80%. Acceso de imágenes resuelto el día 6."

---

## Artefacto 3: ROAM

| Impedimento | Owner | Nivel | ROAM | Acción | Resuelto |
| ----------- | ----- | ----- | ---- | ------ | -------- |
| Sin acceso servidor imágenes para Lucía | Diego | 2 | Owned | Diego contactó Infra el Día 5 | Día 6 ✅ |

---

## Artefacto 4: Burndown del Sprint 2

| Día | Pts restantes (ideal) | Pts restantes (real) |
| --- | --------------------- | -------------------- |
| 0 | 22 | 22 |
| 2 | 18 | 22 |
| 4 | 13 | 17 |
| 6 | 9 | 11 |
| 8 | 4 | 8 |
| 10 | 0 | 3 |

**Velocidad Sprint 2**: 19 puntos (US-14 no completada completamente; 3 pts quedaron fuera)

---

## Artefacto 5: Sprint Review

**Stakeholders**: Fernanda Cuevas (compradora local), Rodrigo Paz (agricultor piloto)

**Demo**: Carla muestra el flujo completo: registro → perfil → listado de productos.

**Feedback:**
| Stakeholder | Comentario | Tipo | Acción |
| ----------- | ---------- | ---- | ------ |
| Rodrigo | "¿Puedo poner horario de disponibilidad en el perfil?" | Nuevo req. | US-New-01 al backlog |
| Fernanda | "La foto del producto es muy pequeña en la vista pública" | Ajuste | Refinamiento de US-16 |
| Rodrigo | "El flujo de registro es justo lo que necesitaba" | Validación | Sin acción |

---

## Artefacto 6: Retrospectiva — Formato 4Ls

**Liked**: El bloqueo de imágenes se resolvió en < 24 h. La colaboración entre Carla y Lucía fue excelente.
**Learned**: Estamos subestimando historias con integración de imágenes. Necesitamos spike previo.
**Lacked**: La especificación del formato de precio (con/sin IVA) llegó tarde. Bloqueó a Mateo 2 días.
**Longed for**: Quisiéramos tener criterios de aceptación más detallados en el Refinement.

**Causa raíz (US-13 bloqueada 2 días):**
- Why 1: Mateo esperó confirmación de Sebastián
- Why 2: El criterio de formato no estaba en la historia
- Why 3: El Refinement no revisa explícitamente formatos de datos
- **Causa raíz**: La Definition of Ready no incluye "formato de datos definido"

**Acciones SMART:**

1. Sebastián agrega "formato de datos" a la plantilla de DoR del equipo.
   Métrica: Ninguna historia entra al Sprint sin este campo. Verificar en S3 Planning.
2. Diego organiza spike de 2 horas para el módulo de imágenes antes del S3 Planning.
   Responsable: Diego + Mateo. Fecha: Día 2 del Sprint 3.
