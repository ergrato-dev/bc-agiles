<!-- Semana 09: User Stories -->
<!-- Práctica 01 — SOLUCIÓN Diagnosis -->

# Solución — Diagnosis de User Stories: ProLink/Natalia

---

<!-- ============================================ -->
<!-- PASO 1: Diagnosis — SOLUCIÓN                -->
<!-- ============================================ -->

**US-A** — *"El sistema debe tener un módulo de autenticación..."*

| Criterio | ¿Cumple? | Problema |
| -------- | -------- | -------- |
| Independent | ✓ | — |
| Negotiable | ✗ | Está escrita como especificación técnica fija, no como historia de conversación |
| Valuable | ✗ | "un módulo de autenticación" no expresa valor para ningún usuario |
| Estimable | ✗ | Sin alcance claro: ¿qué métodos? ¿qué flujos? |
| Small | ✓ | (probablemente, aunque indefinida) |
| Testeable | ✗ | No hay criterio de éxito desde la perspectiva del usuario |

**Diagnóstico principal**: No es una User Story — es un requisito técnico.
No tiene rol usuario (el "sistema" no es usuario de sí mismo) y no
expresa valor de negocio.

---

**US-B** — *"Como usuario quiero que la plataforma sea rápida y fácil de usar."*

| Criterio | ¿Cumple? | Problema |
| -------- | -------- | -------- |
| Valuable | ✗ | "rápida y fácil" no define qué valor concreto recibe el usuario |
| Testeable | ✗ | ¿Cómo sabe el QA que "fácil de usar" está cumplido? |
| Small | ✗ | "la plataforma" abarca todo el producto |

**Diagnóstico principal**: Story de calidad no funcional sin criterio
verificable. Debería descomponerse en requisitos de rendimiento específicos
(ej: "la pantalla de login carga en < 2s") o convertirse en criterios del DoD.

---

**US-C** — *"Como aprendiz quiero conectarme con un mentor."*

**Problemas**:
1. **No es Small (S)**: "conectarme" implica buscar, filtrar, enviar solicitud,
   recibir respuesta, programar sesión — es una Épica completa.
2. **No es Estimable (E)**: sin saber qué significa "conectar", el equipo no puede estimar.
3. **No es Testeable (T)**: ¿cuándo está "conectado"? ¿al enviar solicitud? ¿al confirmar sesión?
4. Falta el **beneficio**: ¿para qué quiere el aprendiz conectarse?

---

**US-D** — *Falla principalmente **S (Small)***

Una sola Story no puede abarcar 7 tipos distintos de reportes. Es una
Épica disfrazada de Story.

---

**US-E** — *"Como mentor quiero confirmar una sesión..."*

Esta Story está esencialmente bien. Tiene rol, acción y beneficio implícito.
Mejoraría especificando el beneficio explícitamente:
> "...para que el aprendiz esté informado y pueda prepararse."

Y necesita criterios de aceptación (ver Paso 2).

---

**US-F** — *Falla principalmente **S (Small)** e **I (Independent)***

Describe un flujo de 7 pasos interdependientes. Cada paso es una Story
independiente potencial.

---

<!-- ============================================ -->
<!-- PASO 2: Reescritura — SOLUCIÓN              -->
<!-- ============================================ -->

**US-A reescrita:**

> Como **usuario nuevo** quiero **crear una cuenta con mi email y contraseña**
> para **poder acceder a la plataforma y encontrar un mentor**.

*Criterio 1:*
```
Dado que el usuario está en la pantalla de registro
Cuando ingresa un email válido y contraseña de mínimo 8 caracteres
Entonces el sistema crea la cuenta y muestra la pantalla de bienvenida
```

*Criterio 2:*
```
Dado que el usuario ingresa un email ya registrado
Cuando hace clic en "Registrarse"
Entonces el sistema muestra "Este email ya está en uso" sin revelar si existe o no
```

---

**US-C reescrita:**

> Como **aprendiz** quiero **buscar mentores filtrando por área profesional**
> para **encontrar a alguien con experiencia relevante en mi campo**.

*Criterio 1:*
```
Dado que el aprendiz está en la pantalla de búsqueda
Cuando selecciona "Tecnología" como área profesional
Entonces el sistema muestra una lista de mentores con ese perfil
```

*Criterio 2:*
```
Dado que no hay mentores disponibles para el filtro aplicado
Cuando el aprendiz busca
Entonces el sistema muestra "No hay mentores disponibles en esta área por ahora"
```

---

**US-E** confirmada y mejorada:

> Como **mentor** quiero **confirmar una solicitud de sesión**
> para **que el aprendiz esté informado y pueda prepararse con anticipación**.

*Criterio 1:*
```
Dado que el mentor recibe una solicitud de sesión pendiente
Cuando hace clic en "Confirmar"
Entonces el aprendiz recibe una notificación (email + in-app) con la fecha y hora confirmadas
```

*Criterio 2:*
```
Dado que el mentor rechaza una solicitud
Cuando selecciona "Rechazar" y escribe un motivo
Entonces el aprendiz recibe notificación con el motivo y puede buscar otro mentor
```

---

<!-- ============================================ -->
<!-- PASO 3: Descomposición — SOLUCIÓN           -->
<!-- ============================================ -->

**Descomposición de US-D:**

| ID | Story descompuesta |
| --- | --- |
| D-1 | Como administrador quiero ver cuántas sesiones están activas esta semana para monitorear el uso de la plataforma |
| D-2 | Como administrador quiero ver el NPS promedio de los mentores para identificar quiénes necesitan acompañamiento |
| D-3 | Como administrador quiero exportar el reporte mensual de retención para presentarlo a los inversores |

**Descomposición de US-F:**

| ID | Story descompuesta |
| --- | --- |
| F-1 | Como aprendiz quiero buscar mentores por área para encontrar opciones relevantes |
| F-2 | Como aprendiz quiero ver el perfil completo de un mentor para decidir si quiero conectarme |
| F-3 | Como aprendiz quiero enviar una solicitud de conexión para comenzar el proceso de mentoría |
| F-4 | Como aprendiz quiero dejar un review al mentor después de la sesión para ayudar a otros aprendices a elegir |
