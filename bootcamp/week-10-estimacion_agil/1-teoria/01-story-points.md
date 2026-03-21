# 01 — Story Points y Estimación Relativa

## Objetivos

- Entender por qué los Story Points superan a las horas en precisión útil
- Conocer la secuencia de Fibonacci y por qué se usa en estimación
- Aplicar el concepto de "Story de referencia" para calibrar al equipo

---

## 1. El problema con las horas

Cuando un developer dice "esto tarda 4 horas", en realidad significa:
- 4 horas si no hay interrupciones
- 4 horas si el entorno está configurado
- 4 horas... de las horas de ese developer específico

El mismo ítem estimado en 4h por Bruno puede tardar 10h para Areli.

Los **Story Points** evitan ese problema: son una estimación **relativa**
del esfuerzo, complejidad e incertidumbre — no del tiempo.

---

## 2. Estimación relativa: cómo funciona

El equipo elige una **Story de referencia** (la más simple de todas)
y le asigna 1 punto. Luego compara todas las demás contra ella:

> "La Story de búsqueda básica es 1 punto. La de búsqueda con filtros
> es aproximadamente 3 veces más compleja → 3 puntos."

Lo que el equipo calibra: **complejidad + esfuerzo + incertidumbre**.

---

## 3. La secuencia de Fibonacci modificada

Valores estándar de Planning Poker:

```
0 · 1 · 2 · 3 · 5 · 8 · 13 · 21 · 40 · 100 · ? · ∞
```

Por qué estas opciones:
- Los **gaps grandes entre valores altos** fuerzan a reconocer incertidumbre
- Un ítem de 21 vs 20 no hace diferencia real — la brecha entre 13 y 21 sí
- `?` = "no entiendo suficiente para estimar"
- `∞` = "esto es demasiado grande, hay que dividirlo"

> Una Story que recibe `?` o `∞` **no debe entrar al Sprint** hasta
> ser refinada. Es el primer filtro de calidad del backlog.

---

## 4. El mito de "1 punto = 1 hora"

Si el equipo empieza a igualar Story Points con horas, pierde los
beneficios de la estimación relativa:

| Estimación en horas | Estimación en Story Points |
| -------------------- | --------------------------- |
| Individual y precisa | De equipo y relativa |
| Falsa precisión | Honesta sobre la incertidumbre |
| Se "gana o pierde" tiempo | El equipo aprende su velocity |
| Promueve multitarea | Promueve focus en completar |

---

## Checklist

- [ ] ¿Definiste una Story de referencia de 1 punto para tu equipo?
- [ ] ¿Las estimaciones más altas reflejan más complejidad, no más tiempo?
- [ ] ¿Hay ítems marcados como `?` que necesitan refinamiento?
- [ ] ¿Tu equipo entiende que los puntos no equivalen a horas?

---

## Referencias

- [Mountain Goat Software — Story Points](https://www.mountaingoatsoftware.com/blog/what-are-story-points)
- [Ron Jeffries — Story Points Revisited](https://ronjeffries.com/articles/019-01ff/story-points/)
