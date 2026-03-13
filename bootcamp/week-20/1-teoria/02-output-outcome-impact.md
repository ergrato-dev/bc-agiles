# 02 — Output, Outcome e Impact: Medir lo que Importa

## Objetivos

- Distinguir output, outcome e impact en el contexto del desarrollo ágil
- Connectar el trabajo del Sprint con métricas de valor de negocio
- Evitar la trampa de medir solo lo que es fácil de medir

---

## 1. Los tres niveles de medición

| Nivel | Definición | Ejemplo |
| ----- | ---------- | ------- |
| **Output** | Lo que el equipo entrega | "Lanzamos el módulo de pagos" |
| **Outcome** | El cambio de comportamiento del usuario | "El 40% de los usuarios ahora paga en la app (antes pagaba en efectivo)" |
| **Impact** | El beneficio a largo plazo para el negocio | "Las ventas aumentaron 25% por la reducción de fricción en el pago" |

> La mayoría de los equipos mide solo Output. Los equipos maduros miden Outcome.
> El Impact es territorio del CEO y la estrategia, pero el equipo debe tenerlo presente.

---

## 2. ¿Por qué importa la diferencia?

Un equipo puede entregar 50 historias en un trimestre (alto Output) y no generar
ningún cambio en el comportamiento del usuario (cero Outcome).

**La trampa del "feature factory"**: equipos que producen features continuamente
sin medir si esas features resuelven el problema del usuario.

### El ciclo correcto

```
Hipótesis del producto → Feature entregada (Output)
  → ¿Cambió el comportamiento del usuario? (Outcome)
    → ¿Mejoró el negocio? (Impact)
      → Nueva hipótesis
```

---

## 3. Métricas de Outcome por dominio

| Tipo de producto | Métricas de Outcome típicas |
| ---------------- | ----------------------------- |
| App de consumo | DAU/MAU, retención a 30 días, NPS, session duration |
| B2B SaaS | Adoption rate, time-to-value, churn, expansion revenue |
| Plataforma interna | Tiempo ahorrado por usuario, tasa de adopción del equipo |
| E-commerce | Conversion rate, cart abandonment rate, repeat purchase rate |

---

## 4. OKRs como puente entre Output y Outcome

Un Key Result bien escrito mide Outcome, no Output:

| Output (evitar en KRs) | Outcome (correcto en KRs) |
| ---------------------- | ------------------------- |
| "Lanzar 3 nuevas features" | "Aumentar la retención a 30 días de 45% a 60%" |
| "Refactorizar el módulo de login" | "Reducir el tiempo de login de 8s a 2s" |
| "Publicar 10 artículos de ayuda" | "Reducir los tickets de soporte de login en 40%" |

---

## Checklist

- [ ] ¿Puedes reescribir un output de tu backlog como un outcome medible?
- [ ] ¿Tienes forma de medir si la última feature que entregaste cambió el comportamiento del usuario?
- [ ] ¿Tus KRs miden outcome o output?
- [ ] ¿Qué métrica de impacto sería relevante para el negocio de tu dominio asignado?

---

## Referencias

- Outcome vs Output: <https://www.jpattonassociates.com/the-new-backlog/>
- Teresa Torres — Continuous Discovery Habits: <https://www.producttalk.org/>
