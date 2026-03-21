# Práctica 02 — Alineación Backlog ↔ OKRs

**Semana 20 | OKRs y Métricas de Valor**
**Dominio**: MediLink — plataforma de coordinación de citas médicas entre pacientes y clínicas
**Personajes**: Claudia (Product Owner) · Esteban (Scrum Master)

---

## Contexto

MediLink opera en 3 países. El equipo tiene 8 personas y trabaja en Sprints de 2 semanas.
Al inicio del Q3 definieron el siguiente OKR de equipo:

**OKR de equipo Q3:**
> **Objective**: Ser la plataforma que elimina la frustración del paciente en la gestión de citas.
>
> **KR 1**: Reducir el tiempo promedio de confirmación de cita de 4 horas a 45 minutos para el 30 de septiembre.
> **KR 2**: Aumentar el NPS de pacientes de 31 a 52 para el 30 de septiembre.
> **KR 3**: Reducir el porcentaje de citas canceladas por el paciente de 22% a 12% para el 30 de septiembre.

Estamos en el Sprint 5 (semana 9 del Q3). El equipo lleva 4 sprints entregando features pero
el KR 1 sigue en 3h 50min (casi sin cambio). El KR 2 bajó de 31 a 28. El KR 3 está en 20%.

Claudia presenta el Sprint Backlog para el Sprint 5:

| ID | User Story | Story Points | Estado |
|----|-----------|--------------|--------|
| US-031 | Como paciente quiero recibir confirmación automática de mi cita para no tener que llamar a la clínica | 5 | Seleccionada |
| US-032 | Como paciente quiero cancelar mi cita con 1 clic desde el email de recordatorio para no tener que llamar | 3 | Seleccionada |
| US-033 | Como administrador de clínica quiero exportar el listado de citas del mes en CSV para análisis interno | 3 | Seleccionada |
| US-034 | Como paciente quiero ver el historial de mis últimas 10 citas para controlar mis visitas | 2 | Seleccionada |
| US-035 | Como paciente quiero buscar médicos por especialidad y zona para encontrar opciones cercanas | 8 | Seleccionada |
| US-036 | Como clínica quiero recibir alertas cuando un paciente no confirma en 30 min para reasignar el turno | 5 | Seleccionada |

**Sprint Goal propuesto por Claudia:**
> "Completar las mejoras de experiencia del paciente."

---

## Paso 1: Clasificar Backlog Items por alineación con el OKR

Para cada User Story, determina si está **alineada** con algún KR del OKR del equipo, es
**parcialmente alineada** o **no alineada** (es valor de negocio, pero no mueve los KRs activos).

**Abre `starter/plantilla.md`** y completa la tabla del Paso 1.

---

## Paso 2: Diagnosticar por qué los KRs no mejoran

Con base en los sprints anteriores y el Sprint Backlog del Sprint 5, Esteban nota un patrón:
el equipo entrega features pero los KRs no se mueven.

> **Escenario**: En la Sprint Review del Sprint 4, la demo fue exitosa. Los stakeholders
> aplaudieron. Pero el KR 1 (tiempo de confirmación) bajó solo 10 minutos en 4 sprints.

**Abre `starter/plantilla.md`** y completa la sección del Paso 2.

---

## Paso 3: Reescribir el Sprint Goal alineado al OKR

El Sprint Goal de Claudia ("Completar las mejoras de experiencia del paciente") tiene el
mismo problema que una feature factory: describe output, no outcome.

**Abre `starter/plantilla.md`** y completa la sección del Paso 3.

---

## Criterios de Evaluación

- Tabla de clasificación con justificación para cada US
- Diagnóstico identifica la desconexión entre entrega y medición de OKRs
- Sprint Goal reescrito es específico, mide outcome y conecta con un KR concreto
- Las US depriorizadas tienen justificación coherente con el OKR activo
