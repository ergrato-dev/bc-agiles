<!-- ============================================ -->
<!-- Semana 22: Facilitación Avanzada            -->
<!-- Práctica 02 — Solución                      -->
<!-- solution/solucion.md                        -->
<!-- ============================================ -->

# Solución — Design Thinking: SocialCare / Valentina

---

<!-- ============================================ -->
<!-- PASO 1: Mapa de Empatía — Rosa              -->
<!-- ============================================ -->

| Cuadrante | Datos de la conversación |
|-----------|--------------------------|
| **¿Qué piensa y siente?** | Miedo a equivocarse y perder todo lo llenado. Preocupación por no entender palabras técnicas del formulario. Vergüenza implícita de no poder hacerlo sin ayuda. Esperanza de poder completarlo sola si el sistema fuera más claro. |
| **¿Qué dice y hace?** | "Quería hacerlo sola" → intenta la autonomía. "Me da miedo equivocarme" → evita avanzar cuando no está segura. Abandona el formulario sin completar. Espera a Javier para continuar. |
| **¿Qué ve?** | Formulario con 18 campos. Términos que no reconoce. Una interfaz que no le comunica progreso ni le dice qué pasará si se equivoca. |
| **¿Qué escucha?** | A Javier diciendo que la ayuda tarde (llega a las 19h). Información implícita de que "el sistema no funciona bien de noche" (posible retraso del servidor). |

**Mayor pain point de Rosa:**
> Rosa no puede completar el formulario sola porque no entiende algunos términos y teme que
> un error borre todo su progreso, lo que la paraliza y la hace depender de su hijo que no
> siempre está disponible.

---

<!-- ============================================ -->
<!-- PASO 2: HMW                                 -->
<!-- ============================================ -->

**HMW 1 — Válido:**
> ¿Cómo podríamos hacer que Rosa entienda cada campo sin tener que llamar a alguien, para
> que pueda completar el formulario de forma autónoma y sin miedo a equivocarse?

*Por qué es válido*: Abierto (no prescribe la solución: podría ser tooltip, lenguaje simple,
video, etc.), centrado en el usuario (Rosa), orientado a un outcome claro (autonomía).

**HMW 2 — Válido:**
> ¿Cómo podríamos permitir que Rosa guarde y retome su formulario en cualquier momento, para
> que Javier pueda ayudarla cuando está disponible sin perder el progreso?

*Por qué es válido*: Reconoce el contexto real (Javier ayuda tarde), centrado en comportamiento
real del usuario, abierto a múltiples soluciones (auto-guardado, link compartible, sesión temporal).

**HMW 3 — Con error:**
> ¿Cómo podríamos agregar tooltips explicativos en cada campo del formulario para reducir
> el abandono del 72%?

*Explicación del error*: Este HMW ya prescribe la solución (tooltips). Un buen HMW no debe
incluir la solución en el enunciado. También usa una métrica (72%) como objetivo, lo que
es propio de un KR, no de un HMW. El correcto sería: "¿Cómo podríamos ayudar a Rosa a
entender qué se le pide en cada campo?"

**HMW seleccionado**: HMW 1 — la autonomía de Rosa es el pain point central según el mapa.

---

<!-- ============================================ -->
<!-- PASO 3: Crazy 8s — Ideas                    -->
<!-- ============================================ -->

Ideas generadas para el HMW 1:

1. Cambiar todos los campos a lenguaje simple (sin términos jurídicos)
2. Agregar un botón "¿Qué significa esto?" con explicación en lenguaje cotidiano
3. Crear un modo "fácil" vs modo "completo" al inicio del formulario
4. Mostrar un ejemplo de respuesta correcta en cada campo (placeholder visual)
5. Leer el campo en voz alta al hacer clic (accesibilidad de audio)
6. Mostrar una barra de progreso con nombre de cada etapa ("Paso 2 de 4: Datos personales")
7. Agregar un "modo simulacro" donde Rosa puede practicar sin enviar datos reales
8. Whatsapp bot que guía campo a campo con mensajes de texto simples

**Ideas seleccionadas para prototipar:**

**Idea A**: Modo "simulacro" / formulario de práctica
*Justificación*: Rosa no completa el formulario por miedo a equivocarse. Un modo de práctica
sin consecuencias reales elimina directamente ese bloqueo. No requiere rediseñar el formulario
existente; es una capa adicional. Alta probabilidad de impacto con bajo riesgo técnico.

**Idea B**: Explicación "¿Qué significa esto?" + lenguaje simple en campos clave
*Justificación*: Los términos incomprensibles son el segundo bloqueo. Una ayuda contextual
accesible con lenguaje cotidiano tiene bajo costo de implementación y puede probarse con texto
estático (sin programar el backend).

---

<!-- ============================================ -->
<!-- PASO 4: Prototipo y Testeo                  -->
<!-- ============================================ -->

**Prototipo Idea A — Modo simulacro:**
- Tipo: **Role playing** + formulario impreso
- Descripción: Valentina imprime el formulario real. Escribe en la parte superior "MODO PRÁCTICA
  — Nada que escribas aquí se enviará". Pide a Rosa que lo llene como si fuera de verdad, sabiendo
  que no tiene consecuencias.
- Tiempo estimado: 20 minutos para preparar + 15 minutos de sesión

**Criterio de éxito para testear Idea A:**
Rosa completa el formulario impreso hasta el final (sin detenerse ni pedir ayuda) en ≤ 12 minutos.
Si se detiene: anotar en qué campo y por qué. Si llega al final: la hipótesis del "miedo al error"
se confirma como causa raíz del abandono.
*Nota*: NO el criterio "Rosa dice que le gustó el modo práctica". Medir el comportamiento, no la opinión.

**Prototipo Idea B — Ayuda contextual de lenguaje simple:**
- Tipo: **Documento Word / Google Doc** con la lista de campos difíciles y su traducción
- Descripción: El UX Designer crea en 30 min un documento con los 5 campos más complejos del
  formulario y una explicación de cada uno en máximo 2 oraciones en lenguaje cotidiano.
  Durante el testeo, Valentina le da el documento a Rosa para que lo consulte mientras llena el formulario.
- Tiempo estimado: 30 minutos para construir el documento

**Criterio de éxito para testear Idea B:**
Rosa llena los 5 campos "difíciles" sin preguntar qué significa ninguno, usando solo el documento.
Si consulta el doc y completa el campo → la ayuda contextual es suficiente.
Si consulta el doc y aun así pregunta → el lenguaje del doc necesita simplificarse más.
