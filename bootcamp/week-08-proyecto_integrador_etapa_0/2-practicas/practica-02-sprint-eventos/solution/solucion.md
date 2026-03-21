<!-- Semana 08: Proyecto Integrador Etapa 0 -->
<!-- Práctica 02 — SOLUCIÓN Daily + Review + Retro -->

# Solución — Daily, Review y Retro: ClearRoute Sprint 3

---

<!-- ============================================ -->
<!-- PASO 1: Daily Scrum — SOLUCIÓN              -->
<!-- ============================================ -->

**¿Cuál es el impedimento principal en este Daily?**

El impedimento es **doble**:
1. **Dependencia no anticipada**: Diego no empezó su tarea porque aceptó
   reuniones externas sin informar al equipo. Esto bloquea la tarea de
   animaciones que Carmen necesita para hacer los tests.
2. **Cuello de botella en US-009**: Bruno tiene capacidad libre pero
   no está asignado a ninguna tarea del Sprint. Esa capacidad puede
   liberarse para ayudar.

> Antipatrón: Diego esperaba que "alguien notara" que estaba en reuniones.
> En Scrum, el equipo se autogestiona — Diego debía haber informado el
> Day 1 que tenía conflictos y pedir ayuda para renegociar la tarea.

**¿Qué debería hacer el SM Tomás inmediatamente después del Daily?**

1. Hablar 1:1 con Diego (no en el Daily): "¿Qué necesitas para comenzar
   las animaciones hoy?" — identificar si el bloqueo es técnico o de tiempo.
2. Proponer al equipo (no imponer): ¿puede Bruno pair-programmear con Areli
   para acelerar la conexión backend-UI y liberar tiempo para Carmen?
3. Transparencia con la PO: Daniela debe saber que el Sprint Goal está en
   riesgo AHORA, no en la Review.

**¿El Sprint Goal está en riesgo? ¿Por qué?**

Sí. El Sprint Goal es "que los usuarios puedan buscar, filtrar y guardar
favoritas". Sin US-009 Done (backend + UI + tests + deploy), el goal
no se cumple aunque US-007 y US-008 estén perfectos.

**Simulación: Diego en el Daily**

> "Ayer estuve en reuniones externas de otro proyecto y no pude avanzar
> en las animaciones de US-009. Hoy necesito ese tiempo para completarlas
> — son ~4h de trabajo. **¿Alguien puede cubrir el sprint standup de las
> 11am que tengo superpuesto, o puede el SM renegociar mi asistencia
> a esas reuniones?**"

---

<!-- ============================================ -->
<!-- PASO 2: Sprint Review — SOLUCIÓN            -->
<!-- ============================================ -->

**Asumiendo que el Day 10 el equipo hace pair-programming y logra terminar
US-009 sin animaciones pero funcional:**

| Ítem | ¿Se demuestra? | Razón |
| ---- | -------------- | ----- |
| US-007 Buscar rutas | Sí | Done — en producción con tests |
| US-008 Filtrar rutas | Sí | Done — en producción con tests |
| US-009 Guardar favoritas | Sí | Done (sin animaciones — DoD cumplido) |
| US-011 Bug mapa | Sí | Done — fix en producción desde Day 8 |

**¿Se cumplió el Sprint Goal?**

**Sí** — los usuarios SÍ pueden buscar, filtrar y guardar rutas favoritas.
Las animaciones son mejora de UX, no funcionalidad. El equipo debe ser
transparente: "funciona pero sin animaciones; las incluimos en Sprint 4."

**2 preguntas para beta testers:**

1. "¿La búsqueda por nombre te ayuda a encontrar las rutas que buscas,
   o necesitarías poder buscar también por zona geográfica?"
2. "Cuando guardas una ruta favorita, ¿esperarías recibir una notificación
   si hay cambios en esa ruta (precio, disponibilidad)?"

---

<!-- ============================================ -->
<!-- PASO 3: Sprint Retrospective — SOLUCIÓN     -->
<!-- ============================================ -->

**Aportes organizados:**

| Categoría | Aporte |
| --------- | ------ |
| Start | Revisar dependencias entre tareas desde el Day 1 del Sprint |
| Start | Mejorar la estimación de US con dependencias de backend |
| Stop | Aceptar reuniones externas durante el Sprint sin consultar con el equipo |
| Continue | Daily de pie, 15 minutos, sin reportes — sigue funcionando bien |

**Acción de mejora seleccionada:**

El problema más costoso del Sprint fue el bloqueo de Diego. La causa
raíz es la ausencia de una política sobre reuniones externas.

| Qué | Quién | Cuándo |
| --- | ----- | ------ |
| Crear una política explícita: "Cualquier reunión externa durante el Sprint debe ser informada al SM y al equipo en el Daily anterior" | Tomás (SM) redacta, equipo aprueba | Antes del Day 1 del Sprint 4 |

**¿Cómo se verifica?**

En el próximo Daily donde alguien tenga una reunión externa: ¿se informó
el día anterior? Si sí → la política funciona. Si no → se escala en la
Retro del Sprint 4.
