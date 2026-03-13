# 01 — Capacidad del Equipo y Commitment

## Objetivo

Calcular la capacidad real de un equipo antes de comprometer un Sprint.

---

## 1. ¿Por qué no usar la velocidad a ciegas?

La **Velocity** es un promedio histórico. La **Capacidad** es lo que el
equipo puede hacer *en este Sprint específico* considerando ausencias,
eventos y deuda conocida.

**Ejemplo:**
> El equipo tiene velocidad promedio de 24 pts. Pero esta semana hay
> una conferencia obligatoria: 3 personas faltan 2 días.
> Capacidad real: **¿cuánto menos de 24?**

---

## 2. Fórmula de capacidad

```
Capacidad = Σ (días disponibles por persona) × Focus Factor
```

- **Días disponibles**: días del Sprint menos ausencias, vacaciones,
  ceremonias, entrevistas, etc.
- **Focus Factor**: porcentaje del tiempo productivo real. Equipos
  nuevos: 60–70%. Equipos maduros: 70–80%. Nunca 100%.

**Ejemplo calculado:**

| Persona | Días Sprint | Ausencias | Días efectivos | × 0.70 |
| ------- | ----------- | --------- | -------------- | ------ |
| Ana     | 10          | 2         | 8              | 5.6    |
| Bruno   | 10          | 0         | 10             | 7.0    |
| Clara   | 10          | 1         | 9              | 6.3    |
| **Total** |           |           | **27**         | **~19**|

Con 19 días-foco y velocidad promedio de ~2 pts/día → Capacidad: **~18–19 pts**

---

## 3. ¿Qué entra en el Sprint?

El equipo propone qué Stories del tope del Product Backlog puede
completar dentro de la capacidad calculada. La decisión **es del equipo**,
no del PO ni del SM.

> El SM puede recordarle al equipo la capacidad calculada si ve que están
> sobrecomprometiendo — no puede forzar la selección.

---

## 4. Antipatrones del commitment

- **"Nos comprometimos con todo el backlog priorizado"** — el equipo no
  calculó capacidad, aceptó presión del PO
- **"100% de eficiencia siempre"** — no existe: reuniones, code reviews,
  contexto switching son parte del trabajo
- **"Sprint 1 con 40 puntos"** — equipo nuevo sin datos históricos

---

## Checklist

- [ ] ¿Calculaste los días disponibles reales de cada persona?
- [ ] ¿Aplicaste un focus factor entre 60–80%?
- [ ] ¿La selección del Sprint Backlog respeta la capacidad calculada?
- [ ] ¿El equipo hizo el commitment —no el SM ni el PO?
