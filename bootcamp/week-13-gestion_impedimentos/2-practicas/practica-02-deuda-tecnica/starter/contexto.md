# HealthSync — Contexto del Sprint 7

## La empresa

**HealthSync** conecta pacientes con médicos de cabecera mediante registros
de biométricos diarios (frecuencia cardíaca, glucosa, presión arterial).
El sistema envía alertas automáticas cuando los valores salen del rango normal.

**Equipo**: 3 desarrolladores (Hernán, Sofía, Tomás), 1 PO (Catalina), 1 SM (Beatriz)

---

## Situación actual

Sprint 7 está por comenzar. En el Backlog Refinement, Hernán plantea:

> "Antes de seguir agregando features, necesitamos hablar de la deuda técnica.
> El módulo de auth lleva 6 meses sin tocarse y no tiene ningún test.
> El PDF solo funciona para pacientes tipo A — los médicos se quejan.
> Las consultas a base de datos tardan hasta 5 segundos. Y el monolito
> ya nos impide separar el flujo de pacientes del de médicos."

Catalina responde:

> "Entiendo la preocupación, pero tenemos tres features prometidas para este Sprint.
> Los stakeholders esperan resultados. ¿No podemos dejar la deuda para después?"

**Beatriz interviene** para facilitar la conversación y llegar a un acuerdo.

---

## Ítems de deuda identificados

| ID   | Descripción del problema                                              | Detectado por |
| ---- | --------------------------------------------------------------------- | ------------- |
| DT-01 | Módulo de auth: sin tests, código del año 1, sin actualizar 6 meses | Hernán        |
| DT-02 | PDF hardcodeado solo para tipo A; tipos B y C no pueden exportar      | Sofía         |
| DT-03 | Queries sin índices: consultas de historial tardan 3–5 seg            | Tomás         |
| DT-04 | Monolito: no se puede separar flujo paciente de flujo médico          | Equipo        |

---

## Capacidad del Sprint 7

- Días disponibles: 50 días-persona (equipo completo, sin ausencias)
- Factor de foco: 0.75
- **Capacidad neta estimada**: ~37–38 puntos de historia
