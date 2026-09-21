# Log

Registro cronológico, append-only. No editar entradas pasadas — solo agregar al final.

## [2026-09-21] setup | Creación de la wiki (Paso 0)

- Se creó la estructura `/wiki` (`fuentes/`, `conceptos/`, `entidades/`, `sintesis/`, `index.md`, `log.md`) y `CLAUDE.md` en la raíz, replicando y adaptando el formato de organización y análisis usado en el repositorio `programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `wiki/`), a pedido explícito del usuario ("aplica el formato de organizacion y analisis de la informacion aplicado en el repo de innovacion del mismo github").
- El `CLAUDE.md` de este repo no es una copia literal: incorpora las reglas propias de este proyecto de grado (fuente exclusiva, citación exacta con número de página, APA 7, sin datos = decirlo, retroalimentación crítica activa) como requisitos obligatorios del flujo INGEST, más estrictos que en el repositorio de referencia.
- Se relevaron los 35 documentos de la raíz del repo (30 PDF + 5 DOCX) y se listaron en `index.md`, agrupados solo por lo que indica el nombre de archivo (procedimientos/anexos SGC-DCI, normativa nacional, Plan 365, planes/documentos técnicos, correspondencia). No se leyó el contenido completo de ningún documento en este paso, salvo el ya cubierto abajo.
- Se migró `procedimiento-asistencia-tecnica-pr06.md` (análisis ya existente en la raíz del repo, previo a esta wiki) a `wiki/fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md`, reorganizado bajo el schema de front matter y con `status: ingerido`. No se agregó contenido nuevo respecto al análisis original; se marcó como `[INCIERTO]` la falta de número de página exacto por cada dato, pendiente de una relectura dirigida a citación APA.
- El archivo `procedimiento-asistencia-tecnica-pr06.md` de la raíz se eliminó tras la migración (su contenido íntegro quedó preservado en `wiki/fuentes/`).
- El INGEST detallado de las 34 fuentes restantes queda pendiente, para procesarse **una por vez** según el flujo por defecto de `CLAUDE.md`, salvo que el usuario pida explícitamente un procesamiento en lote.
