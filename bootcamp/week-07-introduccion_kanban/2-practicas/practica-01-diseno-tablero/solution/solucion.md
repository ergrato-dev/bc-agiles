<!-- Semana 07: Introducción a Kanban -->
<!-- Práctica 01: Diseñar Tablero — SOLUCIÓN -->

# Solución — Diseño de Tablero Kanban HelpDesk360

---

## Sección 1: Columnas del tablero

| # | Columna | Descripción | ¿Quién trabaja aquí? |
|---|---------|-------------|---------------------|
| 1 | **Entrante** | Tickets recibidos, sin triaje | Nadie activamente (cola de entrada) |
| 2 | **Triaje** | Revisión de info, clasificación de prioridad | Técnicos N1 |
| 3 | **En espera de info** | Se pidió información al cliente, esperando respuesta | Ticket en pausa (no cuenta en WIP) |
| 4 | **En Investigación** | Técnico trabajando activamente en el problema | N1 (simple) / N2 (complejo) |
| 5 | **En Verificación** | Fix aplicado, verificando en entorno del cliente | Técnico Senior o QA |
| 6 | **Done** | Ticket cerrado y confirmado por el cliente | — |

**Paso NO convertido en columna**: "notificación al cliente" — es una acción dentro de la columna Done, no un estado independiente. Agregar una columna para eso agrega ruido sin valor de visibilidad.

---

## Sección 2: WIP Limits

| Columna | WIP Limit | Razonamiento |
|---------|-----------|--------------|
| Triaje | 5 | 2 técnicos N1 × 2 ítems c/u + 1 de buffer = 5 |
| En Investigación N1 | 4 | 2 técnicos N1, máx 2 tickets simultáneos por persona |
| En Investigación N2 | 4 | 2 técnicos N2, máx 2 tickets simultáneos por persona |
| En Verificación | 3 | 1 técnico Senior + capacidad de revisión real; saturación actual visible |

**Efecto en Ana y Marcos**: El WIP limit de 4 en "En Investigación N1" haría
explícito que no pueden tener 8 tickets activos. Si los 4 slots están ocupados,
DEBEN terminar uno antes de jalar otro. Esto resuelve el problema de multitarea y
reduce el caos visible en el tablero actual.

---

## Sección 3: Política explícita

**Criterio de ENTRADA a En Verificación:**
- El fix técnico fue aplicado en el entorno de staging o directamente en prod del cliente
- El técnico que hizo el fix documentó qué cambió y por qué
- No hay errores activos en los logs relacionados con el ticket

**Criterio de SALIDA de En Verificación:**
- El técnico senior o QA confirmó manualmente que el problema original no reproduce
- Se registró el resultado de la verificación en el ticket (fecha, quién verificó, método)
- El cliente fue notificado y confirmó el cierre (o pasaron 24 horas sin respuesta)

**Si la verificación falla:**
El ticket vuelve a "En Investigación" con una nota clara del error detectado.
No se vuelve a "Triaje" porque ya pasó por ese filtro. El técnico que hizo el fix
es responsable de corregirlo; no se asigna a otro a menos que esté bloqueado.
