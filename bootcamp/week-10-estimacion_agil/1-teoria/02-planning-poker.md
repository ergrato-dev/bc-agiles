# 02 — Planning Poker y T-Shirt Sizing

## Objetivos

- Facilitar una sesión de Planning Poker paso a paso
- Gestionar divergencias de estimación productivamente
- Elegir entre Planning Poker y T-Shirt Sizing según el contexto

---

## 1. Planning Poker: el proceso

**Participantes**: Todo el equipo Scrum (PO presente para preguntas,
no para influenciar estimaciones).

**Pasos:**

1. **El PO lee la User Story** en voz alta e incluye los criterios de aceptación
2. **El equipo hace preguntas** de clarificación (máx. 5 min)
3. **Cada developer selecciona** su carta en secreto
4. **Revelación simultánea** — todos muestran su carta al mismo tiempo
5. **Si hay consenso** → esa es la estimación, siguiente Story
6. **Si hay divergencia** → los extremos (más alto y más bajo) justifican su elección en 2 minutos, nueva ronda

> La revelación simultánea es NON-NEGOTIABLE. Si se revela en secuencia,
> el ancoring bias contamina las estimaciones del resto.

---

## 2. Gestionar divergencias

**Escenario típico**: Areli pone 3, Bruno pone 8.

El SM facilita sin opinar:
> "Areli, ¿qué ves que te hace pensar en 3?"
> "Bruno, ¿qué ves que hace que sea 8 para ti?"

Frecuentemente, la divergencia revela **información que uno tiene y el
otro no** — y eso es exactamente lo valioso de la sesión.

Regla: si después de 3 rondas no hay consenso, el equipo vota por la
estimación más alta (el ruido adicional es más seguro que la subestimación).

---

## 3. T-Shirt Sizing

Alternativa más rápida para backlog inicial o refinamiento de Épicas:

| Talla | Descripción | Story Points aprox. |
| ----- | ----------- | ------------------- |
| XS | Trivial, sin complejidad | 1–2 |
| S | Simple, bien entendida | 3 |
| M | Mediana complejidad | 5–8 |
| L | Alta complejidad o incertidumbre | 13 |
| XL | Muy grande, probablemente dividir | 21+ |

**Cuándo usar T-Shirt Sizing**:
- Backlog inicial con 50+ ítems (hace el proceso más rápido)
- Refinamiento de Épicas antes de descomponer en Stories
- Equipos nuevos que aún no tienen puntos de referencia consolidados

**Cuándo usar Planning Poker**:
- Sprint Planning o refinamiento detallado
- Stories que entrarán al próximo Sprint
- Cuando la precisión relativa importa para el compromiso del Sprint

---

## 4. #NoEstimates

Corriente de pensamiento que propone eliminar las estimaciones formales
y en su lugar usar métricas de flujo (Lead Time, Throughput).

> Es un tema avanzado que se verá en la Semana 18 (Kanban avanzado).
> Por ahora, domina Planning Poker antes de cuestionar la estimación.

---

## Checklist

- [ ] ¿Las cartas se revelan siempre de forma simultánea?
- [ ] ¿El SM facilita la discusión sin compartir su propia estimación?
- [ ] ¿Los Stories de 13+ puntos son candidatos a descomposición?
- [ ] ¿El PO está disponible para resolver dudas pero no influye en la estimación?

---

## Referencias

- [Planning Poker — Mike Cohn](https://www.mountaingoatsoftware.com/agile/planning-poker)
- [Scrum.org — Story Points](https://www.scrum.org/resources/blog/why-do-we-use-story-points-estimating)
