<!-- ============================================ -->
<!-- Semana 22: Facilitación Avanzada            -->
<!-- Práctica 01 — Solución                      -->
<!-- solution/solucion.md                        -->
<!-- ============================================ -->

# Solución — Retro con LS: DataReach / Patricia

---

<!-- ============================================ -->
<!-- PASO 1: Diagnóstico                         -->
<!-- ============================================ -->

**Causa raíz de que las acciones nunca se ejecuten:**
Las acciones se toman como compromisos grupales difusos del tipo "deberíamos revisar los PRs
antes del viernes". Nadie es responsable individualmente. Un compromiso de equipo sin dueño
nominal es un compromiso que nadie cumple. La estructura de la Retro no fuerza la especificidad:
¿quién hace qué, cuándo, cómo lo sabemos?

**Por qué el dominio de Martín es estructural y no de personalidad:**
En reuniones sin estructura de participación, los patrones de jerarquía informal se activan
automáticamente. El Tech Lead habla más porque el grupo lo espera —es el experto técnico.
Esto no es culpa de Martín; es el resultado de una facilitación que no diseña espacios
explícitos para que todos hablen *antes* de que los más senior lo hagan. El cambio no está
en pedirle a Martín que hable menos, sino en estructurar la sesión para que todos hablen primero.

**Cambio en el diseño de la sesión:**
(1) Usar reflexión individual escrita antes de cualquier conversación grupal — elimina el
efecto de ancla del Tech Lead. (2) Asignar compromisos individuales nominales (no de equipo)
con nombre, fecha y criterio de éxito. (3) Abrir la siguiente Retro revisando si el compromiso
del Sprint anterior se cumplió (retrospectiva de la retrospectiva).

---

<!-- ============================================ -->
<!-- PASO 2: Selección de 3 LS                   -->
<!-- ============================================ -->

**LS 1 — Apertura: TRIZ (15 min)**

*Justificación*: El equipo lleva 8 sprints con los mismos problemas sin nombrarlos directamente.
TRIZ usa la inversión ("¿cómo garantizaríamos el fracaso?") para que el equipo nombre sus
propios antipatrones sin el miedo de la crítica. En un equipo que tiene "cansancio de retro",
la pregunta inversa sorprende y activa la participación. Además, el incidente del reporte
incorrecto tiene una causa que nadie quiere nombrar directamente ("nadie revisa los PRs del
viernes"). TRIZ lo sacará a la luz de forma segura.

**LS 2 — Análisis del incidente: What / So What / Now What (20 min)**

*Justificación*: Después de TRIZ el equipo habrá nombrado comportamientos disfuncionales reales.
W³ permite procesar el incidente en 3 capas sin convertirlo en blame game: (1) ¿qué pasó
factualmente? (hechos, no juicios), (2) ¿qué patrón representa? (el incidente no es único,
es síntoma de algo sistémico), (3) ¿qué hace el equipo diferente desde hoy? La capa "So What"
es la que más falta en las retros tradicionales — el equipo actúa sobre síntomas sin diagnosticar.

**LS 3 — Compromisos: 15% Solutions (20 min)**

*Justificación*: Los compromisos grupales sin dueño no se ejecutan. 15% Solutions obliga a
cada persona a identificar lo que ELLA MISMA puede cambiar sin permiso ni presupuesto. El
resultado son 6 compromisos individuales nominales (uno por persona) en lugar de 1 compromiso
de equipo difuso. Este cambio estructural ataca directamente la causa raíz del paso 1.

---

<!-- ============================================ -->
<!-- PASO 3: Diseño detallado de la sesión       -->
<!-- ============================================ -->

| Bloque | Tiempo | LS / Actividad | Instrucción exacta al equipo | Resultado esperado |
|--------|--------|----------------|------------------------------|-------------------|
| Apertura | 0–5 min | Encuadre | *"Hoy vamos a trabajar diferente. Esta Retro tiene 3 actividades específicas. Antes de empezar, quiero que sepan que el incidente del viernes es el foco, pero no queremos buscar culpables — queremos entender patrones. ¿Todos de acuerdo?"* | Alineación de expectativas, reducción del miedo al blame game. |
| Actividad 1 | 5–20 min | **TRIZ** | *"Primera pregunta: ¿qué haríamos con certeza para garantizar que el próximo Sprint tengamos otro incidente como el del viernes? Escriban en silencio durante 3 minutos. Luego compartimos en voz alta. No hay respuestas incorrectas."* | El equipo nombra 8–12 comportamientos disfuncionales reales, incluyendo "no revisar PRs del viernes". |
| Actividad 2 | 20–40 min | **What/So What/Now What** | *"Ahora tomamos 2 de los comportamientos más frecuentes de la lista. Para cada uno: (1) ¿qué pasó exactamente? Solo hechos. (2) ¿Qué patrón representa? ¿Es la primera vez? (3) ¿Qué cambia desde hoy?"* | El equipo conecta el incidente con patrones estructurales y genera 2–3 áreas de mejora con causa clara. |
| Actividad 3 | 40–55 min | **15% Solutions** | *"Para cada área de mejora, pregunta personal: ¿qué puedes hacer TÚ, esta semana, sin pedir permiso? Escríbelo con tu nombre, qué harás y cuándo. Compartimos en 3 min."* | 6 compromisos individuales nominales. Patricia los captura en el tablero compartido. |
| Cierre | 55–60 min | Revisión | *"El próximo Sprint, abrimos la Retro revisando si los 6 compromisos se cumplieron. Cada quien reporta su propio estado. ¿Alguna duda sobre lo comprometido hoy?"* | Responsabilidad individual visible. El equipo sabe que habrá seguimiento. |
