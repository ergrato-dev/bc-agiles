<!-- Semana 18: Práctica 02 — Políticas — SOLUCIÓN -->
<!-- EventFlow: plataforma de gestión de eventos    -->

<!-- ============================================ -->
<!-- PASO 1: Políticas — SOLUCIÓN               -->
<!-- ============================================ -->

**Columna: En Producción**

Política de entrada:
- El presupuesto del evento está aprobado por el cliente por escrito
- El brief completo (fecha, lugar, asistentes, catering) está documentado en el sistema
- El ítem tiene un responsable asignado del equipo

Política de salida:
- Todos los proveedores clave (venue, catering, AV) están confirmados
- El cronograma detallado del evento está completo
- La coordinadora de cuenta revisó y aprobó la propuesta técnica

---

**Columna: Revisión Cliente**

Política de entrada:
- El dossier del evento (cronograma, proveedores, presupuesto final) está preparado
- No hay ítems abiertos de "En Producción" que bloqueen la revisión

Política de salida:
- El cliente validó por correo o herramienta la propuesta completa
- No hay ítems de revisión pendientes del cliente (todos respondidos)

---

**Columna: Ejecutado**

Política de entrada:
- El evento se realizó en la fecha y lugar acordados
- El cliente firmó el acta de cierre del evento
- La factura del evento fue emitida y enviada

---

<!-- ============================================ -->
<!-- PASO 2: Clases de servicio — SOLUCIÓN      -->
<!-- ============================================ -->

| Tipo de evento | Clase de servicio | SLA | Color de tarjeta |
| -------------- | ----------------- | --- | ---------------- |
| Congreso anual | **Fecha fija** | Fecha del evento inamovible — inicio 60+ días antes | 🔵 Azul |
| Lanzamiento urgente | **Urgente** | ≤ 10 días desde solicitud | 🔴 Rojo |
| Evento estándar | **Estándar** | 20–30 días desde solicitud | ⬜ Blanco/gris |

---

<!-- ============================================ -->
<!-- PASO 3: Congreso urgente — SOLUCIÓN        -->
<!-- ============================================ -->

**Decisión de Camila:**

Camila activa la política de la **clase de servicio Urgente**.
Identifica cuál de los 3 ítems en "En Producción" puede pausarse o
transferirse temporalmente a otro miembro del equipo para liberar capacidad.

El congreso urgente entra como **tarjeta roja** (clase Urgente) y se coloca
al frente del tablero con bandera visual. El WIP limit se puede exceder
**excepcionalmente** para clases Urgente — pero debe documentarse como excepción
explícita en la política del tablero.

**Justificación:**
Las clases de servicio existen exactamente para esto: dar tratamiento diferenciado
a ítems con restricciones de tiempo distintas. Sin esta política, el equipo
trataría el congreso urgente igual que un evento estándar, lo que causaría
incumplimiento de SLA y pérdida del cliente.

> ⚠️ Camila también notifica al cliente del evento que se está posponiendo
> temporalmente, para mantener transparencia sobre el impacto.
