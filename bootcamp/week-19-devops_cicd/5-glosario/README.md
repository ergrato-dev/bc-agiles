# 📖 Glosario — Semana 19: DevOps y CI/CD

Términos clave de DevOps, CI/CD y prácticas XP. Ordenados A–Z.

---

**CALMS**
Framework conceptual de DevOps: Culture, Automation, Lean, Measurement, Sharing.
Describe los 5 pilares de una organización DevOps madura.

**CD — Continuous Delivery**
Práctica que garantiza que el software siempre está en un estado desplegable,
aunque el despliegue requiera aprobación manual.

**CD — Continuous Deployment**
Extensión de Continuous Delivery donde cada cambio que pasa los tests se despliega
automáticamente a producción sin intervención manual.

**CI (Continuous Integration)**
Práctica de integrar cambios de código al repositorio principal varias veces al día,
con tests automatizados que validan cada integración.

**Change Failure Rate**
Métrica DORA: porcentaje de despliegues que causan incidentes o rollbacks en producción.
Equipos de élite: ≤ 15% de change failure rate.

**Deployment Frequency**
Métrica DORA: con qué frecuencia se despliega a producción.
Equipos de élite: múltiples veces por día.

**DORA Metrics**
Cuatro métricas clave de DevOps: Deployment Frequency, Lead Time for Changes,
Change Failure Rate y MTTR. Definidas por el grupo de investigación DevOps Research and Assessment.

**Integration Hell**
Antipatrón: equipos que integran código solo al final del Sprint o del proyecto.
Causa conflictos masivos, regresiones y despliegues fallidos.

**MTTR (Mean Time To Recover)**
Tiempo promedio para recuperarse de un incidente en producción.
Equipos de élite: menos de 1 hora.

**Pair Programming**
Práctica XP: dos desarrolladores trabajan juntos en el mismo código.
Uno escribe (driver), el otro revisa (navigator). Mejora calidad y transfiere conocimiento.

**Refactoring**
Proceso de mejorar el diseño interno del código sin cambiar su comportamiento externo.
En Scrum, es parte de la DoD en equipos con prácticas técnicas maduras.

**TDD (Test-Driven Development)**
Práctica XP: se escribe el test ANTES de escribir el código.
Ciclo: test rojo → código mínimo → test verde → refactorizar.

**XP (Extreme Programming)**
Framework ágil enfocado en prácticas técnicas de excelencia: TDD, Pair Programming,
Continuous Integration, Refactoring, Small Releases.
Complementa a Scrum definiendo CÓMO codificar bien.
