# Design Thinking como Facilitación de Innovación

**Semana 22 | Etapa 2: Ágil Avanzado**

## Objetivos

1. Comprender las 5 fases del proceso de Design Thinking
2. Conectar Design Thinking con el refinamiento del Product Backlog
3. Identificar los artefactos clave: HMW, mapa de empatía, prototipo y test

---

## 1. ¿Qué es Design Thinking en contexto ágil?

Design Thinking (DT) es un proceso de resolución de problemas centrado en el usuario.
En equipos ágiles, se usa para descubrir y validar ideas antes de escribir User Stories.
Evita el antipatrón de construir features sin evidencia de valor para el usuario.

**Relación con Scrum**: DT vive en el espacio de Discovery (antes del Sprint). Sus outputs
alimentan directamente el Product Backlog con ítems validados.

---

## 2. Las 5 Fases

### Empatizar
Entender al usuario: sus comportamientos, frustraciones y motivaciones reales.
Herramientas: entrevistas en profundidad, shadowing, mapa de empatía.

> **Mapa de empatía** (4 cuadrantes): ¿Qué piensa y siente? / ¿Qué ve? /
> ¿Qué dice y hace? / ¿Qué escucha?

### Definir
Sintetizar lo aprendido en un problema concreto y centrado en el usuario.
Herramienta clave: **"How Might We" (HMW)**.

> Formato HMW: *"¿Cómo podríamos [acción deseable] para que [usuario] logre [resultado]
> sin [restricción]?"*
>
> Ejemplo: *"¿Cómo podríamos reducir la fricción al completar el formulario de admisión
> para que el paciente finalice el proceso en menos de 5 minutos?"*

El HMW debe ser suficientemente abierto para generar múltiples ideas y suficientemente
acotado para no ser trivial.

### Idear
Generar muchas ideas sin juzgar. Cantidad antes que calidad.
Herramientas: brainstorming clásico, Crazy 8s (8 ideas en 8 minutos).

**Crazy 8s**: Doblar una hoja en 8 partes. Cada cuadrante = 1 idea en 1 minuto.
El formato tiempo-presión elimina el filtro del juicio.

### Prototipar
Construir una representación de bajo costo de las mejores ideas para aprender rápido.
Un prototipo NO es el producto final. Es la mínima representación que permita aprender.

Tipos de prototipo:
| Tipo | Material | Tiempo |
|------|----------|--------|
| Boceto en papel | Papel y lápiz | 15 min |
| Storyboard | Secuencia de viñetas | 30 min |
| Landing page falsa | HTML estático | 2h |
| Role playing | Actuación del flujo | 20 min |

### Testear
Presentar el prototipo a usuarios reales y observar su reacción.
Regla de oro: **el testeo no es una demo**. No se explica el prototipo.
Se observa y se escucha. Las confusiones son datos valiosos.

---

## 3. Conexión con el Product Backlog

| Fase DT | Artefacto generado | Uso en Scrum |
|---------|-------------------|--------------|
| Empatizar | Mapa de empatía, Jobs To Be Done | Define el usuario real de las User Stories |
| Definir | HMW, Point of View statement | Inspira el Sprint Goal y el Objective del OKR |
| Idear | Lista de ideas priorizadas | Insumo para el Product Backlog (Epics, Features) |
| Prototipar | Mockups, storyboards verbales | Criterios de aceptación de User Stories |
| Testear | Feedback de usuarios | Retroalimenta el backlog y el sprint siguiente |

---

## 4. Antipatrones

- **Saltar Empatizar**: el equipo asume que ya sabe lo que quiere el usuario.
  Resultado: features que nadie usa (feature factory confirmado).
- **Prototipo sobreproducido**: gastan 2 semanas en el mockup "perfecto" antes de testear
  con usuarios. Pierden el principio de bajo costo y rápido aprendizaje.
- **Testeo como venta**: el facilitador explica el prototipo en lugar de observar.
  El usuario no puede confundirse porque el facilitador impone el flujo correcto.

---

## Checklist

- [ ] ¿Puedo escribir un HMW correctamente formulado?
- [ ] ¿Entiendo qué diferencia un prototipo de un MVP?
- [ ] ¿Sé conectar los outputs del DT con el Product Backlog?
- [ ] ¿Identifico el antipatrón de usar DT como excusa para no entregar?

---

## Referencias

- [IDEO Design Thinking for Educators](https://www.ideo.com/tools)
- Stanford d.school — *An Introduction to Design Thinking Process Guide*
