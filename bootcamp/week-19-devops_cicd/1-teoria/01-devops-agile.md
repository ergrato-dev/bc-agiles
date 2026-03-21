# 01 — DevOps: Cultura, Pipeline y el Ciclo CALMS

## Objetivos

- Entender DevOps como cultura, no solo como herramientas
- Conocer las etapas de un pipeline CI/CD y su relación con el Sprint
- Identificar las métricas DORA para medir la madurez DevOps

---

## 1. DevOps = Dev + Ops + Cultura

DevOps no es un rol ni un cargo. Es un **movimiento cultural** que derriba el muro
entre los equipos de desarrollo y de operaciones para entregar software de forma
continua y confiable.

En Scrum, DevOps permite que el Incremento del Sprint sea **realmente desplegable**,
no solo "funciona en mi máquina".

### El framework CALMS

| Letra | Concepto | Qué significa en la práctica |
| ----- | -------- | ----------------------------- |
| **C** | Culture | Responsabilidad compartida — Dev y Ops co-dueños de la calidad |
| **A** | Automation | Pipelines que ejecutan tests y despliegues sin intervención manual |
| **L** | Lean | Eliminar desperdicio en el ciclo de entrega |
| **M** | Measurement | Métricas DORA: MTTR, Deployment Frequency, etc. |
| **S** | Sharing | Documentación compartida, post-mortems sin culpas |

---

## 2. CI/CD en el ciclo del Sprint

```
Sprint Planning → Desarrollo (Sprints) → Sprint Review
      ↑                    ↓
   Feedback               CI/CD Pipeline
                          ├── CI: tests al hacer commit
                          ├── CD (Delivery): artefacto listo para producción
                          └── CD (Deployment): despliega automáticamente
```

| Etapa | Qué hace | Beneficio para Scrum |
| ----- | -------- | -------------------- |
| **CI (Continuous Integration)** | Integra el código y ejecuta tests en cada commit | Detecta conflictos temprano — evita "integration hell" |
| **CD — Continuous Delivery** | El artefacto siempre está listo para desplegar | Reduce el riesgo de la Sprint Review |
| **CD — Continuous Deployment** | El despliegue es automático sin aprobación manual | Feedback del usuario real en horas, no semanas |

---

## 3. Métricas DORA

Las métricas DORA (DevOps Research and Assessment) miden la elite del rendimiento de entrega:

- **Deployment Frequency**: ¿Con qué frecuencia se despliega a producción?
- **Lead Time for Changes**: ¿Cuánto tarda un commit en llegar a producción?
- **Change Failure Rate**: ¿Qué % de despliegues causan incidentes?
- **MTTR (Mean Time To Recover)**: ¿Cuánto tarda el equipo en resolver un incidente?

> Equipos de élite: deployment frequency diaria o mayor, MTTR < 1 hora.

---

## 4. Antipatrones de DevOps en contextos ágiles

- ❌ "Integration hell": integrar código solo al final del Sprint
- ❌ Equipo de QA manual separado que prueba al final (bloquea la entrega)
- ❌ Pipeline CI/CD que tarda más de 15 minutos (nadie lo espera)
- ❌ Despliegues manuales que solo sabe hacer una persona

---

## Checklist

- [ ] ¿Qué significa la "C" en CALMS y cómo se aplica en Scrum?
- [ ] ¿Cuál es la diferencia entre Continuous Delivery y Continuous Deployment?
- [ ] ¿Qué antipatrón ocurre cuando el equipo integra código solo al final del Sprint?
- [ ] ¿Qué métrica DORA mide qué tan rápido el equipo se recupera de un incidente?

---

## Referencias

- CALMS Framework: <https://www.atlassian.com/devops/frameworks/calms>
- DORA Metrics: <https://dora.dev/>
