# 01 — SAFe, LeSS y Nexus: panorama de marcos de escalado

## Objetivos

- Reconocer los 3 principales frameworks de Scaled Agile
- Comparar sus características y contextos de aplicación
- Identificar los antipatrones más comunes del escalado

---

## 1. ¿Por qué escalar?

Un equipo Scrum funciona bien hasta ~9 personas.
Cuando la empresa crece necesita coordinar múltiples equipos trabajando en el **mismo producto**.

El escalado no significa "más reuniones". Significa **mantener la agilidad** con más personas.

> ⚠️ **Antipatrón clásico**: escalar Scrum antes de dominarlo en un equipo.
> Si el equipo aún no hace Retros efectivas, escalar lo empeorará.

---

## 2. Los tres frameworks

| Framework | Creado por | Equipos objetivo | Complejidad |
| --------- | ---------- | ---------------- | ----------- |
| **SAFe** | Scaled Agile, Inc. | 5–125+ equipos | Alta |
| **LeSS** | Larman & Vodde | 2–8 equipos (LeSS) / +8 (LeSS Huge) | Media |
| **Nexus** | Scrum.org | 3–9 equipos | Baja-Media |

### SAFe (Scaled Agile Framework)

SAFe organiza los equipos en un **Agile Release Train (ART)** — un "meta-equipo"
de 50–125 personas que planifican juntas en ciclos de 8–12 semanas llamados **PI (Program Increment)**.

- Rol clave: **Release Train Engineer (RTE)** — Scrum Master del ART
- Artefacto clave: **Program Backlog** (Epics → Features → Stories)
- Evento clave: **PI Planning** — reunión de 2 días donde todos los equipos sincronizan

### LeSS (Large-Scale Scrum)

LeSS aplica los principios de Scrum **directamente** a múltiples equipos, con cambios mínimos.
Un solo Product Owner gestiona un único Product Backlog compartido.

- Todos los equipos comparten el mismo Sprint
- Un único Sprint Review con todos los equipos
- LeSS Huge añade el rol de **Area Product Owner**

### Nexus

Framework de Scrum.org que añade solo una capa mínima sobre Scrum estándar.
Introduce el **Nexus Integration Team (NIT)** — responsable de la integración entre equipos.

- Artefacto clave: **Nexus Sprint Backlog** — visibilidad de dependencias
- Evento clave: **Nexus Sprint Planning** — coordinación de dependencias entre equipos

---

## 3. ¿Cuándo usar cada uno?

| Situación | Framework recomendado |
| --------- | --------------------- |
| Empresa grande, múltiples departamentos | SAFe |
| 2–8 equipos en el mismo producto | LeSS o Nexus |
| Organización que ya domina Scrum | LeSS |
| Primera vez escalando, cambio mínimo | Nexus |

---

## 4. Antipatrones del escalado

- ❌ Añadir niveles jerárquicos sin eliminar los anteriores
- ❌ PI Planning como ceremonia de presentación (no de planificación real)
- ❌ Equipos "Scrum" que en realidad son silos funcionales
- ❌ Un solo backlog compartido sin Product Owner con autoridad real

---

## Checklist

- [ ] ¿Puedes nombrar el rol equivalente al "Scrum Master del ART" en SAFe?
- [ ] ¿Cuántos equipos soporta Nexus como máximo?
- [ ] ¿Qué diferencia al Product Backlog de LeSS del Program Backlog de SAFe?
- [ ] ¿Cuáles son las señales de que escalar es prematuro?

---

## Referencias

- SAFe Overview: <https://scaledagileframework.com/>
- LeSS Framework: <https://less.works/>
- Nexus Guide: <https://www.scrum.org/resources/nexus-guide>
