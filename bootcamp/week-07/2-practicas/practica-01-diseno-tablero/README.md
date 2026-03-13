# Práctica 01 — Diseñar un Tablero Kanban

**Semana 07 — Introducción a Kanban**
**Tiempo estimado**: 1.5 horas

---

## Contexto

> **Escenario**: **HelpDesk360**, una empresa que ofrece soporte técnico
> a empresas medianas, tiene un equipo de 6 personas que gestiona tickets
> de soporte. Actualmente usan una hoja de Excel con columnas Nuevo /
> En Progreso / Resuelto. Los tiempos de respuesta varían mucho: algunos 
> tickets se resuelven en horas, otros llevan 2 semanas sin mover.
> El manager, Roberto, quiere implementar un tablero Kanban real.

---

## Paso 1: Mapear el flujo de trabajo real

Antes de diseñar el tablero, hay que entender cómo viaja realmente un
ticket desde que llega hasta que se cierra. Roberto describe el proceso:

```
1. El cliente reporta un ticket por email o chat
2. El equipo lo lee y decide si tiene toda la info para trabajarlo
3. Si falta información, se le pide al cliente
4. Cuando se tiene todo, el técnico comienza a investigar el problema
5. Una vez encontrada la solución, se aplica el fix
6. Se verifica que el fix funcione en el entorno del cliente
7. Se le notifica al cliente y se cierra el ticket
```

Define las columnas del tablero Kanban que reflejen este flujo real.
Algunos pasos pueden combinarse o separarse según el equipo.

**Abre `starter/plantilla.md`** y completa la Sección 1.

---

## Paso 2: Definir WIP limits

Para las columnas de trabajo activo (no Backlog ni Done), define un WIP
limit razonado. El equipo tiene 6 técnicos especializados:

- 2 técnicos en nivel 1 (responden tickets simples)
- 2 técnicos en nivel 2 (investigan problemas complejos)  
- 1 técnico senior (revisión de soluciones y escalados)
- 1 manager (supervisión)

**Abre `starter/plantilla.md`** y completa la Sección 2.

---

## Paso 3: Política explícita de columna

Escribe la política explícita para la columna "En Verificación" del
tablero. Una política explícita responde: ¿Qué condición debe cumplir
un ítem para ENTRAR a esta columna? ¿Y para SALIR?

**Abre `starter/plantilla.md`** y completa la Sección 3.
