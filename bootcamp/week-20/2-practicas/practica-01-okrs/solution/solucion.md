<!-- ============================================ -->
<!-- Semana 20: OKRs y Métricas de Valor        -->
<!-- Práctica 01 — Escritura de OKRs            -->
<!-- solution/solucion.md                        -->
<!-- ============================================ -->

# Solución — Escritura de OKRs: UrbanRent

---

<!-- ============================================ -->
<!-- PASO 1: Reescribir el Objective del equipo  -->
<!-- ============================================ -->

**Objective del equipo (Q3) — reescrito:**

> Ser el primer destino de búsqueda de espacios para el nómada profesional latinoamericano.

**Por qué funciona:**
- Es **cualitativo** (no tiene número) e **inspirador** (pinta una imagen)
- Se alinea directamente con el OKR de empresa ("plataforma de referencia")
- No dice cómo lograrlo (eso es trabajo de los KRs), solo adónde ir
- Un equipo puede recordarlo sin mirar el doc

**Por qué el original no funcionaba:**
"Mejorar la experiencia del usuario en la app" es genérico (todo equipo podría usarlo),
orientado a output implícito (mejorar la app = cambiar features) y no conecta con "nómadas".

---

<!-- ============================================ -->
<!-- PASO 2: Key Results correctos               -->
<!-- ============================================ -->

**KR 1:**
> Aumentar la tasa de retención mensual de usuarios nómada de 51% a 65% para el 30 de septiembre.

*Tipo*: Outcome — mide si el usuario vuelve (comportamiento), no si lanzamos algo.
*Stretch*: +14 pp en 3 meses es ambicioso pero alcanzable con mejoras de onboarding y búsqueda.

**KR 2:**
> Reducir el tiempo desde registro hasta primera reserva de 18 min a 8 min para el 15 de septiembre.

*Tipo*: Outcome — mide la fricción real del usuario en el flujo de compra.
*Baseline*: 18 min (dato dado). Target: 8 min (benchmark de plataformas similares).

**KR 3:**
> Aumentar la proporción de reservas de perfil nómada de 26% (310/1.200) a 40% del total para el 30 de septiembre.

*Tipo*: Outcome — mide si el segmento objetivo crece dentro del total de la plataforma.
*Nota*: Expresa el 310/1.200 como porcentaje para facilitar el seguimiento sin depender del volumen total.

---

<!-- ============================================ -->
<!-- PASO 3: Antipatrones en el borrador         -->
<!-- ============================================ -->

| KR del borrador | Antipatrón detectado | Justificación |
|-----------------|----------------------|---------------|
| KR 1: "Lanzar el nuevo flujo de búsqueda en julio" | **KR de output (entrega)** | "Lanzar X" es una tarea, no un resultado medible. Podemos lanzar el flujo y que nadie lo use. No tiene baseline ni target de comportamiento. |
| KR 2: "Los usuarios deben estar más felices con la plataforma" | **KR no medible** | No tiene métrica concreta (¿NPS? ¿CSAT? ¿porcentaje?), no tiene baseline ni target numérico. Es imposible saber si se cumplió. |
| KR 3: "Aumentar las reservas en un 30% para el 30 de septiembre" | **Ambiguo — podría ser válido pero falta baseline explícito** | El porcentaje (30%) es usable, pero no dice si refiere solo a nómadas o a todas las reservas. Sin baseline declarado (1.200 → 1.560 o 310 → 403) no se puede hacer seguimiento semanal objetivo. |

**Nota sobre el KR 3 de Helena**: No es incorrecto de raíz (tiene fecha y porcentaje), pero mezcla
output implícito ("reservas" mide el negocio, no el comportamiento del segmento nómada) y le falta
el baseline explícito. Válido como KPI de negocio, parcialmente válido como KR de outcome.

---

<!-- ============================================ -->
<!-- REFLEXIÓN FINAL                             -->
<!-- ============================================ -->

**¿Cuál es la diferencia entre un KR de outcome y uno de output?**

Un KR de **output** mide lo que el equipo entrega ("lanzar el flujo de búsqueda"). Un KR de
**outcome** mide el cambio que esa entrega produce en el comportamiento del usuario ("reducir
el tiempo de primera reserva de 18 a 8 minutos"). En UrbanRent podemos lanzar 10 features
(output) y que los nómadas sigan tardando 20 minutos en reservar (cero outcome). Lo que importa
es el cambio real en el usuario, no el volumen de trabajo entregado.
