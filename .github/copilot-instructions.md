# 🤖 Instrucciones para GitHub Copilot

## 📋 Contexto del Bootcamp

Este es un **Bootcamp de Metodologías Ágiles de Cero a Héroe** estructurado
para llevar a estudiantes desde cero conocimiento sobre gestión ágil de
proyectos hasta un nivel de Scrum Master Junior, Product Owner Junior o
Agile Coach Junior.

### 📊 Datos del Bootcamp

- **Duración**: 24 semanas (~6 meses)
- **Dedicación semanal**: 8 horas
- **Total de horas**: ~192 horas
- **Nivel de entrada**: Cero (sin experiencia previa en metodologías ágiles)
- **Nivel de salida**: Scrum Master Junior / Product Owner Junior / Agile Coach Junior
- **Enfoque**: Progresión desde el Manifiesto Ágil hasta Scaled Agile y transformación organizacional
- **Herramienta principal**: GitHub Projects (visualización de tableros) + Markdown (artefactos y documentación)

---

## 🎯 Objetivos de Aprendizaje

Al finalizar el bootcamp, los estudiantes serán capaces de:

- ✅ Aplicar los valores y principios del Manifiesto Ágil en proyectos reales
- ✅ Facilitar todos los eventos de Scrum: Sprint Planning, Daily Scrum, Sprint Review y Retrospectiva
- ✅ Redactar y priorizar User Stories con criterios de aceptación claros
- ✅ Construir y refinar un Product Backlog ordenado y estimado
- ✅ Utilizar métricas ágiles: Velocity, Burndown Chart, Cumulative Flow Diagram
- ✅ Gestionar impedimentos y facilitar la mejora continua del equipo
- ✅ Aplicar técnicas de facilitación para retrospectivas efectivas
- ✅ Escalar Scrum con marcos como SAFe, LeSS o Nexus
- ✅ Prepararse para certificaciones: PSM I, PSPO I o PMI-ACP

---

## 📚 Estructura del Bootcamp

### Distribución por Etapas

#### **Etapa 0: Fundamentos Ágiles (Semanas 1–8)** — 64 horas

- Historia del desarrollo de software: del ciclo en cascada al Manifiesto Ágil
- Los 4 valores y 12 principios del Manifiesto Ágil
- Panorama de frameworks ágiles: Scrum, Kanban, XP, SAFe
- Introducción a Scrum: roles, eventos y artefactos
- **Roles**: Scrum Master, Product Owner, Equipo de Desarrollo
- **Eventos**: Sprint, Sprint Planning, Daily Scrum, Sprint Review, Retrospectiva
- **Artefactos**: Product Backlog, Sprint Backlog, Incremento
- Definition of Done (DoD) y Definition of Ready (DoR)
- Introducción a Kanban: tablero, columnas, WIP limits
- Comparativa Scrum vs. Kanban vs. Scrumban

#### **Etapa 1: Scrum Practicante (Semanas 9–16)** — 64 horas

- User Stories: formato, criterios de aceptación, INVEST
- Épicas, Features, Stories y Tasks: jerarquía del backlog
- Técnicas de estimación: Planning Poker, T-Shirt Sizing, #NoEstimates
- Refinamiento del Product Backlog (Backlog Refinement)
- Sprint Planning: capacidad del equipo, Sprint Goal, descomposición de tareas
- Velocity y Capacity Planning
- Métricas: Burndown Chart, Burnup Chart, Velocity Chart, CFD
- Gestión de impedimentos y escalación
- Facilitación de Sprint Reviews y Demo efectiva con stakeholders
- Técnicas de retrospectiva: 4Ls, Start/Stop/Continue, Fishbone, Mad/Sad/Glad
- Mejora continua: Kaizen y acciones de retrospectiva con seguimiento

#### **Etapa 2: Ágil Avanzado (Semanas 17–24)** — 64 horas

- Scaled Agile: SAFe (Scaled Agile Framework), LeSS, Nexus
- Kanban avanzado: políticas explícitas, clases de servicio, cadencias, métricas de flujo
- DevOps y CI/CD en contexto ágil: la integración entre desarrollo y operaciones
- OKRs (Objectives & Key Results) y alineación estratégica con el backlog
- Agile Coaching: niveles de coaching, estilos de conversación, stance del Agile Coach
- Técnicas de facilitación avanzada: Liberating Structures, Design Thinking
- Transformación organizacional ágil: journey map, resistencia al cambio
- Preparación para certificaciones: PSM I (Scrum.org), PSPO I, PMI-ACP

---

## 🗂️ Estructura de Carpetas

Cada semana sigue esta estructura estándar:

```
bootcamp/week-XX/
├── README.md                  # Descripción y objetivos de la semana
├── rubrica-evaluacion.md      # Criterios de evaluación detallados
├── 0-assets/                  # Diagramas SVG (flujos, tableros, mapas)
├── 1-teoria/                  # Material teórico (archivos .md)
├── 2-practicas/               # Simulaciones y casos de estudio guiados
│   └── practica-XX/
│       ├── README.md          # Instrucciones y pasos del caso
│       ├── starter/
│       │   ├── contexto.md    # Descripción del escenario
│       │   └── plantilla.md   # Plantilla con secciones a completar
│       └── solution/
│           ├── contexto.md
│           └── solucion.md    # Ejemplo de solución comentada
├── 3-proyecto/                # Proyecto integrador semanal
│   ├── README.md
│   └── starter/
│       ├── contexto.md        # Escenario genérico adaptable al dominio
│       └── entregables.md     # TODOs para que el aprendiz implemente
├── 4-recursos/                # Recursos adicionales
│   ├── ebooks-free/
│   ├── videografia/
│   └── webgrafia/
└── 5-glosario/                # Términos ágiles clave (A–Z)
    └── README.md
```

### 📁 Carpetas Raíz

- **`_assets/`**: Recursos visuales globales (logos, headers, banners)
- **`_docs/`**: Documentación general del bootcamp
- **`_scripts/`**: Scripts de automatización y utilidades
- **`bootcamp/`**: Contenido semanal del bootcamp

### 🗂️ Orden de Creación de Cada Semana

Al desarrollar el contenido de una nueva semana, seguir **siempre** este orden:

1. `README.md` — Descripción general, objetivos, distribución del tiempo, navegación
2. `rubrica-evaluacion.md` — Tabla de criterios y puntajes
3. `1-teoria/` — Archivos markdown numerados (`01-`, `02-`, …)
4. `0-assets/` — Diagramas SVG vinculados a la teoría
5. `2-practicas/` — Casos de estudio con `starter/` + `solution/`
6. `3-proyecto/` — Proyecto integrador semanal
7. `4-recursos/` — Ebooks gratuitos, videografía, webgrafía
8. `5-glosario/README.md` — Términos ágiles de la semana ordenados A–Z

---

## 🎓 Componentes de Cada Semana

### 1. Teoría (1-teoria/)

- Archivos markdown con explicaciones conceptuales
- Escenarios y diálogos situacionales que ilustren los conceptos
- Referencia a diagrama SVG al inicio (después de objetivos)
- Referencias a documentación oficial (Scrum Guide, Agile Manifesto, etc.)

#### 📏 Límites de Extensión (NON-NEGOTIABLE)

El público objetivo tiene déficit de atención. Textos extensos generan
abandono. Seguir el patrón del bootcamp SQL hermano (`bc-sql`):

| Elemento           | Límite                                          |
| ------------------ | ----------------------------------------------- |
| Líneas por archivo | **Máximo 120**                                  |
| Objetivos          | 3–4 ítems                                       |
| Secciones          | 4–6 secciones numeradas (`## 1.`, `## 2.`...)   |
| Checklist          | **4 ítems** formulados como preguntas concretas |
| Referencias        | 2–3 links                                       |

**Qué NO incluir en teoría:**

- ❌ Tablas de comparación de más de 4 filas
- ❌ Transcripciones completas de la Scrum Guide (enlazar en su lugar)
- ❌ Secciones de "Herramientas recomendadas" (van en `4-recursos/`)
- ❌ Notas de certificación extensas (una línea `>` es suficiente)
- ❌ Más de 2 ejemplos de caso por sección

### 2. Prácticas (2-practicas/)

Las prácticas son **simulaciones guiadas**, NO tareas abiertas. El aprendiz
aprende completando plantillas con instrucciones paso a paso.

#### 📋 Formato de Prácticas

**README.md de la práctica:**

```markdown
### Paso 1: Nombre del Concepto

Explicación del concepto con ejemplo de contexto:

> **Escenario**: El equipo de desarrollo de una app de delivery lleva 3 sprints
> sin entregar valor. El Scrum Master nota que el Daily Scrum dura 40 minutos.

**Abre `starter/plantilla.md`** y completa la sección correspondiente.
```

**starter/plantilla.md:**

```markdown
<!-- ============================================ -->
<!-- PASO 1: Nombre del Concepto                 -->
<!-- ============================================ -->

<!-- Instrucción: Analiza el escenario y responde -->

**¿Cuál es el impedimento principal?**

<!-- Tu respuesta aquí -->

**¿Qué haría el Scrum Master en este caso?**

<!-- Tu respuesta aquí -->
```

**solution/solucion.md:**

```markdown
<!-- ============================================ -->
<!-- PASO 1: Nombre del Concepto — SOLUCIÓN      -->
<!-- ============================================ -->

**¿Cuál es el impedimento principal?**

El Daily Scrum se ha convertido en una reunión de reporte al Scrum Master
en lugar de una sincronización del equipo. Esto viola el evento tal como
lo define la Scrum Guide.

**¿Qué haría el Scrum Master en este caso?**

Facilitar una retrospectiva enfocada en el formato del Daily...
```

#### ❌ NO usar este formato en prácticas:

```markdown
<!-- ❌ INCORRECTO — Este formato es para PROYECTOS, no prácticas -->
Tarea: Diseña un Sprint Planning completo para tu equipo. <!-- TODO: completar -->
```

#### ✅ Usar este formato en prácticas:

```markdown
<!-- ✅ CORRECTO — Plantilla guiada con secciones claras -->
<!-- Completa el Sprint Goal según el formato: "Para [beneficio] el equipo [acción]" -->
**Sprint Goal:**
<!-- Tu respuesta aquí -->
```

### 3. Proyecto (3-proyecto/)

A diferencia de las prácticas, el proyecto SÍ usa TODOs para que el
estudiante implemente desde cero.

**Las instrucciones de los proyectos deben ser genéricas y adaptables a
cualquier dominio de negocio.**

#### 🏛️ Política de Dominios Únicos (Anticopia)

**Cada aprendiz recibe un dominio único asignado por el instructor:**

- 📱 App de delivery de comida
- 🛒 E-commerce de ropa
- 🏦 App bancaria digital
- 🎓 Plataforma educativa online
- 🏥 Sistema de gestión de citas médicas
- 🚗 App de movilidad urbana
- 🎮 Videojuego mobile
- 🏋️ App de fitness y bienestar
- 📰 Portal de noticias digital
- 🏠 Plataforma de alquiler de inmuebles
- 🎵 App de streaming de música
- 🌱 App de sostenibilidad ambiental
- Y otros dominios únicos según cantidad de aprendices

**Objetivo**: Prevenir copia entre estudiantes y fomentar implementaciones
originales.

**⚠️ IMPORTANTE para desarrollo de contenidos:**

- Los ejemplos en los proyectos **NO deben usar dominios de la lista anterior**
- Usar ejemplos genéricos o dominios diferentes (ej: sistema de gestión de biblioteca municipal, plataforma de adopción de mascotas)
- Esto evita "regalar" soluciones a aprendices con esos dominios asignados

#### 📋 Formato del starter del proyecto:

```markdown
<!-- ============================================ -->
<!-- PROYECTO SEMANAL: [Título Genérico]         -->
<!-- Semana XX — [Tema]                          -->
<!-- ============================================ -->

<!-- NOTA PARA EL APRENDIZ:                      -->
<!-- Adapta este proyecto a tu dominio asignado. -->
<!-- Ejemplos:                                   -->
<!--   App delivery   → pedidos, riders, zonas   -->
<!--   E-commerce     → productos, carrito, envíos-->
<!--   App bancaria   → cuentas, transacciones   -->
<!--   Plataforma edu → cursos, estudiantes      -->

<!-- TODO: Definir el nombre del producto en tu dominio -->
**Nombre del Producto**: [nombre de tu producto]

<!-- TODO: Redactar la Product Vision en formato elevator pitch -->
**Product Vision**:
Para [segmento de usuarios] que [necesitan/quieren algo],
[nombre del producto] es un [categoría]
que [beneficio principal].
A diferencia de [alternativa actual],
nuestro producto [diferenciador clave].

<!-- TODO: Crear el Product Backlog inicial con mínimo 10 User Stories -->
## Product Backlog Inicial

| ID   | User Story | Prioridad | Estimación |
| ---- | ---------- | --------- | ---------- |
| US-01 | <!-- TODO --> | Alta | <!-- TODO --> |
```

### 4. Recursos (4-recursos/)

- **ebooks-free/**: Libros y guías gratuitas sobre ágil y Scrum
- **videografia/**: Videos, charlas TED y conferencias recomendadas
- **webgrafia/**: Documentación oficial, artículos y referencias

### 5. Glosario (5-glosario/)

- Términos ágiles ordenados alfabéticamente
- Definiciones claras y concisas en español
- Ejemplos contextuales cuando aplique
- Diferenciación entre términos similares (ej: Scrum Master vs. Project Manager)

---

## 📝 Convenciones de Documentación

### Estilo de Escritura

```markdown
<!-- ✅ BIEN — Explicaciones en voz activa, segunda persona, ejemplos concretos -->
## ¿Qué es el Sprint Goal?

El Sprint Goal es el **objetivo único** que da coherencia al Sprint.
Lo define el equipo durante el Sprint Planning y no cambia durante el Sprint.

**Ejemplo concreto:**
> "Implementar el flujo completo de registro y login para que los usuarios
> puedan crear cuentas y acceder a la plataforma."

<!-- ❌ MAL — Voz pasiva, jerga sin definir, demasiado abstracto -->
## Sprint Goal

Es un objetivo que es establecido por los participantes del evento de
planeación denominado Sprint Planning, el cual es definido como...
```

### Reglas de Nomenclatura de Archivos

- **Teoría**: `01-manifiesto-agil.md`, `02-roles-scrum.md` (numerados, kebab-case)
- **Prácticas**: `practica-01-daily-scrum/`, `practica-02-retrospectiva/`
- **Assets SVG**: `flujo-sprint.svg`, `roles-scrum.svg`, `tablero-kanban.svg`
- **Glosario**: `README.md` (un único archivo por semana, ordenado A–Z)

### Formato de Plantillas y Artefactos

- Títulos en **español** (es contenido educativo)
- Campos `<!-- TODO: ... -->` para proyectos, secciones guiadas para prácticas
- Tablas simples de máximo 5 columnas
- User Stories siempre en formato: `Como [rol] quiero [acción] para [beneficio]`

### Convenciones de User Stories

```markdown
<!-- ✅ CORRECTO — Formato INVEST, criterios de aceptación en Gherkin -->
**US-001: Registro de usuario**

Como **usuario nuevo** quiero **crear una cuenta con email y contraseña**
para **acceder a las funcionalidades de la plataforma**.

**Criterios de Aceptación:**
- Dado que el usuario está en la pantalla de registro
  Cuando ingresa un email válido y una contraseña de mínimo 8 caracteres
  Entonces el sistema crea la cuenta y envía un email de confirmación

- Dado que el usuario ingresa un email ya registrado
  Cuando hace clic en "Registrarse"
  Entonces el sistema muestra el mensaje "Este email ya está en uso"

**Estimación**: 3 puntos | **Prioridad**: Must Have

<!-- ❌ INCORRECTO — Sin formato, sin criterios, sin valor de negocio -->
Hacer el login del usuario.
```

---

## 🌐 Idioma y Nomenclatura

### ⚠️ REGLA CRÍTICA: Terminología Técnica + Español Educativo

**TÉRMINOS TÉCNICOS ÁGILES: MANTENER EN INGLÉS (son nombres propios)**

- ✅ Scrum, Sprint, Backlog, Kanban, Burndown, Velocity, DoD, DoR
- ✅ Product Owner, Scrum Master, Stakeholder, Epic, Story
- ✅ Daily Scrum, Sprint Review, Sprint Retrospective, Sprint Planning
- ✅ WIP (Work In Progress), CFD (Cumulative Flow Diagram)
- ✅ SAFe, LeSS, Nexus, DevOps, CI/CD, OKR

**EXPLICACIONES Y DOCUMENTACIÓN: SIEMPRE EN ESPAÑOL**

- ✅ Descripciones, instrucciones y definiciones
- ✅ READMEs y documentación
- ✅ Comentarios en plantillas
- ✅ Títulos de secciones de teoría

### Ejemplos Correctos

```markdown
<!-- ✅ CORRECTO — Términos técnicos en inglés, explicación en español -->
## ¿Qué es el Product Backlog?

El Product Backlog es la lista ordenada de todo lo que podría necesitar
el producto. El Product Owner es el responsable de mantenerlo actualizado.
Cada ítem del backlog se llama Product Backlog Item (PBI).
```

---

## 🎨 Recursos Visuales y Estándares de Diseño

### Formato de Assets

- ✅ **Preferir SVG** para todos los diagramas (flujos, tableros, mapas mentales, timelines)
- ❌ **NO usar ASCII art** para diagramas o visualizaciones
- ✅ Usar PNG/JPG solo para screenshots de herramientas reales

### Tema Visual

- 🌙 **Tema dark** para todos los assets visuales
- ❌ **Sin degradés** (gradients) en diseños
- ✅ Colores sólidos y contrastes claros
- ✅ Paleta base: `#0052CC` (azul Jira/Atlassian) para elementos principales
- ✅ Acento: `#36B37E` (verde) para estados "Done"/completados
- ✅ Alerta: `#FF8B00` (naranja) para impedimentos/bloqueados
- ✅ Fondos: `#1a1a2e` y `#16213e`

### Tipografía

- ✅ **Fuentes sans-serif** exclusivamente
- ✅ Recomendadas: Inter, Roboto, Open Sans, System UI
- ❌ **NO usar fuentes serif**

### Tipos de Diagramas por Semana

| Tipo de Diagrama          | Cuándo usar                           |
| ------------------------- | ------------------------------------- |
| Tablero Scrum (SVG)       | Semanas de Scrum events               |
| Burndown Chart (SVG)      | Semanas de métricas                   |
| Mapa de roles (SVG)       | Semana 2 (roles Scrum)                |
| Flujo del Sprint (SVG)    | Semana 5 (ciclo completo)             |
| CFD — Cumulative Flow (SVG)| Semanas de Kanban avanzado           |
| Org chart ágil (SVG)      | Semanas de Scaled Agile               |

---

## 🛠️ Herramientas del Bootcamp

### Stack Principal

| Herramienta        | Uso en el Bootcamp                                   |
| ------------------- | ----------------------------------------------------- |
| **GitHub Projects** | Simulación de tableros Scrum/Kanban                  |
| **Markdown**        | Artefactos: Backlogs, DoD, User Stories, Actas       |
| **Miro / FigJam**   | Retrospectivas colaborativas (semanas presenciales)  |
| **Git**             | Control de versiones de los entregables              |
| **VS Code**         | Editor principal para todos los archivos `.md`       |

### GitHub Projects como Tablero Scrum

Las semanas 5–8 usan GitHub Projects para simular un tablero Scrum real:

```markdown
## Cómo configurar el tablero

1. Crea un nuevo Project en GitHub (tipo Board)
2. Configura las columnas: Backlog | To Do | In Progress | In Review | Done
3. Crea Issues para las User Stories del Sprint
4. Asigna estimaciones con labels: `1pt`, `2pt`, `3pt`, `5pt`, `8pt`
5. Asigna el Sprint Goal como descripción del Milestone
```

---

## 🔐 Mejores Prácticas

### Diseño de Contenido Ágil

- Usar **escenarios realistas** de equipos reales (no ejemplos genéricos tipo "empresa X")
- Incluir **antipatrones comunes** y cómo reconocerlos/corregirlos
- Presentar **dilemas reales**: ¿Qué hace el Scrum Master cuando el PO quiere agregar ítems al Sprint en curso?
- Mostrar la **curva de aprendizaje** honesta: Scrum es simple de entender, difícil de dominar

### Calidad de los Artefactos

- Toda User Story debe cumplir el criterio **INVEST**: Independiente, Negociable, Valiosa, Estimable, Small (pequeña), Testeable
- Los criterios de aceptación deben estar en formato **Gherkin** (Dado/Cuando/Entonces)
- Los Sprint Goals deben ser **medibles y orientados al valor** del usuario
- Las rúbricas de evaluación deben alinearse con prácticas reales de equipos ágiles

### Antipatrones que NO se deben usar en contenido

- ❌ Llamar "Scrum Master" a alguien que solo gestiona tareas (es un rol de facilitación y coaching)
- ❌ Presentar el Sprint Planning como una simple asignación de tareas
- ❌ Mostrar retrospectivas como reuniones de quejas sin acciones de mejora
- ❌ Confundir velocity con productividad absoluta
- ❌ Presentar el Daily Scrum como un reporte de status al Scrum Master

---

## 📊 Evaluación

Cada semana incluye **tres tipos de evidencias**:

1. **Conocimiento 🧠** (30%): Cuestionarios sobre conceptos ágiles, identificación de antipatrones
2. **Desempeño 💪** (40%): Simulaciones prácticas ejecutadas correctamente
3. **Producto 📦** (30%): Artefacto entregable funcional adaptado al dominio asignado

### Criterios de Aprobación

- Mínimo **70%** en cada tipo de evidencia
- Entrega puntual de proyectos
- Artefactos completos y coherentes con el dominio asignado
- **Originalidad**: Sin copia de implementaciones de otros aprendices

---

## 🚀 Metodología de Aprendizaje

### Estrategias Didácticas

- **Aprendizaje Basado en Proyectos (ABP)**: Proyectos semanales que simulan situaciones reales de equipos ágiles
- **Dominios Únicos**: Cada aprendiz aplica conceptos a su producto/empresa asignada
- **Role Playing**: Simulaciones de eventos Scrum (Planning, Daily, Review, Retro)
- **Estudio de Casos Reales**: Análisis de equipos que adoptaron (o fallaron en adoptar) ágil
- **Práctica Deliberada**: Ejercicios con complejidad incremental
- **Peer Review**: Revisión de artefactos entre aprendices

### Distribución del Tiempo (8h/semana)

- **Teoría**: 2–2.5 horas
- **Prácticas**: 3–3.5 horas
- **Proyecto**: 2–2.5 horas

---

## 🤖 Instrucciones Específicas para Copilot

### Límites de Respuesta

1. **Divide respuestas largas**
   - ❌ **NUNCA generar respuestas que superen los límites de tokens**
   - ✅ **SIEMPRE dividir contenido extenso en múltiples entregas**
   - ✅ Crear contenido por secciones, esperar confirmación del usuario
   - Para semanas completas: dividir por carpetas (`teoria → practicas → proyecto`)

### Generación de Contenido Ágil

1. **Usa siempre las convenciones definidas**
   - User Stories en formato: `Como [rol] quiero [acción] para [beneficio]`
   - Criterios de aceptación en Gherkin: `Dado/Cuando/Entonces`
   - Términos técnicos en inglés, explicaciones en español

2. **Progresión pedagógica**
   - Etapa 0 (semanas 1–8): conceptos puros con escenarios sencillos
   - Etapa 1 (semanas 9–16): aplicación práctica con simulaciones completas
   - Etapa 2 (semanas 17–24): escenarios complejos y scaled agile

3. **Artefactos estructurados**
   - Incluir siempre un `contexto.md` con el escenario de startup/empresa
   - Comenzar con `<!-- Semana XX: Tema -->` en el encabezado de cada plantilla
   - Usar `<!-- ===================================== -->` como separador de secciones

### Creación de Contenido

1. **Estructura clara y progresiva**
   - De lo simple a lo complejo
   - Conceptos construidos sobre conocimientos previos
   - Repetición espaciada de conceptos clave (ej: el Sprint Goal aparece en múltiples semanas)

2. **Escenarios del mundo real**
   - Situaciones que un Scrum Master o PO encontrará en el trabajo
   - Datos y contextos realistas (no "Empresa A" o "Equipo B")
   - Dilemas frecuentes en adopciones ágiles y cómo resolverlos

3. **Equilibrio teoría–práctica**
   - No más del 30% de cada semana debe ser teoría pura
   - El 70% restante debe ser aplicación, simulación o proyecto

### Diagramas SVG de Flujos Ágiles

- Usar notación visual clara con íconos representativos
- Incluir etiquetas en español en los diagramas
- Tema dark: fondo `#1a1a2e`, elementos `#16213e`, bordes `#0052CC`
- Mostrar solo los elementos relevantes al tema de la semana
- Para tableros Scrum: columnas `Backlog | To Do | In Progress | Review | Done`

---

## 📚 Referencias Oficiales

- **Scrum Guide** (2020): https://scrumguides.org/
- **Agile Manifesto**: https://agilemanifesto.org/
- **Scrum.org** (PSM I): https://www.scrum.org/
- **Kanban Guide**: https://kanban.university/
- **SAFe Framework**: https://scaledagileframework.com/
- **Mountain Goat Software** (Mike Cohn): https://www.mountaingoatsoftware.com/
- **Liberating Structures**: https://www.liberatingstructures.com/

---

## 🔗 Enlaces Importantes

- **Repositorio**: https://github.com/ergrato-dev/bc-agiles
- **Documentación general**: [\_docs/README.md](_docs/README.md)
- **Primera semana**: [bootcamp/week-01/README.md](bootcamp/week-01/README.md)

---

## ✅ Checklist para Nuevas Semanas

Cuando crees contenido para una nueva semana:

- [ ] Crear estructura de carpetas completa
- [ ] `README.md` con objetivos, estructura y navegación
- [ ] Material teórico en `1-teoria/` (máx. 120 líneas por archivo)
- [ ] Diagrama SVG en `0-assets/` (mínimo 1 por semana)
- [ ] Prácticas guiadas en `2-practicas/` (mínimo 2 prácticas)
- [ ] Plantillas `starter/` con secciones comentadas y TODOs claros
- [ ] Soluciones de referencia en `solution/`
- [ ] Proyecto integrador en `3-proyecto/` con dominio genérico
- [ ] Recursos adicionales en `4-recursos/`
- [ ] Glosario de términos ágiles en `5-glosario/`
- [ ] Rúbrica de evaluación con los 3 tipos de evidencia
- [ ] Verificar coherencia con semanas anteriores
- [ ] Revisar progresión de dificultad
- [ ] Confirmar que los artefactos de ejemplo NO usan dominios de la lista anticopia
- [ ] **Etapa 1–2**: verificar que los escenarios incluyan antipatrones y cómo resolverlos
- [ ] **Etapa 2**: confirmar que el contenido de Scaled Agile hace referencia al framework correcto (SAFe/LeSS/Nexus)

---

## 💡 Notas Finales

- **Prioridad**: Claridad sobre exhaustividad
- **Enfoque**: Aplicación práctica sobre teoría abstracta
- **Objetivo**: Preparar facilitadores, coaches y líderes de producto listos para trabajar en equipos ágiles reales
- **Filosofía**: Scrum como framework de inspección y adaptación, no como receta rígida
- **Diferenciador clave**: Los aprendices salen siendo capaces de *facilitar* eventos ágiles, no solo de describirlos

---

_Última actualización: Marzo 2026_
_Versión: 1.0_
