<!-- Semana 17: Práctica 02 — PI Planning — SOLUCIÓN -->
<!-- EduRed: plataforma digital para red de escuelas  -->

<!-- ============================================ -->
<!-- PASO 1: Features — SOLUCIÓN                -->
<!-- ============================================ -->

**Feature A — Rendimiento académico en tiempo real:**

**Nombre**: Panel directivo de rendimiento académico en tiempo real

Criterio de aceptación:
```
Dado que el directivo inicia sesión en EduRed
Cuando accede al módulo de reportes
Entonces puede ver el promedio de notas por aula actualizado en los últimos 24 horas
  con filtro por materia, semana y grupo
```

---

**Feature B — Pago de mensualidad en línea:**

**Nombre**: Pago digital de mensualidad sin visita presencial

Criterio de aceptación:
```
Dado que la familia tiene saldo adeudado en el sistema
Cuando ingresa al portal y selecciona "Pagar mensualidad"
Entonces puede completar el pago con tarjeta o transferencia
  y recibe comprobante por correo en menos de 5 minutos
```

---

**Feature C — Gestión de tareas para profesores:**

**Nombre**: Módulo de creación, entrega y calificación de tareas

Criterio de aceptación:
```
Dado que el profesor crea una tarea en la plataforma
Cuando los alumnos la entregan
Entonces el profesor puede calificarla y el alumno recibe la nota
  en su perfil personal en menos de 1 hora
```

---

**Feature D — Migración a la nube:**

**Nombre**: Migración de base de datos on-premise a cloud (habilitadora)

Criterio de aceptación:
```
Dado que la base de datos está migrada al entorno cloud
Cuando el equipo de TI ejecuta las pruebas de carga
Entonces el tiempo de respuesta de las APIs no supera 300ms
  con cero degradación en las features existentes
```

> Nota: La Feature D es un **Enabler** (habilitadora). No entrega valor directo
> al usuario pero habilita las Features A, B y C en futuros PIs.

---

<!-- ============================================ -->
<!-- PASO 2: Team PI Plans — SOLUCIÓN           -->
<!-- ============================================ -->

| Equipo | Feature(s) comprometidas | Dependencia de |
| ------ | ------------------------ | -------------- |
| Alfa   | Feature B (pagos) | Delta (reportes de recibos) |
| Beta   | Feature C (tareas) | Gama (infraestructura de archivos) |
| Gama   | Feature C (soporte) + Feature D (migración) | — |
| Delta  | Feature A (analítica) | Alfa (datos de pagos), Beta (datos de notas) |

> Dependencia crítica: Delta necesita datos de Alfa y Beta — riesgo ROAM "Owned" por Luciana.

---

<!-- ============================================ -->
<!-- PASO 3: PI Objective — SOLUCIÓN            -->
<!-- ============================================ -->

**PI Objective del ART — PI 1:**

"Al final del PI 1, el ART de EduRed habrá entregado **el pago digital de mensualidades**,
**el módulo de tareas para profesores** y **el panel de rendimiento académico**,
lo que permitirá a **directivos, familias y profesores** operar la plataforma sin
procesos presenciales y con visibilidad de datos en tiempo real."

> **Business Value estimado**: Pago digital (10), Tareas (9), Panel (8), Migración (6 — habilitadora)
