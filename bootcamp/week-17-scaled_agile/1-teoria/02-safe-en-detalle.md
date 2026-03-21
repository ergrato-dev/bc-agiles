# 02 — SAFe en profundidad: ART, PI Planning y Program Backlog

## Objetivos

- Comprender la estructura de un Agile Release Train (ART)
- Describir el ciclo de un PI y el evento PI Planning
- Construir un Program Backlog básico con Epics y Features

---

## 1. El Agile Release Train (ART)

Un ART es el principal mecanismo de entrega en SAFe.
Es un equipo de equipos — entre 5 y 12 equipos Scrum — que **planifican, ejecutan y aprenden juntos**.

```
ART (50–125 personas)
│
├── Equipo 1 (7 personas) ← Sprint de 2 semanas
├── Equipo 2 (8 personas)
├── Equipo 3 (6 personas)
└── ...
│
└── Program Increment (PI) = 4–5 Sprints + 1 Sprint de innovación y planificación
```

### Roles del ART

| Rol | Equivalente Scrum | Responsabilidad |
| --- | ----------------- | --------------- |
| **Release Train Engineer (RTE)** | Scrum Master del ART | Facilitar el ART, remover impedimentos sistémicos |
| **Product Manager** | Product Owner del ART | Gestionar el Program Backlog y visión del PI |
| **System Architect** | — | Guía técnica de la arquitectura del ART |

---

## 2. El PI Planning

El PI Planning es el evento más importante de SAFe.
Dura **2 días** y reúne a **todos los equipos del ART** para planificar el próximo PI.

### Agenda típica (2 días)

| Tiempo | Actividad |
| ------ | --------- |
| Día 1 mañana | Visión del negocio — Product Manager comparte el roadmap |
| Día 1 tarde | Cada equipo crea su Team PI Plan (qué entregará en cada Sprint) |
| Día 2 mañana | Identificación de dependencias — los equipos coordinan entre sí |
| Día 2 tarde | Presentación y ajuste de riesgos (ROAM a nivel ART) |
| Día 2 cierre | Compromiso del ART con el PI Objective |

### PI Objectives

Cada equipo declara **3–5 objetivos** para el PI con un Business Value (1–10).
El conjunto forma el **PI Objective del ART**.

---

## 3. El Program Backlog

El Program Backlog es la lista de **Features** pendientes para el ART.
Su jerarquía:

```
Epic (trimestres)
 └── Feature (PI — 8–12 semanas)
      └── Story (Sprint — 2 semanas)
```

**Criterio de aceptación de una Feature** — formato similar a las User Stories:

```
Dado que [contexto del equipo]
Cuando [la feature está implementada]
Entonces [beneficio de negocio medible]
```

---

## 4. Antipatrones de SAFe

- ❌ PI Planning donde los equipos solo escuchan sin planificar activamente
- ❌ Features tan grandes que no caben en un Sprint (deberían ser Stories)
- ❌ RTE que actúa como Project Manager clásico asignando tareas
- ❌ Program Backlog gestionado sin refinamiento continuo

---

## Checklist

- [ ] ¿Cuántos Sprints tiene típicamente un PI?
- [ ] ¿Quién presenta la visión del negocio en el PI Planning?
- [ ] ¿Qué diferencia a una Feature de una Epic en SAFe?
- [ ] ¿Qué significa un Business Value de 10 en un PI Objective?

---

## Referencias

- SAFe PI Planning: <https://scaledagileframework.com/pi-planning/>
- SAFe Roles: <https://scaledagileframework.com/roles/>
- Program Backlog: <https://scaledagileframework.com/program-backlog/>
