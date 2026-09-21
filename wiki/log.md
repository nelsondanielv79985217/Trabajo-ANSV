# Log

Registro cronológico, append-only. No editar entradas pasadas — solo agregar al final.

## [2026-09-21] setup | Creación de la wiki (Paso 0)

- Se creó la estructura `/wiki` (`fuentes/`, `conceptos/`, `entidades/`, `sintesis/`, `index.md`, `log.md`) y `CLAUDE.md` en la raíz, replicando y adaptando el formato de organización y análisis usado en el repositorio `programaGradoInnovacion` (rama `claude/llm-wiki-setup-nht7xw`, carpeta `wiki/`), a pedido explícito del usuario ("aplica el formato de organizacion y analisis de la informacion aplicado en el repo de innovacion del mismo github").
- El `CLAUDE.md` de este repo no es una copia literal: incorpora las reglas propias de este proyecto de grado (fuente exclusiva, citación exacta con número de página, APA 7, sin datos = decirlo, retroalimentación crítica activa) como requisitos obligatorios del flujo INGEST, más estrictos que en el repositorio de referencia.
- Se relevaron los 35 documentos de la raíz del repo (30 PDF + 5 DOCX) y se listaron en `index.md`, agrupados solo por lo que indica el nombre de archivo (procedimientos/anexos SGC-DCI, normativa nacional, Plan 365, planes/documentos técnicos, correspondencia). No se leyó el contenido completo de ningún documento en este paso, salvo el ya cubierto abajo.
- Se migró `procedimiento-asistencia-tecnica-pr06.md` (análisis ya existente en la raíz del repo, previo a esta wiki) a `wiki/fuentes/ansv-pr-06-procedimiento-asistencia-tecnica.md`, reorganizado bajo el schema de front matter y con `status: ingerido`. No se agregó contenido nuevo respecto al análisis original; se marcó como `[INCIERTO]` la falta de número de página exacto por cada dato, pendiente de una relectura dirigida a citación APA.
- El archivo `procedimiento-asistencia-tecnica-pr06.md` de la raíz se eliminó tras la migración (su contenido íntegro quedó preservado en `wiki/fuentes/`).
- El INGEST detallado de las 34 fuentes restantes queda pendiente, para procesarse **una por vez** según el flujo por defecto de `CLAUDE.md`, salvo que el usuario pida explícitamente un procesamiento en lote.

## [2026-09-21] ingest | ANSV-CPP-PR-07 (Anexo 3 — estrategias interinstitucionales)

- Por pedido del usuario ("Empieza con PR-07, CA-02 y los anexos del bundle PR-06"), se inició el INGEST del bundle documental del PR-06, comenzando por el PR-07.
- Se extrajo el texto completo del PDF (9 páginas) con `pypdf`, preservando la paginación original, y se creó `wiki/fuentes/ansv-pr-07-estrategias-interinstitucionales.md` con `status: ingerido` y cita de página exacta en cada dato.
- Hallazgo relevante: el PR-07 declara explícitamente al PR-06 como documento asociado (p. 9), pero el PR-06 no declara al PR-07 (su sección de documentos asociados dice "No aplica") — relación asimétrica documentada como incertidumbre en ambas páginas.
- Se actualizó la página del PR-06 con el link cruzado al PR-07 y se actualizó `index.md` (de 1 a 2 fuentes ingeridas, familia SGC-DCI de 5 a 4 pendientes).
- No se crearon páginas de concepto/entidad nuevas en este paso: DCI, ANSV, PNSV y los firmantes ya están cubiertos por el ingest del PR-06; se evalúa crear una página de concepto o entidad propia recién cuando haya evidencia de cruce con una tercera fuente.
- Pendiente: continuar con CA-02 (Anexo 1) y los demás anexos del bundle, de a uno, según lo acordado con el usuario.
