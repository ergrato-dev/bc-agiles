<!-- ============================================ -->
<!-- PASO 1: Clasificación — SOLUCIÓN           -->
<!-- ============================================ -->

## Clasificación de deuda técnica

| ID   | Descripción breve                             | Tipo de deuda    | Justificación |
| ---- | --------------------------------------------- | ---------------- | ------------- |
| DT-01 | Auth sin tests, sin actualizar 6 meses       | **Involuntaria + Acumulada** | Nadie decidió no hacer tests; ocurrió por velocidad en el año 1. Lleva 6 meses acumulándose. |
| DT-02 | PDF solo para tipo A (hardcodeado)            | **Deliberada**   | El equipo tomó la decisión consciente de hardcodear y no generalizar para entregar más rápido. Nunca se pagó. |
| DT-03 | Queries sin índices, 3–5 seg                  | **Acumulada**    | Empezó con datos pequeños (sin impacto). Al crecer el volumen, la deuda se volvió visible. |
| DT-04 | Monolito que impide separar flujos            | **De Diseño**    | Decisión de arquitectura inicial que ahora limita la evolución del sistema. Requiere refactor estructural. |

---

<!-- ============================================ -->
<!-- PASO 2: Cuantificación — SOLUCIÓN          -->
<!-- ============================================ -->

## Cuantificación del impacto

**DT-01 — Auth sin tests:**

El módulo de autenticación es la puerta de entrada de todos los usuarios.
Sin tests, cualquier cambio futuro puede romper el flujo de login o registro
sin que el equipo lo detecte a tiempo. En una app de salud, una falla de acceso
puede impedir que un paciente reciba una alerta crítica. Riesgo: **alto**.

**DT-02 — PDF solo tipo A:**

Los pacientes tipo B y C (estimado: 40% de usuarios activos según datos del PO)
no pueden exportar su historial. Médicos reportan que deben generar los reportes
manualmente. Impacto directo: experiencia degradada + trabajo manual reprocesado.
Riesgo: **medio-alto** (retención de usuarios afectada).

**DT-03 — Queries lentas:**

Consultas de historial tardan 3–5 seg. Con el crecimiento actual (20% más usuarios
cada mes), en 2 meses el tiempo estimado sería 8–12 seg, cruzando el umbral de
abandonamiento de usuarios. Agregar índices hoy = 2 puntos. Hacerlo en 6 meses
con más datos = refactor mayor de 8–13 puntos. Riesgo: **medio, pero urgente**.

**DT-04 — Monolito:**

Las próximas 3 features del Product Backlog (flujo de prescripciones, panel médico,
notificaciones diferenciadas) requieren separar los flujos paciente/médico.
Sin resolver DT-04, cada una de esas features tendrá overhead de +30–50% en
estimación. Es un multiplicador de deuda. Riesgo: **alto a largo plazo**.

---

<!-- ============================================ -->
<!-- PASO 3: Propuesta de negociación — SOLUCIÓN -->
<!-- ============================================ -->

## Propuesta de Beatriz a Catalina

**Capacidad estimada del Sprint 7**: ~38 puntos

**Aplicando la regla del 20%:**

Puntos para nuevas features: **30**
Puntos para deuda técnica: **8**

**Priorización (impacto × urgencia):**

| Prioridad | ID   | Estimación (pts) | ¿Entra en Sprint 7? |
| --------- | ---- | ---------------- | ------------------- |
| 1 (urgente + alto riesgo) | DT-03 | 2 | ✅ Sí |
| 2 (alto impacto usuario)  | DT-02 | 5 | ✅ Sí |
| 3 (riesgo seguridad)      | DT-01 | 8 | ❌ No (entra en Sprint 8) |
| 4 (arquitectura largo plazo) | DT-04 | 13 | ❌ No (requiere spike ANTES) |

**Total deuda en Sprint 7**: 2 + 5 = **7 puntos** (dentro del 20% ≈ 8 pts)

**Argumento clave para Catalina:**

"Catalina, DT-03 nos cuesta 2 puntos hoy. En 2 meses será un refactor de 13.
DT-02 impide que el 40% de los pacientes exporte su historial — es un bug activo.
Invertir 7 puntos ahora protege la velocidad de los próximos 3 Sprints
y evita que la deuda bloquee las features que ya tienes priorizadas."

---

<!-- ============================================ -->
<!-- PASO 4: Enabler Stories — SOLUCIÓN         -->
<!-- ============================================ -->

## Backlog de Enabler Stories

**Enabler 1 (para DT-03 — Queries lentas):**

Como equipo de desarrollo, quiero agregar índices a las consultas de historial
para que las respuestas sean menores a 500ms y el sistema soporte el crecimiento
proyectado sin degradación de experiencia.

**Criterio de aceptación:**
- Dado que un médico consulta el historial de un paciente con 12 meses de datos
  Cuando ejecuta la búsqueda
  Entonces el sistema responde en menos de 500ms con los resultados completos

---

**Enabler 2 (para DT-02 — PDF hardcodeado):**

Como equipo de desarrollo, quiero generalizar el módulo de exportación de PDF
para que soporte todos los tipos de paciente (A, B y C) con un formato dinámico.

**Criterio de aceptación:**
- Dado que un paciente de tipo B o C está autenticado
  Cuando solicita exportar su historial
  Entonces el sistema genera un PDF con sus datos correctos sin error
