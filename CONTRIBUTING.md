# Guía de Contribución

¡Gracias por tu interés en mejorar el Bootcamp de Metodologías Ágiles! Toda contribución es bienvenida, desde correcciones menores hasta nuevas prácticas completas.

---

## 📋 Antes de Empezar

- Lee el [Código de Conducta](CODE_OF_CONDUCT.md) — es obligatorio para participar.
- Revisa los [Issues abiertos](https://github.com/ergrato-dev/bc-agiles/issues) para evitar duplicados.
- Para cambios grandes, abre primero un Issue describiendo lo que propones.

---

## 🚀 Flujo de Contribución

```bash
# 1. Haz fork del repositorio en GitHub

# 2. Clona tu fork
git clone https://github.com/TU_USUARIO/bc-agiles.git
cd bc-agiles

# 3. Crea una rama descriptiva
git checkout -b feat/week-05-tshirt-sizing

# 4. Realiza tus cambios

# 5. Confirma con Conventional Commits
git commit -m "feat(week-05): agregar práctica de estimación T-Shirt Sizing"

# 6. Empuja tu rama
git push origin feat/week-05-tshirt-sizing

# 7. Abre un Pull Request desde GitHub
```

---

## 📝 Convención de Commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/). El formato es:

```
tipo(scope): descripción corta en presente

Cuerpo opcional con más detalle.
```

| Tipo | Cuándo usarlo |
|---|---|
| `feat` | Nueva práctica, semana, diagrama o plantilla |
| `fix` | Corrección de error en contenido o SVG |
| `docs` | Mejora de README, glosario o documentación |
| `refactor` | Reestructuración sin cambio de contenido |
| `style` | Formato, espaciado, typos sin cambio de sentido |

**Ejemplos:**
```
feat(week-09): agregar práctica de User Stories con criterios Gherkin
fix(week-17): escapar ampersand en SVG de frameworks escalados
docs(week-03): ampliar definición de Definition of Done en glosario
```

---

## 🗂️ Qué Puedes Contribuir

### ✅ Contribuciones bienvenidas

- **Nuevos escenarios de práctica**: casos de estudio realistas para semanas existentes
- **Diagramas SVG**: visualizaciones adicionales (tableros, burndown, org charts)
- **Correcciones de contenido**: errores en artefactos, soluciones de referencia o glosario
- **Mejoras de plantillas**: plantillas más claras, mejor estructuradas o más completas
- **Traducciones**: inglés u otros idiomas para semanas existentes
- **Recursos adicionales**: ebooks gratuitos, videos o referencias verificadas

### ❌ Fuera del alcance

- Cambiar la estructura pedagógica de las 24 semanas (requiere discusión previa)
- Agregar herramientas al stack (GitHub Projects + Markdown es intencional)
- Soluciones completas de proyectos que puedan ser copiadas por aprendices

---

## 🎨 Estándares de Contenido

### Archivos Markdown

- Teoría: **máximo 120 líneas** por archivo
- Títulos de sección: numerados (`## 1.`, `## 2.`...)
- Términos técnicos ágiles en **inglés** (Sprint, Backlog, Scrum Master, etc.)
- Explicaciones en **español**

### Diagramas SVG

- Tema dark: fondo `#1a1a2e`, elementos `#16213e`
- Colores: azul `#0052CC`, verde `#36B37E`, naranja `#FF8B00`
- Sin gradientes — colores sólidos únicamente
- Fuentes sans-serif: Inter, Roboto o System UI

### User Stories (cuando aplique)

```markdown
Como [rol] quiero [acción] para [beneficio].
```
Con criterios de aceptación en Gherkin (Dado/Cuando/Entonces).

---

## 🔍 Proceso de Revisión

1. Un mantenedor revisará tu PR en un plazo razonable
2. Se puede pedir cambios antes de hacer merge
3. Una vez aprobado, el mantenedor hace el merge

No todos los PRs son aceptados — si una propuesta no encaja con los objetivos pedagógicos del bootcamp, se explicará el motivo en los comentarios.

---

## 🐛 Reportar Problemas

Usa [GitHub Issues](https://github.com/ergrato-dev/bc-agiles/issues) e incluye:

- **Semana y archivo afectado** (ej: `week-12/1-teoria/02-velocity.md`)
- **Descripción clara del problema**
- **Sugerencia de corrección** (opcional pero útil)

---

## 💬 Preguntas

Para preguntas generales o propuestas de mejora, usa [GitHub Discussions](https://github.com/ergrato-dev/bc-agiles/discussions).
