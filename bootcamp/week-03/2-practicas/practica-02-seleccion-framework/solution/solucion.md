<!-- Semana 03: Panorama de Frameworks Ágiles -->
<!-- Práctica 02 — Solución de referencia -->

# Práctica 02 — Solución

---

<!-- ============================================ -->
<!-- PASO 1: Análisis del contexto — SOLUCIÓN   -->
<!-- ============================================ -->

**¿El trabajo llega en lotes planificados o de forma impredecible?**
Los contratos definen entregables trimestrales y el PM escribe specs planificadas.
El trabajo es **mayormente planificable** aunque los bugs críticos son reactivos.

**¿Los requisitos cambian frecuentemente?**
Los módulos de análisis y reportes regulatorios **cambian cada ciclo contractual**
(3 meses). Variabilidad media: no tan alta como un startup sin producto definido,
pero suficiente para que un proceso waterfall sea inadecuado.

**¿Cuántos equipos coordinar?**
Actualmente **1 equipo de 6 personas**: no necesita Scaled Agile.

**¿Cultura técnica para TDD/CI?**
**No**. Sin tests automatizados, sin CI. XP requiere un nivel técnico mínimo
que VerdeLab aún no tiene. Scrum puede coexistir con mejora técnica gradual.

---

<!-- ============================================ -->
<!-- PASO 2: Framework recomendado — SOLUCIÓN   -->
<!-- ============================================ -->

**Framework seleccionado:** **Scrum** (con elementos de XP como objetivo de 6 meses)

**Justificaciones:**
1. El trabajo llega en lotes planificados: los Sprints de 2 semanas permiten
   comprometerse con el PM y con el cliente sin sorpresas.
2. Los stakeholders (laboratorios) quieren visibilidad: la Sprint Review
   regular genera confianza durante el proceso de due diligence.
3. Sin retrospectivas actuales: la Retrospectiva de Scrum introduce por primera
   vez la mejora continua en el proceso del equipo.

**Framework descartado: XP**
XP requiere TDD desde el inicio. El equipo no tiene la cultura técnica ni las
herramientas para eso hoy. Introducir XP completo en una startup sin tests
crearía resistencia y abandono prematuro del framework.

---

<!-- ============================================ -->
<!-- PASO 3: Plan de adopción — SOLUCIÓN         -->
<!-- ============================================ -->

| Semana | Práctica | Por qué primero |
| ------ | --------- | --------------- |
| 1 | Daily Scrum de 15 min + tablero visual | Crea visibilidad del trabajo sin cambiar nada más |
| 2 | Sprint Planning simple (2h) con Sprint Goal | Define compromiso concreto por período |
| 3 | Sprint Review con el PM como primer stakeholder | El PM ve el progreso; se reduce reunión de "reporte" al CEO |
| 4 | Retrospectiva con formato Start/Stop/Continue | Primera acción de mejora registrada y asignada |

---

<!-- ============================================ -->
<!-- PASO 4: Escenario futuro — SOLUCIÓN         -->
<!-- ============================================ -->

**¿Cambiaría el framework con 3 equipos?**
Con 3 equipos en el mismo producto aparece el problema de dependencias entre
equipos. La opción más simple es **Scrum of Scrums** (una reunión semanal entre
los Scrum Masters de cada equipo) antes de adoptar SAFe o LeSS. SAFe tiene
sentido cuando los 3 equipos trabajan en un programa coordinado con múltiples
releases simultáneas, lo que VerdeLab no necesita en Serie B.

**Problema nuevo con 3 equipos:**
Las historias de usuario que dependen de trabajo de dos equipos se bloquean
mutuamente. Sin coordinación explícita, el velocity de cada equipo sube pero
el producto integrado nunca puede desplegarse porque siempre falta algo del
otro equipo.
