# 01 — Anatomía de una User Story

## Objetivos

- Conocer el formato estándar de una User Story y para qué sirve cada parte
- Entender la jerarquía del Product Backlog: Épica → Feature → Story → Task
- Reconocer cuándo una "historia" no está cumpliendo su propósito

---

## 1. El Formato Estándar

```
Como [ROL]
quiero [ACCIÓN]
para [BENEFICIO del negocio o del usuario]
```

Cada parte tiene una función precisa:

| Parte | Pregunta que responde | Ejemplo |
| ----- | --------------------- | ------- |
| **Como [rol]** | ¿Quién tiene esta necesidad? | "Como viajero frecuente" |
| **quiero [acción]** | ¿Qué necesita poder hacer? | "quiero guardar mis rutas favoritas" |
| **para [beneficio]** | ¿Por qué le importa? | "para encontrarlas rápido en mi próximo viaje" |

> La parte más olvidada es el **beneficio**. Sin ella, la Story no
> comunica valor — es solo una especificación técnica.

---

## 2. La Jerarquía del Backlog

```
ÉPICA (meses de trabajo)
 └── FEATURE (semanas)
      └── USER STORY (días, cabe en 1 Sprint)
           └── TASK (horas, 1 developer)
```

**Épica**: "Permitir que los usuarios gestionen su perfil completo"
**Feature**: "Gestión de preferencias de viaje"
**Story**: "Como viajero, quiero elegir mi nivel de dificultad preferido para recibir rutas adaptadas a mí"
**Task**: "Crear dropdown de dificultad en la pantalla de perfil (4h - Areli)"

---

## 3. Cuándo una Story NO es una Story

| Problema | Ejemplo incorrecto | Corrección |
| -------- | ------------------- | ---------- |
| Sin rol claro | "Quiero ver el mapa" | "Como usuario registrado..." |
| Sin beneficio | "Como PO quiero mejorar el login" | El PO no es usuario del producto |
| Demasiado grande | "Como usuario quiero usar la app" | Descomponer en Épica → Stories |
| Técnica pura | "Refactorizar la base de datos" | Es una Task, no una Story |

---

## 4. La Story como conversación

Una User Story es una **promesa de conversación**, no una especificación
completa. Ron Jeffries la describió con las 3 Cs:

- **Card**: escrita en una tarjeta (breve, visible)
- **Conversation**: se discute en el refinamiento
- **Confirmation**: los criterios de aceptación confirman cuándo está Done

---

## Checklist

- [ ] ¿Tu Story tiene los 3 elementos: rol, acción y beneficio?
- [ ] ¿El "rol" es un usuario real del producto (no el PO ni el SM)?
- [ ] ¿Cabe en un Sprint o necesitas descomponerla?
- [ ] ¿Tienes al menos 1 criterio de aceptación definido?

---

## Referencias

- [User Stories Applied — Mike Cohn (resumen)](https://www.mountaingoatsoftware.com/books/user-stories-applied)
- [Scrum.org — Product Backlog Refinement](https://www.scrum.org/resources/blog/product-backlog-refinement-explained)
