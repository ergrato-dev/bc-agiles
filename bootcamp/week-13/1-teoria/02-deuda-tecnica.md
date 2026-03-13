# 02 — Deuda Técnica: Tipos, Gestión y Negociación

## Objetivo

Identificar la deuda técnica del producto y negociar su pago con el Product Owner.

---

## 1. ¿Qué es la deuda técnica?

La deuda técnica es el **costo futuro de no hacerlo bien hoy**.
Como una deuda financiera, tiene un capital (el trabajo pendiente) y
un interés (el costo que crece si no se paga).

> "La deuda técnica no es mala de por sí. Tomar deuda conscientemente
> para entregar valor antes tiene sentido. El problema es la deuda
> **involuntaria** que nadie registró ni planea pagar." — Ward Cunningham

---

## 2. Tipos de deuda técnica

| Tipo | Descripción | Ejemplo |
| ---- | ----------- | ------- |
| **Deliberada** | Tomada conscientemente para entregar antes | "Hardcodeamos la config, la refactorizamos en Sprint 3" |
| **Involuntaria** | Aparece sin notarse, por falta de conocimiento | Tests unitarios nunca escritos porque el equipo no sabía cómo |
| **Acumulada** | Deuda pequeña que crece con el tiempo | Módulo de autenticación de 2018 sin actualizar |
| **Diseño** | Arquitectura que no escala con el crecimiento del producto | Monolito que imposibilita los microservicios planeados |

---

## 3. ¿Cómo visualizarla?

Agregar ítems de deuda técnica al Product Backlog como **Enabler Stories**:
- No tienen valor directo para el usuario final
- Sí habilitan la entrega futura de valor
- Se priorizan según el riesgo que representan si no se pagan

**Etiqueta sugerida**: `[Deuda técnica]` o `[Enabler]`

**Criterio de priorización: impacto × urgencia**
- Alta prioridad: deuda que bloquea Features del próximo Sprint
- Media: deuda que aumenta el tiempo de desarrollo en un 30%+
- Baja: deuda que solo afecta la qualidad interna sin impacto visible

---

## 4. Cómo negociar con el PO

El PO prioriza valor de negocio. Para que acepte deuda técnica en el Sprint:

1. **Cuantificar el impacto**: "Este módulo tarda 3 horas en compilar. Arreglarlo nos ahorra 1 día de trabajo por Sprint."
2. **Vincular al riesgo**: "Si no lo refactorizamos ahora, US-45 y US-46 tomarán el doble de tiempo."
3. **Proponer la regla 20%**: reservar el 20% de la capacidad del Sprint para deuda técnica en cada Sprint.

---

## Checklist

- [ ] ¿Tienes un registro de items de deuda técnica en el Product Backlog?
- [ ] ¿Cada ítem de deuda tiene un impacto cuantificado en riesgo o tiempo?
- [ ] ¿El PO conoce los 3 mayores riesgos de deuda técnica actuales?
- [ ] ¿Tu equipo reserva capacidad regular para pagar deuda?
