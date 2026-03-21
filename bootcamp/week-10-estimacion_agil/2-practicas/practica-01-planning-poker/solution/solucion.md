<!-- ============================================ -->
<!-- PASO 1: Solución — Tabla de estimaciones  -->
<!-- Semana 10 — Planning Poker                 -->
<!-- ============================================ -->

## Ronda de estimación — SOLUCIÓN

| ID    | User Story (resumen)                          | Consenso | Razonamiento                                              |
| ----- | --------------------------------------------- | -------- | --------------------------------------------------------- |
| US-10 | Listado de proyectos activos                  | **2**    | UI simple, datos ya en DB. Levemente más que la referencia |
| US-11 | Filtrar proyectos por estado                  | **3**    | Componente de filtro + lógica de estados. Descartamos el 5 de Pablo por ser UI simple |
| US-12 | Subir fotos desde teléfono                    | **8**    | Upload mobile requiere compresión, storage S3 y permisos. Lucía se alineó tras discutir el backend |
| US-13 | Email automático 7 días antes                 | **5**    | Consenso sin divergencia: job scheduler + template email |
| US-14 | Cliente aprueba/rechaza avances               | **8**    | Ver análisis detallado abajo                              |
| US-15 | Exportar informe PDF                          | **13**   | Pablo votó 21: coincide en complejidad pero el equipo acordó 13 porque ya existe librería de PDF |
| US-16 | Mapa con proyectos geográficos                | **21**   | Integración con API de mapas + geolocalización. Considerar dividir |
| US-17 | Admin: métricas de uso semanal                | **3**    | Query + tabla simple en panel admin ya existente          |

**Total estimado**: 2+3+8+5+8+13+21+3 = **63 puntos** (4–5 sprints)

---

<!-- ============================================ -->
<!-- PASO 2: Solución — Divergencia US-14       -->
<!-- ============================================ -->

## Divergencia US-14 — SOLUCIÓN COMENTADA

**Cartas reveladas:** Lucía: 5 · Marcos: 13 · Elena: 8 · Pablo: 8

**¿Por qué Lucía ve 5 puntos?**
Lucía solo visualizó la parte de UI: dos botones (Aprobar/Rechazar) y un
campo de texto para el comentario. Desde Frontend parece similar a un
formulario de contacto simple.

**¿Por qué Marcos ve 13 puntos?**
Marcos pensó en todo el flujo Backend: sistema de invitación al cliente
(no tiene cuenta), token de acceso seguro, notificación al contractor,
historial de aprobaciones y posibles estados adicionales (Pendiente /
Aprobado / Rechazado / Solicitud de cambios).

**Preguntas que Tomás debería hacer:**
1. "Lucía, ¿asumiste que el cliente ya tiene cuenta en la plataforma?"
2. "Marcos, ¿cómo se entera el cliente de que tiene un avance para revisar?"

**Estimación final tras la discusión: 8 puntos**
El equipo acordó que el MVP incluye solo aprobación para clientes con
cuenta existente creada por el contractor. La invitación por código o
email queda en una Story separada (US-14b). Con este alcance: 8 pts es
correcto.

**Lección**: La divergencia reveló un assumption no compartido sobre
el alcance. El Planning Poker cumplió su función de alinear al equipo.

---

<!-- ============================================ -->
<!-- PASO 3: Solución — Decisiones post-sesión  -->
<!-- ============================================ -->

## Reflexión post-sesión — SOLUCIÓN

**¿Qué Story debería dividirse?**
**US-16** (21 pts): Demasiado grande para un Sprint. División sugerida:
- US-16a: Ver dirección textual de cada proyecto (2 pts)
- US-16b: Integrar mapa con pins por proyecto usando Google Maps (8 pts)
- US-16c: Filtrar proyectos en el mapa por estado (5 pts)

**¿Story con mayor incertidumbre técnica?**
US-12 — el ? lo mereció en la primera ronda porque dependía de si el
backend ya tenía storage S3 configurado (no estaba claro).

**Selección para Sprint 3 (capacidad ~22 pts):**
US-10 (2) + US-11 (3) + US-13 (5) + US-17 (3) + US-14 (8) = **21 pts** ✅
US-16 queda para después de dividirla. US-15 se evalúa si hay capacidad residual.
