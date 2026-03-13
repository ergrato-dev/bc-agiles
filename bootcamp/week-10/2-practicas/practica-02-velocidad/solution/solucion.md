<!-- ============================================ -->
<!-- PASO 1: SOLUCIÓN — Velocidad Sprint 2     -->
<!-- Semana 10 — Velocity & Capacity Planning   -->
<!-- ============================================ -->

## Velocidad del Sprint 2 — SOLUCIÓN

**Puntos completados (DoD cumplido):**
- US-22: 5 pts ✅
- US-23: 8 pts ✅
- US-24: 3 pts ✅
- US-25: 0 pts ⚠️ (parcial → 0)
- US-26: 2 pts ✅
- US-27: 0 pts ❌ (no iniciada → 0)

**Velocidad Sprint 2 = 5 + 8 + 3 + 2 = 18 puntos**

**Velocidad promedio (Sprint 1: 15, Sprint 2: 18):**
(15 + 18) / 2 = **16.5 → se redondea a 16 pts** (conservador) o **17 pts** (promedio)

> Convención del equipo: usar el promedio redondeado hacia abajo para
> evitar sobrecomprometer. Andrés reportaría **16 pts** como velocidad base.

**¿Por qué US-25 y US-27 no cuentan?**
El principio de **producto terminado** establece que solo genera valor
(y por tanto, solo "cuenta") lo que puede ser utilizado por el usuario.
Una Story parcial no produce valor—no puede desplegarse ni validarse.
Los puntos completados a medias capturan trabajo hecho, no valor entregado.
Este criterio evita inflar artificialmente la velocidad con trabajo parcial.

---

<!-- ============================================ -->
<!-- PASO 2: SOLUCIÓN — Capacity Sprint 3       -->
<!-- ============================================ -->

## Capacity Planning Sprint 3 — SOLUCIÓN

### Días disponibles por persona

| Persona  | Días totales | Días ocupados | Días disponibles |
| -------- | ------------ | ------------- | ---------------- |
| Valentina| 10           | 2 (feria)     | **8**            |
| Rodrigo  | 10           | 1 (mudanza)   | **9**            |
| Camila   | 10           | 0             | **10**           |
| Iván     | 10           | 1 (onboarding)| **9**            |
| **TOTAL**| **40**       | **4**         | **36**           |

### Ratio de disponibilidad

36 / 40 = **0.90 → 90% de disponibilidad**

### Capacidad proyectada

Velocidad base: 16 pts × ratio 0.90 = **14.4 ≈ 14 puntos** (conservador)

Con velocidad 17: 17 × 0.90 = **15.3 ≈ 15 puntos**

**Recomendación de Andrés: comprometer 14–15 puntos en Sprint 3.**

> Usar la banda baja (14) si hay deuda técnica pendiente de US-25 y US-27
> que debe resolverse en este Sprint. Usar 15 si esas Stories quedan fuera
> del Sprint y se reprioriza con Beatriz.

---

<!-- ============================================ -->
<!-- PASO 3: SOLUCIÓN — El stakeholder          -->
<!-- ============================================ -->

## Respuesta al stakeholder — SOLUCIÓN

**Argumentos de Andrés basados en datos:**

1. **Datos históricos**: "Nuestro promedio real de entrega es 16 puntos en
   condiciones normales. En Sprint 3 tenemos 4 días menos disponibles que
   en condiciones ideales (4 eventos conocidos). Proyectar 25 puntos sería
   un 56% más que nuestra velocidad real—eso tiene baja probabilidad de cumplirse."

2. **Costo del sobrecompromiso**: "Si comprometemos 25 pts y entregamos 15–16,
   el stakeholder recibe menos valor que si planificamos 15 pts y entregamos
   todos. La predictibilidad vale más que la ambición."

3. **Principio de mejora**: "La velocidad crece con la práctica y la madurez del
   equipo, no con la presión. Nuestro trend ya muestra mejora: 15 → 18. El Sprint 3
   esperamos 16–17 con eventos. Con el tiempo llegará naturalmente a 20–22."

**Riesgos concretos del sobrecompromiso:**
- Stories entran al Sprint sin terminar → velocidad reportada distorsionada
- Deuda técnica acumulada: corners cortados para cumplir → bugs en producción
- Burnout del equipo → baja de velocidad sostenida en siguientes sprints
- Pérdida de confianza con el stakeholder cuando no se cumple la promesa

**Propuesta alternativa:**
"Si la necesidad de valor urgente existe, revisemos juntos el backlog con
Beatriz para identificar las 3–4 Stories de mayor impacto que caben en nuestra
capacidad real. Así aseguramos que lo más importante SÍ se entrega—en lugar
de arriesgar todo por volumen."
