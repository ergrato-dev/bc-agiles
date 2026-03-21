# 02 — Prácticas XP en Equipos Scrum: TDD, Pair Programming y Refactoring

## Objetivos

- Identificar las prácticas técnicas de XP más útiles para equipos Scrum
- Comprender cómo TDD mejora la calidad sin aumentar el tiempo total
- Reconocer cuándo aplicar Pair Programming y Refactoring en el Sprint

---

## 1. XP como complemento técnico de Scrum

Scrum define QUÉ hacer (eventos, artefactos, roles). XP (Extreme Programming)
define **CÓMO hacerlo bien técnicamente**. Son complementarios, no competidores.

Un equipo Scrum sin prácticas XP puede cumplir la DoD con código de baja calidad.
XP pone el foco en la **excelencia técnica**.

---

## 2. TDD (Test-Driven Development)

El ciclo TDD:

```
1. Escribe un test que FALLA (prueba que define lo que debe hacer el código)
2. Escribe el código MÍNIMO para que el test pase
3. Refactoriza el código sin que los tests fallen
```

### Ventajas en el contexto del Sprint

- Los tests son la documentación ejecutable del código
- Permite refactorizar con confianza (los tests detectan regresiones)
- Reduce el tiempo en bugs en Sprints posteriores

> **Antipatrón**: escribir los tests DESPUÉS de codificar. Es diferente a TDD
> y pierde el principal beneficio: diseñar desde la prueba.

---

## 3. Pair Programming

Dos personas trabajan juntas en el mismo código: una escribe (driver), la otra revisa (navigator).
Rotan el rol cada 25–30 minutos.

| Ventaja | Cuándo aplicarlo |
| ------- | ---------------- |
| Revisión en tiempo real | Historias de alta complejidad o riesgo |
| Transferencia de conocimiento | Onboarding de nuevos miembros |
| Menor deuda técnica | Módulos que otros dependerán críticamente |

> **Mito a desmontar**: "Pair Programming duplica el tiempo."
> Los estudios muestran 15% más de tiempo con 15% menos de bugs y mejor diseño a largo plazo.

---

## 4. Refactoring

Refactorizar es mejorar el diseño interno del código **sin cambiar su comportamiento externo**.
Es parte de la DoD en equipos maduros.

**Cuándo refactorizar en el Sprint**: como parte de la Definition of Done de cada historia,
no como tarea separada. "La historia no está terminada si el código no está limpio."

---

## Checklist

- [ ] ¿En qué orden se escriben el test y el código en TDD?
- [ ] ¿Cuándo es más valioso hacer Pair Programming dentro de un Sprint?
- [ ] ¿Cuál es la diferencia entre refactoring y reescritura?
- [ ] ¿Cómo convencerías a un Product Owner de que TDD aporta valor de negocio?

---

## Referencias

- XP Practices: <http://www.extremeprogramming.org/rules.html>
- TDD Guide: <https://martinfowler.com/bliki/TestDrivenDevelopment.html>
