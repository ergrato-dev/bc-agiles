<!-- Semana 09: User Stories -->
<!-- Práctica 02 — SOLUCIÓN Gherkin -->

# Solución — Escritura con Gherkin: VitalApp/Sofía

---

**Necesidad 1 — Registro de agua**

**User Story:**
> Como **estudiante universitario** quiero **registrar cada vaso de agua
> que tomo durante el día** para **saber si alcanzo mi meta diaria de hidratación**.

*Criterio positivo 1:*
```
Dado que el usuario está en la pantalla de hábitos
Cuando toca el botón "+ 1 vaso (250ml)"
Entonces el contador diario de agua aumenta en 250ml y muestra el progreso (ej: 1500/2000ml)
```

*Criterio positivo 2:*
```
Dado que el usuario alcanza su meta diaria de agua
Cuando registra el último vaso
Entonces el sistema muestra el mensaje "¡Meta de hidratación alcanzada!" y registra el logro del día
```

*Criterio negativo:*
```
Dado que el usuario intenta registrar agua sin conexión a internet
Cuando toca el botón de registro
Entonces el sistema guarda el registro localmente y lo sincroniza cuando recupere conexión
```

---

**Necesidad 2 — Registro de alimentación**

**User Story:**
> Como **estudiante con hábitos alimenticios irregulares** quiero
> **registrar cómo me alimenté cada día con una calificación sencilla**
> para **identificar los días y patrones en que como peor**.

*Criterio positivo 1:*
```
Dado que el usuario abre el registro diario de alimentación
Cuando selecciona "Día difícil 🍟" (de las opciones: Excelente / Normal / Difícil)
Entonces el sistema guarda la calificación con la fecha y hora del registro
```

*Criterio positivo 2:*
```
Dado que el usuario tiene 7 días registrados
Cuando abre la pantalla de "Mi patrón semanal"
Entonces el sistema muestra un gráfico con la calificación diaria de la semana
```

*Criterio negativo:*
```
Dado que el usuario intenta registrar la alimentación de un día ya registrado
Cuando abre el registro de ese día
Entonces el sistema permite editar el registro existente con confirmación "¿Editar registro del [fecha]?"
```

---

**Necesidad 3 — Panel del monitor universitario**

**User Story:**
> Como **monitor de salud universitaria** quiero **ver un resumen del
> progreso de hábitos del grupo de estudiantes que asesoro**
> para **identificar quiénes necesitan más apoyo sin revisar cada perfil**.

*Criterio positivo 1:*
```
Dado que el monitor está en el panel de su grupo asignado
Cuando hace clic en "Ver resumen semanal"
Entonces el sistema muestra: % de estudiantes activos, promedio de metas cumplidas/semana, top 3 hábitos registrados
```

*Criterio positivo 2:*
```
Dado que el monitor quiere ver solo estudiantes con baja actividad
Cuando aplica el filtro "Sin actividad en +7 días"
Entonces el sistema muestra la lista de estudiantes que no han registrado nada en esa semana
```

*Criterio negativo:*
```
Dado que el monitor no tiene estudiantes asignados aún
Cuando abre el panel
Entonces el sistema muestra "Aún no tienes estudiantes asignados. Contacta al coordinador."
```

---

**Necesidad 4 — Compartir logro social**

**User Story:**
> Como **usuario activo** quiero **compartir cuando cumplo mi meta diaria
> de hábitos** para **celebrar mi progreso con mi comunidad de amigos**.

*Criterio positivo 1:*
```
Dado que el usuario cumplió su meta diaria (todos los hábitos marcados como Done)
Cuando toca el botón "Compartir logro"
Entonces el sistema genera una tarjeta visual con el logro y opciones para compartir en WhatsApp, Instagram o copiar enlace
```

*Criterio positivo 2:*
```
Dado que el usuario toca "Compartir en WhatsApp"
Cuando confirma
Entonces se abre WhatsApp con la imagen del logro y el texto pre-cargado "¡Cumplí mis metas de hoy con VitalApp!" (editable)
```

*Criterio negativo:*
```
Dado que el usuario no ha cumplido todas sus metas del día
Cuando intenta compartir
Entonces el botón "Compartir logro" está desactivado y muestra un tooltip "Completa todas tus metas para compartir"
```

---

<!-- ============================================ -->
<!-- PASO 3: Validación INVEST — SOLUCIÓN        -->
<!-- ============================================ -->

| Story | Small (S) | Testeable (T) | Ajuste |
| ----- | --------- | ------------- | ------ |
| Necesidad 1 — Agua | ✓ | ✓ | Ninguno — está bien acotada |
| Necesidad 2 — Alimentación | ✓ | ✓ | Ninguno — "patrón semanal" puede ser Sprint 2 si el equipo lo necesita |
| Necesidad 3 — Panel monitor | ⚠ | ✓ | Podría dividirse: "ver resumen" (S-1) y "filtrar por actividad" (S-2) |
| Necesidad 4 — Compartir logro | ✓ | ✓ | Ninguno |

> Nota sobre Necesidad 3: Si el equipo considera que el resumen + el
> filtro son demasiado para 1 Sprint, dividir en 2 Stories independientes
> es la decisión correcta. INVEST permite (y fomenta) esa negociación.
