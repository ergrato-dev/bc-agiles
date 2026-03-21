# Práctica 02 — Políticas Explícitas para un Tablero Kanban

## Escenario: EventFlow — Plataforma de gestión de eventos corporativos

**EventFlow** coordina producción de eventos corporativos (congresos, lanzamientos, ferias).
Su tablero Kanban tiene las columnas:

`Ideas → Propuesta → En Producción → Revisión Cliente → Ejecutado`

La Kanban Master **Camila** detectó que el equipo tiene problemas recurrentes:

1. Ítems pasan a "En Producción" sin presupuesto aprobado
2. Los clientes aprueban eventos incompletos y luego piden cambios
3. No saben qué hacer con un congreso urgente que llegó en medio de otra producción

---

### Paso 1: Políticas de entrada y salida

Para cada una de las 3 columnas críticas, define:

- **Política de entrada**: ¿qué debe cumplir el ítem ANTES de entrar a la columna?
- **Política de salida**: ¿qué debe cumplir ANTES de pasar a la columna siguiente?

**Columnas a definir**: "En Producción", "Revisión Cliente" y "Ejecutado"

---

### Paso 2: Clases de servicio

EventFlow recibe 3 tipos de solicitudes:

| Tipo | Descripción |
| ---- | ----------- |
| **Congreso anual** | Evento grande, planificado con meses de anticipación |
| **Lanzamiento urgente** | El cliente necesita un evento en menos de 2 semanas |
| **Evento estándar** | Feria o celebración corporativa, plazo de 1 mes |

**Define una clase de servicio para cada uno** con SLA y color de tarjeta.

---

### Paso 3: Solucionar el caso del congreso urgente

> "En el día 8 del Sprint, llega un congreso urgente de 500 personas para dentro de 10 días.
> El equipo ya tiene 3 ítems en 'En Producción' (WIP limit = 3)."

¿Qué debe hacer Camila según las clases de servicio definidas?

**Abre `starter/plantilla.md`** y completa los 3 pasos.
