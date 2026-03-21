<!-- ============================================ -->
<!-- Semana 21: Agile Coaching                   -->
<!-- Práctica 01 — Solución                      -->
<!-- solution/solucion.md                        -->
<!-- ============================================ -->

# Solución — Stance Correcto: CivicHub / Marina

---

<!-- ============================================ -->
<!-- PASO 1: Escenario A — SM sin estructura     -->
<!-- ============================================ -->

**Stance correcto: Mentor**

**Justificación**: Gabriela tiene una brecha de conocimiento específica (cómo estructurar un
Sprint Planning). Pregunta "¿cómo se hace?", que es exactamente la señal para usar el stance
Mentor. No tiene sentido hacerle coaching sobre "qué quiere lograr en su rol" cuando la
necesidad es práctica e inmediata. Trainer sería válido si hubiera más de una persona en la
situación (taller grupal), pero es 1:1 con una pregunta concreta → Mentor.

**Qué haría Marina concretamente**:
Comparte su experiencia: "Yo estructuro el Sprint Planning en 3 bloques: (1) ¿Qué queremos
lograr? → Sprint Goal, 30 min con PO. (2) ¿Qué hacemos? → selección del backlog, 45 min.
(3) ¿Cómo lo hacemos? → descomposición en tareas, 45 min." Le muestra un ejemplo de agenda
con tiempos y le sugiere que Gabriela la adapte al equipo de CivicHub.

**Stance que NO debería usar**: Coach. Hacerle preguntas del tipo "¿qué quieres tú?" cuando
alguien tiene una necesidad técnica inmediata es ineficiente y frustrante. El coaching puro
funciona para creencias limitantes, no para brechas de conocimiento práctico.

---

<!-- ============================================ -->
<!-- PASO 2: Escenario B — Equipo sin feedback   -->
<!-- ============================================ -->

**Stance correcto: Facilitador**

**Justificación**: La Retrospectiva de CivicHub no genera feedback real, no porque el equipo
no quiera, sino porque la dinámica de la reunión no crea el espacio seguro para hacerlo.
El Developer senior dominante es una señal de dinámica de poder no gestionada.
Marina como Facilitador puede diseñar una estructura diferente que neutralice esa dinámica.

**Técnica concreta**: Silent Brainstorming (escritura individual antes de compartir).
Marina pide a cada persona que anote en post-its o notas digitales sus observaciones del
sprint (qué funcionó / qué mejorar) durante 5 minutos en silencio individual, antes de
compartir con el grupo. Esto elimina el efecto de ancla del Developer dominante, ya que
todos tienen sus ideas formadas antes de escuchar a los demás.

**¿Hay algo sistémico?**: Sí. El silencio sobre los deploys manuales que causaron 4 horas
de retraso es alarmante. Probablemente hay miedo a señalar problemas técnicos. Esto sugiere
baja seguridad psicológica, que no se resuelve solo con facilitación. Marina debería hacer
un Team Assessment en las próximas 2 semanas para diagnosticar el nivel de seguridad
psicológica del equipo.

---

<!-- ============================================ -->
<!-- PASO 3: Escenario C — Andrés paralizado     -->
<!-- ============================================ -->

**Stance correcto: Coach**

**Justificación**: Andrés no tiene una brecha de conocimiento técnico (lleva 2 años en CivicHub).
Tiene una creencia limitante: "no soy suficientemente bueno". Esto es terreno de coaching puro.
Darle instrucciones, asignarle un mentor técnico o facilitarle una reunión de feedback no toca
la causa raíz. La creencia hay que trabajarla con preguntas que él mismo responda.

**3 preguntas poderosas para Marina:**

1. "¿Qué significaría para ti que esta PR fuera aprobada sin cambios?" *(explora el valor que
   Andrés asocia a la aprobación del trabajo → puede revelar que confunde calidad del código
   con valor personal)*

2. "¿Hubo alguna PR tuya que fue aprobada con pocos cambios o que el equipo valorara?
   ¿Qué fue diferente en esos casos?" *(rompe el pensamiento de todo-o-nada, busca evidencia
   contraria a la creencia)*

3. "¿Qué te diría la versión de Andrés en 3 años, mirando este momento?" *(cambia de perspectiva
   temporal y reduce la carga emocional del presente)*

**¿Cuándo cambiar de stance?**: Si Marina descubre que las PRs de Andrés son rechazadas porque
el proceso de code review del equipo es inconsistente o el criterio de "hecho" no está definido,
el problema escala al nivel de equipo (falta de Definition of Done clara). En ese punto, Marina
sale del coaching individual y trabaja con todo el equipo para definir criterios de DoD
explícitos. El problema "individual" de Andrés podría tener causa sistémica.
