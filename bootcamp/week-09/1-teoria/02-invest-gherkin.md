# 02 — INVEST y Criterios de Aceptación

## Objetivos

- Evaluar la calidad de una User Story con el criterio INVEST
- Escribir criterios de aceptación en formato Gherkin libre de ambigüedades
- Identificar escenarios positivos y negativos en los criterios

---

## 1. El Criterio INVEST

Cada User Story debe cumplir 6 propiedades (acrónimo INVEST):

| Letra | Propiedad | ¿Qué significa? |
| ----- | --------- | --------------- |
| **I** | Independent | No depende de otra Story para poder implementarse |
| **N** | Negotiable | Los detalles son conversables; la Story no es un contrato |
| **V** | Valuable | Aporta valor directo al usuario o al negocio |
| **E** | Estimable | El equipo puede darle un tamaño aproximado |
| **S** | Small | Cabe en un Sprint (no más de 8–13 pts) |
| **T** | Testeable | Tiene criterios verificables de "listo" |

> Una Story que falla **V** (Valuable) o **T** (Testeable) es la más
> peligrosa: puede pasar al Sprint y el equipo no sabrá cuándo terminarla.

---

## 2. Criterios de Aceptación en Gherkin

El formato **Gherkin** usa lenguaje natural estructurado:

```
Dado que [contexto/precondición]
Cuando [acción del usuario]
Entonces [resultado esperado/observable]
```

**Ejemplo completo:**

**Story**: Como usuario registrado, quiero recuperar mi contraseña por
email para poder acceder si la olvidé.

```
Dado que el usuario está en la pantalla de login
Cuando hace clic en "Olvidé mi contraseña" e ingresa su email
Entonces el sistema envía un correo con un enlace de recuperación válido por 24h

Dado que el usuario ingresa un email no registrado
Cuando hace clic en "Enviar"
Entonces el sistema muestra "Si el email existe, recibirás instrucciones"
(sin revelar si el email está o no registrado — seguridad)
```

---

## 3. Cuántos criterios de aceptación por Story

| Story size | Criterios mínimos |
| ---------- | ----------------- |
| 1–2 pts | 1–2 criterios |
| 3–5 pts | 2–4 criterios |
| 8 pts | 3–5 criterios (considerar dividir la Story) |
| 13+ pts | Muy probablemente no es Testeable → dividir |

---

## 4. Antipatrones en criterios de aceptación

- ❌ "El sistema funciona correctamente" → no es verificable
- ❌ "El usuario puede hacer cosas" → demasiado vago
- ❌ Solo escenario positivo → olvida los casos de error
- ❌ Criterio técnico: "El endpoint responde en < 200ms" → es una tarea, no un criterio de aceptación de la Story

---

## Checklist

- [ ] ¿Tu Story pasa las 6 dimensiones de INVEST?
- [ ] ¿Tienes al menos 1 escenario positivo y 1 negativo en los criterios?
- [ ] ¿Cada criterio es verificable (puede ser probado por QA)?
- [ ] ¿Los criterios están escritos desde la perspectiva del usuario, no del sistema?

---

## Referencias

- [Bill Wake — INVEST in Good Stories](https://xp123.com/articles/invest-in-good-stories-and-smart-tasks/)
- [Cucumber — Gherkin Reference](https://cucumber.io/docs/gherkin/reference/)
