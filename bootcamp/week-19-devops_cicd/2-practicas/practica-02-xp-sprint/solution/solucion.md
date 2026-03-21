<!-- Semana 19: Práctica 02 — Prácticas XP — SOLUCIÓN -->
<!-- GreenField: gestión de áreas verdes urbanas        -->

<!-- ============================================ -->
<!-- PASO 1: Tests TDD — SOLUCIÓN               -->
<!-- ============================================ -->

**Test CA-1 — Alerta si no hubo inspección en 30 días:**

```javascript
test("genera alerta si el parque no tuvo inspección en 30 días", () => {
  const parque = crearParque({ ultimaInspeccion: hace31Dias() });
  const alertas = verificarAlertas(parque);
  expect(alertas).toContain("ALERTA: Park #parque.id requiere inspección");
});
```

**Test CA-2 — Configurar frecuencia de inspección:**

```javascript
test("permite configurar frecuencia de 7, 14 o 30 días por parque", () => {
  const parque = crearParque({ id: 1 });
  configurarFrecuencia(parque, 14); // 14 días
  expect(parque.frecuenciaInspeccion).toBe(14);
  expect(() => configurarFrecuencia(parque, 20)).toThrow("Frecuencia no válida");
});
```

**Test CA-3 — Reasignación automática:**

```javascript
test("reasigna inspector si el asignado está de vacaciones", () => {
  const inspector = crearInspector({ disponible: false });
  const inspectorSuplente = crearInspector({ disponible: true });
  const inspeccion = crearInspeccion({ inspector });
  const asignado = reasignarSiNoDisponible(inspeccion, [inspector, inspectorSuplente]);
  expect(asignado.id).toBe(inspectorSuplente.id);
});
```

> **Clave TDD**: estos tests se escriben ANTES del código.
> Al ejecutarlos por primera vez, todos deben FALLAR (el código no existe aún).

---

<!-- ============================================ -->
<!-- PASO 2: Pair Programming — SOLUCIÓN        -->
<!-- ============================================ -->

**Par recomendado**: **Jair** (driver/navigator) + **Priya** (navigator/driver)

**Justificación:**
- Jair conoce el módulo legacy — puede navegar la complejidad del código existente
- Priya es fuerte en tests — puede identificar oportunidades de cobertura mientras Jair explica el legacy
- Rotar roles cada 25 min: cuando Jair codifica, Priya detecta donde faltan tests. Cuando Priya codifica, Jair revisa decisiones de diseño.
- Tomás queda disponible para otras historias sin bloquear al par.

> El objetivo secundario es **transferencia de conocimiento**: Priya aprende el legacy
> y el conocimiento deja de estar en una sola persona.

---

<!-- ============================================ -->
<!-- PASO 3: Argumento a Valeria — SOLUCIÓN     -->
<!-- ============================================ -->

**Miguel responde a Valeria:**

"Valeria, tienes razón en que el refactoring toma tiempo — aproximadamente el
20% del tiempo de cada historia. Pero considera esto:

En los últimos 4 Sprints tuvimos bugs en producción en 2 de ellos.
Cada bug en producción nos costó en promedio 8 horas: 2 de análisis, 3 de corrección,
2 de regresión y 1 de comunicación con clientes.

El módulo de inspecciones tiene 3 áreas con código sin tests. La próxima vez que
toquemos esas áreas, el riesgo de bug es alto. Si incluimos refactoring en la DoD
ahora, invertimos 2 horas adicionales por historia. Si no lo hacemos y sale un bug,
invertimos 8 horas no planificadas más impacto en la confianza del cliente.

Propuesta concreta: incluimos refactoring solo para historias que toquen módulos
legacy (no para historias nuevas). Evaluamos el impacto en el Sprint 7."
