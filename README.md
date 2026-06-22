# Arte — Lesson Plans (Instituto Alberto Einstein)

Repositorio de continuidad para los lesson plans semanales de Arte de secundaria (10°, 11°, 12°).

## Estructura
- **`ESTADO.md`** — memoria viva del avance de cada grado. Se lee y se actualiza cada semana.
- **`FORMATO.md`** — formato oficial y reglas de los lesson plans.
- **`CURRICULO.md`** — currículo por grado (referencia conceptual).
- **`lesson-plans/`** — un archivo por semana con los planes de los 3 grados.
- **`modulos/`** — módulos de recuperación y trabajos especiales.

## Rutina automática (cada jueves)
Un agente programado en la nube:
1. Lee `ESTADO.md`, `FORMATO.md` y `CURRICULO.md`.
2. Genera los lesson plans de la **semana siguiente** para 10°, 11° y 12° (2 clases por nivel),
   encadenando el "siguiente paso lógico" de cada grado.
3. Guarda el archivo en `lesson-plans/AAAA-MM-DD-semana.md`.
4. Actualiza `ESTADO.md` con el nuevo avance de cada grado.
5. Sube los cambios en una rama y abre un Pull Request para que Jonathan los revise.

Jonathan revisa el PR el jueves en la mañana, ajusta lo que necesite y lo usa en clase.

<!-- prueba de notificacion 054852 -->
